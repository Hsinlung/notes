
> Nginx 
>> `安装 Nginx 之前必须先安装它所依赖的环境`
>>
>> `yum install -y gcc gcc-c++ pcre pcre-devel zlib zlib-devel openssl-devel`
>> 
>> `指定 nginx 的安装路径 ./configure --prefix=/usr/local/nginx/`
>>  
>> `编译并安装 make && make install`
  + 基于C语言开发
  + HTTP模块使用pcre来解析正则表达式
  + 可以使用zlib对HTTP包的内容进行gzip 压缩
  + 不仅支持HTTP协议,还支持HTTPS
  + HTTPS需要openssl提供支持
---

| 功能 | 说明 |
| :----:| :----: |
| 正向代理（forward proxy） | 代理服务器代理了客户端，去和目标服务器进行交互 |
| 反向代理（Reverse Proxy） | 代理服务器代理了目标服务器，去和客户端进行交互 |
| 负载均衡（Load Balance） | 多台服务器以对称的方式组成一个服务器集群 |

---
* 启动

    > `sbin/nginx`

* 重启

   > `sbin/nginx -s reload`

* 停止
    > `sbin/nginx -s quit`
