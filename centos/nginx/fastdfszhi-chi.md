#### Fastdfs支持

cd /app/soft/nginx/conf

./configure --prefix=/app/soft/nginx --add-module=/app/fastdfs-nginx-module-master/src

make & make install

#### 缩略图image\_filter

[http://blog.csdn.net/clevercode/article/details/52278482](http://blog.csdn.net/clevercode/article/details/52278482)

./configure --prefix=/app/soft/nginx --add-module=/app/fastdfs-nginx-module-master/src  --with-http\_image\_filter\_module

#### 缓存模块

./configure --prefix=/app/soft/nginx --add-module=/app/ngx\_cache\_purge-2.3



#### 开放端口

firewall-cmd --add-port=22122/tcp --permanent

firewall-cmd --add-port=23000/tcp --permanent

firewall-cmd --add-port=80/tcp --permanent

