#前期准备工作
>从 [NGINX机构官网http://nginx.org/en/download.html](http://nginx.org/en/download.html) 下载 NGINX 最新版，版本中同时包含了mac以及win版，分别命名，方便不同系统下使用git进行同步编辑
>从nginx文件夹中复制html文件夹到项目根目录，用于公用mac、win版的nginx静态资源。
>在mac、win版的NGINX中找到cong/nginx.conf，修改http.server['location /'].root，修改为../html
>win下直接运行nginx.exe
>mac下执行：
>>$ ./configure
>>$ sudo make
>>启动nginx:
>> $ sudo  /nginx