# 自用 Rime 配置

<br>

## 同步至 iCloud

1. 配置文件里打开 installation.yaml，将 id 改为 Mac（支持自定义）。
2. 复制下面路径代码粘贴进去，将 admin 替换为 Mac 管理员名称（代码里 RimeSync 是同步后文件夹名称，支持自定义）。
```
sync_dir: "/Users/admin/Library/Mobile Documents/com~apple~CloudDocs/RimeSync"
```
3. 点击菜单栏【ㄓ】-【同步用户数据】，等待几秒提示同步成功。打开访达 iCloud 找到名为 RimeSync 的文件即是。

<br>

## 感谢：上手时参考过的主要仓库和博客

[maomiui](https://github.com/maomiui)/**[rime](https://github.com/maomiui/rime)** 详细的图文教程及实例
[twlz0ne](https://github.com/twlz0ne)/**[rime-settings](https://github.com/twlz0ne/rime-settings)** 基本配置
[iDvel](https://github.com/iDvel)/**[雾凇拼音 | 长期维护的简体词库](https://github.com/iDvel/rime-ice)** 词库
[lewangdev](https://github.com/lewangdev)/**[scel2txt](https://github.com/lewangdev/scel2txt)** 搜狗细胞词库转鼠须管（Rime）词库
[Rime方案製作詳解](https://rime-aca.tumblr.com/post/67241713724/rime方案製作詳解)