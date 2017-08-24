# 代码积累
林小志的css
---
/*===== 清除默认的margin的属性值 =====*/
body,
blockquote,
dd,
dl,
figure,
form,
p,
pre,
h1,
h2,
h3,
h4,
h5,
h6 {margin:0;}

/*===== 统一设置列表的margin和padding，以及列表表形式 =====*/
menu,
ul,
ol {list-style:none;margin:0;padding:0;}

/*===== 全局定义字体以及页面背景 =====*/
body {line-height:1.5;background-color:#FFFFFF;}
body,h1,h2,h3,h4,h5,h6,input,button,select,textarea {font-size: 18px;} /* 设置字体大小 */
input[type="button"],
input[type="submit"],
input[type="reset"] {font-size: 16px;} /* 设置字体大小，这部分跟前面写在一起，IE6中会无效 */

/*===== 字体控制 =====*/
body,
input,
button,
select,
optgroup,
option,
textarea,
pre {font-family: Arial, Roboto, 'Droid Sans', 'Hiragino Sans GB', 'Microsoft YaHei', 'Simsun', STXihei, 'sans-serif';}

/*===== 设置iframe的背景色以及去除个别浏览器iframe底部的几个像素 =====*/
iframe {background-color:#FFFFFF;vertical-align:middle;}

/*===== 设置文本链接样式 =====*/
a {color:#000000;}
a:hover {text-decoration:underline;color:#FF0000;}

/*===== 去除个别浏览器图片底部的几个像素，以及设置图片形式链接无边框 =====*/
img {vertical-align:middle;}
a img {border:0 none;}

/*===== 设置表单元素的样式 =====*/
fieldset {margin:0;padding:0;}
legend {color:windowtext;} /* 设置表单域部分的字体颜色为系统窗体文本颜色 */
button,
input.ie6 {overflow:visible;padding:.1em .25em;cursor:pointer;} /* 尽量统一按钮的大小，鉴于IE6不支持【属性选择符】，所以使用一个类名来控制 */
input[type="button"],
input[type="submit"],
input[type="reset"] {overflow:visible;padding:.1em .25em;cursor:pointer;} /* 尽量同意按钮的大小，如果采用input方式做的按钮 */
input[type="text"],
select,
textarea {background-color:#FFFFFF;} /* 统一文本输入框、下拉、文本框的背景色，避免被用户设置系统颜色而破坏页面色彩 */
select {border:1px inset;} /* 统一下拉的边框 */
textarea {overflow:auto;vertical-align:text-bottom;*vertical-align:auto;border:1px solid;resize:vertical;} /* 滚动条为auto，与周边的元素对齐方式，其中hack部分是IE6&7中vertical-align影响范围清除，resize为上下可拉动，避免左右拉动破坏页面布局，如有需要可以设置为none */

/*===== 设置表格元素的样式 =====*/
table {border-spacing:0;} /* 合并表格的间隙，去掉单元格之间的间距，如有需要合并单元格为细线表格，可增加 border-collapse:collapse; */
td, th, caption {padding:0;} /* 去除单元格以及caption表头的padding值 */

转载地址：http://linxz.github.io/tianyizone/css_reset.html
