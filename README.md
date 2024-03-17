# 自用 Rime 配置


## 基本套路：

-   Squirrel 0.15.2 简中全拼
-   「袖珍简化字方案」 [rime](https://github.com/rime)/**[rime-pinyin-simp](https://github.com/rime/rime-pinyin-simp)**  配合简体字表和词库，这样在 `*.userdb.txt` 中的也是简体的了
-   《通用规范汉语表》8105 字表   [iDvel](https://github.com/iDvel)/**[The-Table-of-General-Standard-Chinese-Characters](https://github.com/iDvel/The-Table-of-General-Standard-Chinese-Characters)**  
-   华宇野风系统词库 [华宇拼音输入法论坛 - 华语野风系统词库](http://bbs.pinyin.thunisoft.com/forum.php?mod=viewthread&tid=30049)
-   英文输入方案 Easy English Nano（支持大写字母） [tumuyan](https://github.com/tumuyan)/**[rime-pinyin-simp](https://github.com/tumuyan/rime-pinyin-simp)**  
-   简繁切换 [rime/home/issues#388](https://github.com/rime/home/issues/388#issuecomment-504572224) 
-   动态日期、时间、星期 [KyleBing](https://github.com/KyleBing)/**[rime-wubi86-jidian](https://github.com/KyleBing/rime-wubi86-jidian)**
-   所有标点符号直接上屏，「/」模式改为「v」模式，「/」直接上屏
-   没有 emoji，如需要可参考 [maomiui](https://github.com/maomiui)/**[rime](https://github.com/maomiui/rime)** 、[fkxxyz](https://github.com/fkxxyz)/**[rime-cloverpinyin](https://github.com/fkxxyz/rime-cloverpinyin)** 等
-   增加了许多全拼纠错（手速太快经常按错 😅）
-   参考谷歌、《现代汉语规范词典》、[异形词整理表](https://wucuozi.com/cuobiezi/yixingzi/)、[错别字辨析](https://wucuozi.com/bian/ ) 修正了大量的异形词、错别字

<br>

## 精简字表

袖珍简化方案原版字表 17K+ 的字，而《通用规范汉字表》才只收录了 8105 个字。

如果不是需要大字库的文字相关工作者，推荐使用精简后的字表。

使用了自己整理的完全正确注音的字表并加上了四叶草方案的字频。

<br>

## 系统词库

同样的，原方案词库中有大量的异形词和错别字，找到了“华语野风系统词库”，感谢原作者的辛苦整理，几乎已经修正了所有的异形词和错别字。

<br>

## 感谢：上手时参考过的主要仓库和博客

[maomiui](https://github.com/maomiui)/**[rime](https://github.com/maomiui/rime)** 详细的图文教程及实例

[fkxxyz](https://github.com/fkxxyz)/**[rime-cloverpinyin](https://github.com/fkxxyz/rime-cloverpinyin)** 四叶草拼音输入方案

[placeless](https://github.com/placeless)/**[squirrel_config](https://github.com/placeless/squirrel_config)**  [鼠须管配置 2021](https://placeless.net/blog/rime-squirrel-customization-2021) 见过的最酷炫的只有两个候选项的小鹤双形 

[Rime方案製作詳解](https://rime-aca.tumblr.com/post/67241713724/rime方案製作詳解)

<br>

## 其他

在  `custom_phrase.txt` 中可以设置某些字词永远只出现在前 N 个候选项，但是这样设置之后，这些字词就不能与正常的字共同造词（自造词无法被记住）。现在不知道如何能完美的固定某些字词的候选项顺序。  

<br>

顺便推荐一下在 VSCode 中给 YAML 设置默认 Tab 行为的方法：https://github.com/microsoft/vscode/issues/69011

使 Tab 变成 2 个空格长度的 Tab（而不是空格），修改词库时很方便，不用总是手动调节了。

建议配置都折腾完了再启用这个，因为配置文件中如果使用了 Tab 来缩进会产生一些意想不到的错误。。。

`.../.vscode/settings.json`：

```json
    // Configure editor settings to be overridden for [yaml] language.
    "[yaml]": {
        "editor.insertSpaces": false,
        "editor.tabSize": 2,
        "editor.autoIndent": false,
    },
```

