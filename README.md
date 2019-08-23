# CICD_M
docker-compose部署jenkins+sonarqube+mysql+ansible+jenkins+maven+jdk


### 前提条件：
先在hosts文件中添加IP和域名的映射关系，例如我在192.168.5.186上部署
example:
192.168.5.186 harbor.aecg.com.cn

# gitlab访问方式
http://harbor.aecg.com.cn
初始账号root,登录时密码会让你自己修改


# jenkins访问方式
http://192.168.5.186:8080



# sonarqube访问方式
http://192.168.5.186:9000


# mysql访问方式
mysql -u root -p -h 192.168.5.186 -P 3308
