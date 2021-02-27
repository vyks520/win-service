# win-service
基于aardio语言的Windows服务管理程序，赋予不支持安装为系统服务的程序（如nginx、node.js、批处理等）创建Windows Service，无任何环境依赖，配置简单。欢迎大家指导。

基于aardio官方范例改造。

## 使用说明

### nginx服务安装示例

下载服务管理主程序`win-service.exe`及配置文件`service.json`并复制到nginx安装目录下。

`service.json`配置文件数据：

```json
    {
      "name": "nginx",
      "display_name": "Nginx Service",
      "description": "Nginx Service",
      "executable": "nginx.exe",
      "executable_args": "",
      "stop_args":"-s stop"
    }
```

确认配置没问题后打开`win-service.exe`管理程序按照提示操作即可。

![]()

