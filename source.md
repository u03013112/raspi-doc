# 换源
mv /etc/apt/sources.list /etc/apt/sources.list.bak
echo "deb http://mirrors.aliyun.com/raspbian/raspbian/ buster main contrib non-free rpi" > /etc/apt/sources.list
echo "deb-src http://mirrors.aliyun.com/raspbian/raspbian/ buster main contrib non-free rpi" >> /etc/apt/sources.list

cp /etc/apt/sources.list.d/raspi.list /etc/apt/sources.list.d/raspi.list.bak
echo "deb http://mirrors.aliyun.com/raspbian/raspbian/ buster main" > /etc/apt/sources.list.d/raspi.list
echo "deb-src http://mirrors.aliyun.com/raspbian/raspbian/ buster main" >> /etc/apt/sources.list.d/raspi.list

# 更新
apt-get update
apt-get upgrade