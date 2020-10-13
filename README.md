# CICD_M，别名"小公司一把梭"
docker-compose一键部署gitlab +sonarqube + mysql + jenkins + ansible + maven + jdk1.8  
添加gitlab的http强制跳转https访问功能

### 前提条件：
先在hosts文件中添加IP和域名的映射关系，例如我在192.168.5.186上部署
#### example:
192.168.5.186 harbor.aecg.com.cn
# 启动 
docker-compose up -d

# gitlab访问方式
http://harbor.aecg.com.cn
初始账号root,登录时密码会让你自己修改


# jenkins访问方式
http://192.168.5.186:8080



# sonarqube访问方式
http://192.168.5.186:9000  
账号: admin   
密码: admin  



# mysql访问方式
mysql -u root -p -h 192.168.5.186 -P 3308  
密码:  example

## 注意:  
1.可以在宿主机安装nginx反向代理gitlab,可以获取到客户端的真实IP地址，方便查看日志  
2.在阿里云申请对应的域名证书，替换上述docker-compose.yaml文件中关于ssl,即harbor.aecg.com.cn证书相关配置即可使用
