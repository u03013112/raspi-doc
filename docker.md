## Docker 安装
`curl -sSL https://get.docker.com| sh`

默认情况下执行docker命令是需要root权限的，也就是要用sudo docker 来运行。

一下方法可以免去sudo执行，重启生效：

sudo usermod -aG docker pi && sudo reboot

## Docker Compose 安装
`sudo apt-get update`
`sudo apt-get install -y python python-pip`
`sudo pip install docker-compose`