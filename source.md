# 换源
mv /etc/apt/sources.list /etc/apt/sources.list.bak
echo "deb http://mirrors.aliyun.com/raspbian/raspbian/ wheezy main non-free contrib" > /etc/apt/sources.list
echo "deb-src http://mirrors.aliyun.com/raspbian/raspbian/ wheezy main non-free contrib" >> /etc/apt/sources.list

# 更新
apt-get update
apt-get upgrade