# 关闭省电模式
sudo iw dev wlan0 set power_save off

# wpa_supplicant.conf
country=CN
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1
 
network={
    ssid="NB1201-5G"
    psk="19850421"
    priority=100
}

network={
    ssid="A131wings.S5G"
    psk="123456a131"
    priority=1
}

network={
    ssid="jing5G"
    psk="123456a121"
    priority=10
}