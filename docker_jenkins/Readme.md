#### 打包方式:  
docker build -t docker_jenkins .
#### 启动方式:  
docker run -dti --privileged=true  --cap-add SYS_ADMIN -v /sys/fs/cgroup:/sys/fs/cgroup:ro -p 8080:8080 --name docker_jenkins docker_jenkins
#### 快捷启动方式:
docker run -dit  --privileged=true  --cap-add SYS_ADMIN -p 8080:8080 --name jenkins registry.cn-hangzhou.aliyuncs.com/houzigang/jenkins_pod
