#前期准备工作
从 [NGINX机构官网http://nginx.org/en/download.html](http://nginx.org/en/download.html) 下载 NGINX 最新版，仓库中只包含了win版
从nginx文件夹中复制html文件夹到项目根目录，公用nginx静态资源。
#1.Window下Nginx部署
在win版的NGINX中找到cong/nginx.conf，修改http.server['location /'].root，修改为../html
win下直接运行nginx.exe
#2.Ubuntu下部署
ubuntu直接在root用户下
>`apt install nginx`
如果需要开机启动继续执行`systemctl enable nginx`
#3.Mac下部署
mac下下载NGINX最新版源文件，解压后进入到nginx-xxx文件夹
>`sudo ./configure `
>`sudo make`
>`sudo make install`
安装完毕后，进行nginx
>`sudo  /usr/local/nginx/sbin/nginx `
