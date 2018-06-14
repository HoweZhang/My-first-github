一个CSS的px值转rem值的Sublime Text 3自动完成插件。
---

安装<br>
* 下载本项目<br>
* 进入packages目录：Sublime Text -> Preferences -> Browse Packages...<br>
* 复制下载的cssrem目录到刚才的packges目录里。<br>
* 重启Sublime Text。<br>


配置参数
---
* 参数配置文件：Sublime Text -> Preferences -> Package Settings -> cssrem<br>

* px_to_rem - px转rem的单位比例，默认为40。<br>
* max_rem_fraction_length - px转rem的小数部分的最大长度。默认为6。<br>
* available_file_types - 启用此插件的文件类型。默认为：[".css", ".less", ".sass"]。<br>

```
{
"px_to_rem": 40, //px转rem的单位比例，默认为40
"max_rem_fraction_length": 6, //px转rem的小数部分的最大长度。默认为6。
"available_file_types": [".css", ".less", ".sass",".html"]
//启用此插件的文件类型。默认为：[".css", ".less", ".sass"]
}
```
