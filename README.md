# nginx--install-shell
CentOS 一键安装 Nginx

### 环境要求
* CentOS 6/7

### 当前版本
* nginx/1.14.2

#### 已编译模块
* --with-stream
* --with-http_stub_status_module
* --with-http_v2_module
* --with-http_ssl_module
* --with-http_gzip_static_module
* --with-http_realip_module
* --with-pcre-jit
* pcre-8.39
* zlib-1.2.11
* openssl-1.1.1
* ngx_http_substitutions_filter_module
* ngx_cache_purge
* ngx_brotli
* headers-more-nginx-module

### 安装
```
wget https://raw.githubusercontent.com/tianfanfan/nginx--install-shell/master/nginx.sh && bash nginx.sh
```

* 如果是 CentOS 6 的系统，请选择编译安装。
* CentOS 7 可选择编译安装或二进制安装。
* 编译安装通常 10 分钟左右，常用模块齐全。
* 二进制安装通常 2 分钟左右，模块较少，但是日常使用也绝对够了。

### 常用命令
安装完成后执行命令 `source /etc/profile` 让环境变量立即生效，或重新打开终端。
* 启动nginx：`nginx`
* 停止nginx：`nginx -s stop`
* 重载nginx：`nginx -s reload`
* 语法检测：`nginx -t`

### 联系我