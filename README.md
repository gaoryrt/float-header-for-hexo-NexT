# Float Header for Hexo NexT Mist theme
在 NexT-Mist主题 的基础上做的一点点改动  
把顶栏改成一直停靠在窗口上沿了 
# 预览 preview
***
![before](http://ww3.sinaimg.cn/large/a243ad6cjw1exaa8z4itgj20se0qztay.jpg)  
*origin NexT Mist*
***
[click to see](http://gaoryrt.github.io)
*After*
***
# 安装 install
```
cd YourPath/hexo/themes/next/source/css/_schemes
git clone https://github.com/gaoryrt/float_header_for_hexo_NexT.git
```
  

Rename` Mist` folder to ` Mist_without_float_haeder`  
Rename`float_header_for_hexo_NexT` to ` Mist`  
Done.  
# 已知的问题 problems
~~1. `menu`栏在某段固定浏览器宽度（tablet）下不能做到上下对齐。原因未知。~~原来还有`desktop-large`这个大小  
2. `site-nav site-nav-on`栏（mobile 时展开的 menu 栏）失去了原有的延展特性，变为了遮盖下方内容。原因未知。  
~~3. `site-nav site-nav-on`栏（mobile 时展开的 menu 栏）没有背景颜色。暂时不解决，见#2。~~改好了  

***
# 贴一下我自己的custom.styl文件
强烈推荐修改这个`custom.styl`文件，别问为什么。  
位置： `next/source/css/_variables/custom.styl`  
```
$content-desktop = 600px  // 修改成你期望的宽度
$content-desktop-large = 600px // 当视窗超过 1600px 后的宽度

$font-family-sans-serif   = "PingFang", Verdana, sans-serif
$font-family-serif        = "PingFang", Verdana, sans-serif
$font-family-monospace    = "PingFang", Verdana, sans-serif
$font-family-chinese      = "PingFang", Verdana, sans-serif
$font-family-base         = "PingFang", Verdana, sans-serif
$font-family-headings     = "Cambria Bold", cambria, Verdana, sans-serif
$font-family-posts        = $font-family-base

$code-font-family = "Input Mono", "PT Mono", Consolas, Monaco, Menlo, monospace // 代码字体
$font-size-base = 16px;
$font-size-large = 16px;
$font-size-small = 13px;
```