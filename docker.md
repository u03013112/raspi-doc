## Docker 安装
`curl -sSL https://get.docker.com| sh`

默认情况下执行docker命令是需要root权限的，也就是要用sudo docker 来运行。

一下方法可以免去sudo执行，重启生效：

sudo usermod -aG docker pi && sudo reboot

## Docker Compose 安装
`apt-get update`
`apt-get install -y libffi-dev libssl-dev`
`apt install -y python3-dev python3 python3-pip`
`pip3 install docker-compose -i http://mirrors.aliyun.com/pypi/simple/ --trusted-host mirrors.aliyun.com`