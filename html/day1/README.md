# 前期准备工作
从 [NGINX机构官网http://nginx.org/en/download.html](http://nginx.org/en/download.html) 下载 NGINX 最新版，仓库中只包含了win版
从nginx文件夹中复制html文件夹到项目根目录，公用nginx静态资源。
# 一.Window下Nginx安装与运行
在仓库中的win版NGINX中找到cong/nginx.conf，修改http.server['location /'].root，修改为../html
win下直接运行nginx.exe
# 二-1.Ubuntu下安装
ubuntu直接在root用户下
`apt install nginx`
如果需要开机启动继续执行`systemctl enable nginx`
# 二-2.Mac下安装
mac下下载NGINX最新版源文件，解压后进入到nginx-xxx文件夹
```
    sudo ./configure 
    sudo make
    sudo make install
```
# 三.Linux系系统运行
假设本地仓库的路径是/usr/home/FrontLearn
那么win版配置文件在是/usr/home/FrontLearn/nginx-1.17.3-win/conf/nginx.conf
安装完毕后，进行nginx
`sudo  /usr/local/nginx/sbin/nginx -c /usr/home/FrontLearn/nginx-1.17.3-win/conf/nginx.conf`
