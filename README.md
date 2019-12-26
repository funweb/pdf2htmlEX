pdf2htmlEX is no longer under active development. New maintainers are [wanted](http://pdf2htmlex.blogspot.ch/2016/12/looking-for-new-maintainer.html).

#![](http://coolwanglu.github.io/pdf2htmlEX/images/pdf2htmlEX-64x64.png) pdf2htmlEX 

<!--
[![Build Status](https://travis-ci.org/coolwanglu/pdf2htmlEX.png?branch=master)](https://travis-ci.org/coolwanglu/pdf2htmlEX)
-->
>一图胜千言<br>A beautiful demo is worth a thousand words

- **Bible de Genève, 1564** (fonts and typography): [HTML](http://coolwanglu.github.com/pdf2htmlEX/demo/geneve.html) / [PDF](https://github.com/raphink/geneve_1564/releases/download/2015-07-08_01/geneve_1564.pdf)
- **Cheat Sheet** (math formulas): [HTML](http://coolwanglu.github.com/pdf2htmlEX/demo/cheat.html) / [PDF](http://www.tug.org/texshowcase/cheat.pdf)
- **Scientific Paper** (text and figures): [HTML](http://coolwanglu.github.com/pdf2htmlEX/demo/demo.html) / [PDF](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.148.349&rep=rep1&type=pdf)
- **Full Circle Magazine** (read while downloading): [HTML](http://coolwanglu.github.com/pdf2htmlEX/demo/issue65_en.html) / [PDF](http://dl.fullcirclemagazine.org/issue65_en.pdf)
- **Git Manual** (CJK support): [HTML](http://coolwanglu.github.com/pdf2htmlEX/demo/chn.html) / [PDF](http://files.cnblogs.com/phphuaibei/git%E6%90%AD%E5%BB%BA.pdf)

pdf2htmlEX renders PDF files in HTML, utilizing modern Web technologies.
Academic papers with lots of formulas and figures? Magazines with complicated layouts? No problem!

pdf2htmlEX is also an [online publishing tool](http://coolwanglu.github.io/pdf2htmlEX/doc/tb108wang.html) which is flexible for many different use cases. 

Learn more about [who](https://github.com/coolwanglu/pdf2htmlEX/wiki/Use-Cases) and [why](https://github.com/coolwanglu/pdf2htmlEX/wiki/Introduction) should use pdf2htmlEX.

### Features

* Native HTML text with precise font and location.
* Flexible output: all-in-one HTML or on demand page loading (needs JavaScript).
* Moderate file size, sometimes even smaller than PDF.
* Supporting links, outlines (bookmarks), printing, SVG background, Type 3 fonts and [more...](https://github.com/coolwanglu/pdf2htmlEX/wiki/Feature-List)

[Compare to others](https://github.com/coolwanglu/pdf2htmlEX/wiki/Comparison)

### Portals

 * [:house:Wiki Home](https://github.com/coolwanglu/pdf2htmlEX/wiki)
 * [Download](https://github.com/coolwanglu/pdf2htmlEX/wiki/Download) & [Building](https://github.com/coolwanglu/pdf2htmlEX/wiki/Building)
 * [Quick Start](https://github.com/coolwanglu/pdf2htmlEX/wiki/Quick-Start)
 * [Report Issues / Ask for Help](https://github.com/coolwanglu/pdf2htmlEX/blob/master/CONTRIBUTING.md#guidance)
 * [:question:FAQ](https://github.com/coolwanglu/pdf2htmlEX/wiki/FAQ)
 * [:envelope:Mailing List](https://groups.google.com/forum/#!forum/pdf2htmlex)
 * [:mahjong:中文邮件列表](https://groups.google.com/forum/#!forum/pdf2htmlex-cn)

### LICENSE

pdf2htmlEX, as a whole package, is licensed under GPLv3+.
Some resource files are released with relaxed licenses, read `LICENSE` for more details.

### Acknowledgements

pdf2htmlEX is made possible thanks to the following projects:

* [poppler](http://poppler.freedesktop.org/)
* [Fontforge](http://fontforge.org/)

pdf2htmlEX is inspired by the following projects:

* pdftohtml from poppler 
* MuPDF
* PDF.js
* Crocodoc
* Google Doc

#### Special Thanks

* Hongliang Tian
* Wanmin Liu 






### Python3.x：pdf2htmlEX（解析pdf）安装和使用
#### 简介
pdf2htmlEX是一款优秀的pdf转换成html的工具；

#### 下载
windows下载地址：http://soft.rubypdf.com/software/pdf2htmlex-windows-version

#### 安装
下载pdf2htmlEX-win32-0.14.6-with-poppler-data.zip后，直接解压，即可用；

#### 测试
在dos窗口中切换到解压目录：



cd /d D:\pdf2htmlEX-win32-0.14.6
输入测试命令：

pdf2htmlex -v
结果如下图，表示安装成功；

#### pdf2html命令用法

--
用法: pdf2htmlEX [options] <input.pdf> [<output.html>]  
  -f,--first-page <int>         需要转换的起始页 (默认: 1)  
  -l,--last-page <int>          需要转换的最后一页 (默认: 2147483647)  
  --zoom <fp>                   缩放比例  
  --fit-width <fp>              适合宽度 <fp> 像素  
  --fit-height <fp>             适合高度 <fp> 像素  
  --use-cropbox <int>           使用剪切框 (default: 1)  
  --hdpi <fp>                   图像水平分辨率 (default: 144)  
  --vdpi <fp>                   图像垂直分辨率 (default: 144)  
  --embed <string>              指定哪些元素应该被嵌入到输出  
  --embed-css <int>             将CSS文件嵌入到输出中 (default: 1)  
  --embed-font <int>            将字体文件嵌入到输出中 (default: 1)  
  --embed-image <int>           将图片文件嵌入到输出中 (default: 1)  
  --embed-javascript <int>      将javascript文件嵌入到输出中 (default: 1)  
  --embed-outline <int>         将链接嵌入到输出中 (default: 1)  
  --split-pages <int>           将页面分割为单独的文件 (default: 0)  
  --dest-dir <string>           指定目标目录 (default: ".")  
  --css-filename <string>       生成的css文件的文件名 (default: "")  
  --page-filename <string>      分割的网页名称  (default:"")  
  --outline-filename <string>   生成的链接文件名称 (default:"")  
  --process-nontext <int>       渲染图行，文字除外 (default: 1)  
  --process-outline <int>       在html中显示链接 (default: 1)  
  --printing <int>              支持打印 (default: 1)  
  --fallback <int>              在备用模式下输出 (default: 0)  
  --embed-external-font <int>   嵌入局部匹配的外部字体 (default: 1)  
  --font-format <string>        嵌入的字体文件后缀 (ttf,otf,woff,svg) (default: "woff")  
  --decompose-ligature <int>    分解连字-> fi (default:0)  
  --auto-hint <int>             使用fontforge的autohint上的字体时不提示 (default: 0)  
  --external-hint-tool <string> 字体外部提示工具 (overrides --auto-hint) (default: "")  
  --stretch-narrow-glyph <int>  伸展狭窄的字形，而不是填充 (default: 0)  
  --squeeze-wide-glyph <int>    收缩较宽的字形，而不是截断 (default: 1)  
  --override-fstype <int>       clear the fstype bits in TTF/OTF fonts (default:0)  
  --process-type3 <int>         convert Type 3 fonts for web (experimental) (default: 0)  
  --heps <fp>                   合并文本的水平临界值，单位：像素(default: 1)  
  --veps <fp>                   vertical threshold for merging text, in pixels (default: 1)  
  --space-threshold <fp>        断字临界值 (临界值 * em) (default:0.125)  
  --font-size-multiplier <fp>   一个大于1的值增加渲染精度 (default: 4)  
  --space-as-offset <int>       把空格字符作为偏移量 (default: 0)  
  --tounicode <int>             如何处理ToUnicode的CMap (0=auto, 1=force,-1=ignore) (default: 0)  
  --optimize-text <int>         尽量减少用于文本的HTML元素的数目 (default: 0)  
  --bg-format <string>          指定背景图像格式 (default: "png")  
  -o,--owner-password <string>  所有者密码 (为了加密文件)  
  -u,--user-password <string>   用户密码 (为了加密文件)  
  --no-drm <int>                覆盖文档的 DRM 设置 (default: 0)  
  --clean-tmp <int>             转换后删除临时文件 (default: 1)  
  --data-dir <string>           指定的数据目录 (default: ".\share\pdf2htmlEX")  
  --debug <int>                 打印调试信息 (default: 0)  
  -v,--version                  打印版权和版本信息  
  -h,--help                     打印使用帮助信息
