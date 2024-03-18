## 基本套路：

-   Squirrel 0.16.2 简中全拼
-   「袖珍简化字方案」 [rime](https://github.com/rime)/**[rime-pinyin-simp](https://github.com/rime/rime-pinyin-simp)**
-   《通用规范汉语表》8105 字表   [iDvel](https://github.com/iDvel)/**[The-Table-of-General-Standard-Chinese-Characters](https://github.com/iDvel/The-Table-of-General-Standard-Chinese-Characters)**  
-   「雾凇拼音」词库 [iDvel](https://github.com/iDvel)/**[rime-ice](https://github.com/iDvel/rime-ice/tree/main)**
-   英文输入方案 Easy English Nano（支持大写字母） [tumuyan](https://github.com/tumuyan)/**[rime-pinyin-simp](https://github.com/tumuyan/rime-pinyin-simp)**  
-   简繁切换 [rime/home/issues#388](https://github.com/rime/home/issues/388#issuecomment-504572224) 
-   动态日期、时间、星期 [KyleBing](https://github.com/KyleBing)/**[rime-wubi86-jidian](https://github.com/KyleBing/rime-wubi86-jidian)**
-   所有标点符号直接上屏，「/」模式改为「v」模式，「/」直接上屏
-   没有 emoji，如需要可参考 [maomiui](https://github.com/maomiui)/**[rime](https://github.com/maomiui/rime)** 、[fkxxyz](https://github.com/fkxxyz)/**[rime-cloverpinyin](https://github.com/fkxxyz/rime-cloverpinyin)** 等
-   微信键盘皮肤 [zsakvo](https://gist.github.com/zsakvo)/**[squirrel-custom.yaml](https://gist.github.com/zsakvo/fff6e4859265d5d629439d5ccb553f8a)**

<br>

## 同步至 iCloud

1. 配置文件里打开 installation.yaml，将 id 改为 Mac（支持自定义）。
2. 复制下面路径代码粘贴进去，将 admin 替换为 Mac 管理员名称（代码里 RimeSync 是同步后文件夹名称，支持自定义）。
```
sync_dir: "/Users/admin/Library/Mobile Documents/com~apple~CloudDocs/RimeSync"
```
3. 点击菜单栏【ㄓ】-【同步用户数据】

<br>

## 参考

[maomiui](https://github.com/maomiui)/**[rime](https://github.com/maomiui/rime)** 详细的图文教程及实例

[twlz0ne](https://github.com/twlz0ne)/**[rime-settings](https://github.com/twlz0ne/rime-settings)** 基本配置

[lewangdev](https://github.com/lewangdev)/**[scel2txt](https://github.com/lewangdev/scel2txt)** 搜狗细胞词库转鼠须管（Rime）词库

[Rime方案製作詳解](https://rime-aca.tumblr.com/post/67241713724/rime方案製作詳解)