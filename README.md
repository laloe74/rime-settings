## 基本套路：

-   Squirrel 0.16.2 简体 全拼
-   「[袖珍简化字方案](https://github.com/rime/rime-pinyin-simp)」作为基础
    -   [简繁切换](https://github.com/rime/home/issues/388#issuecomment-504572224)
    -   [动态日期、时间、星期](https://github.com/KyleBing/rime-wubi86-jidian)
    -   所有标点符号直接上屏，「/」模式改为「v」模式，「/」直接上屏
    -   删除了「[Emoji](https://github.com/rime/rime-emoji)」，改为词语与符号映射
    -   增加了许多拼音纠错
-   融合「[easy_en](https://github.com/BlindingDark/rime-easy-en)」英文输入方案
    -   使用了「[融合拼音](https://github.com/tumuyan/rime-pinyin-simp)」的词库和拼写规则
-   纯简体字表、词库（这样在用户词典中也是简体了）
    -   字表：[《通用规范汉字表》的 8105 字字表](https://github.com/iDvel/The-Table-of-General-Standard-Chinese-Characters)
    -   词库：「[雾凇拼音 | 长期维护的简体词库](https://github.com/iDvel/rime-ice)」 + 「[搜狗细胞词库](https://github.com/lewangdev/scel2txt)」
-   皮肤 「[默认皮肤](https://github.com/iDvel/rime-ice/blob/main/squirrel.yaml)」 + 「[微信键盘皮肤](https://gist.github.com/zsakvo/fff6e4859265d5d629439d5ccb553f8a)」
-   长期持续修订遇到的异形词、错别字、错误注音

<br>

**部署前请先将 `pinyin_simp.extended.dict.yaml` 中的 `- cn_dicts/privacy` 这行删除，这是我自己的私人隐私词库，否则部署时会报错。**

<br>

## 删除错词

将光标（`↑` `↓`或`←` `→`）移到要删除的词组上，按 `Shift+Fn+Delete` 键（第三方键盘按 `Control+Delete`）。只能从用户词典中删除词组，词库里词组只会取消其调频顺序。

<br>

## 不同设备间通过 iCloud 同步

1. 配置文件里打开 `installation.yaml`，将 `installation_id` 后的名称改为 Mac（支持自定义）
2. 复制下面路径代码粘贴进去，将 `admin` 替换为 Mac 管理员名称（代码里 `RimeSync` 是同步后文件夹名称，支持自定义）
```
sync_dir: "/Users/admin/Library/Mobile Documents/com~apple~CloudDocs/RimeSync"
```
3. 点击菜单栏【ㄓ】-【同步用户数据】

<br>

## 仓 | Hamster 输入法配置

-   [仓 | Hamster](https://github.com/imfuxiao/Hamster) 2.3.0 适用于 iOS 系统
-   和鼠须管同方案，使用 `hamster.yaml` 替换 `default.custom.yaml` 为通用配置
    -   内含「[微信键盘皮肤](https://gist.github.com/laloe74/c0c2b481abb7f0f272a1b0c86cf67dc0)」+「古罗配列26键及9键」
-   使用方法同鼠须管
    -   在仓输入法里开启 iCloud 同步，将本项目所有文件拷贝至 `iCloud/Hamster/Rime/` 目录下
    -   仓输入法-RIME-重新部署，既可
    -   支持高度自定义 「[通用教程1](https://ihsiao.com/apps/hamster/docs/)」 + 「[通用教程2](https://github.com/imfuxiao/Hamster/wiki)」
    -   可以通过这个 「[在线自定义工具](https://lost-melody.github.io/hamster-tools/)」 导入配置文件 `hamster.yaml` 后，自定义修改皮肤、按键等

<br>

## 参考

[maomiui](https://github.com/maomiui)/**[rime](https://github.com/maomiui/rime)** 详细的图文教程及实例

[twlz0ne](https://github.com/twlz0ne)/**[rime-settings](https://github.com/twlz0ne/rime-settings)** 基本配置

[pengcu](https://github.com/pengcu)/**[rime-settings](https://github.com/pengcu/rime-settings)** 基本配置

[Rime配置教程：雾凇拼音 博客版](https://dvel.me/posts/rime-ice/)

[Rime方案製作詳解](https://rime-aca.tumblr.com/post/67241713724/rime方案製作詳解)