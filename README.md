### Typecho-QiniuFile
---

Qiniu File 是一款 Typecho 的七牛云存储插件，可将 Typecho 的文件功能接入到七牛云存储中，包括上传附件、修改附件，以及获取文件在七牛的绝对网址。

原修改版作者：[https://github.com/licxisky/typecho-Plugin-QiniuFile](https://github.com/licxisky/typecho-Plugin-QiniuFile)

#### 使用方法：
- 第一步：下载本插件，放在 `usr/plugins/` 目录中，改名为 QiniuFile；
- 第二步：激活插件；
- 第三步：填写空间名称、Access Key、Secret Key、域名 等配置；
- 第四步：完成。

#### 与原版本的不同之处：

在有关处增加代码  
`$upload_filename = date("Ymdhis") . '.' . $part[1];`  
来自动更改文件名为当前时间格式，防止文件名冲突。  
  
格式：年+月+日+时+分+秒.文件后缀，时间均为首个数字含0