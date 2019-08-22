打包方式:docker build -t docker_jenkins .
启动方式:docker run -dti --privileged=true -v /sys/fs/cgroup:/sys/fs/cgroup:ro -p 8098:8098 --name docker_jenkins docker_jenkins
