# WireGuard 服务器一键安装脚本



然后执行一键安装命令：

yum install wget -y -q ; wget -q -O wgs https://raw.githubusercontent.com/chinashiyu/wireguard/master/wg.txt ; sh wgs


安装完成后，下载安装客户端，并导入配置文件：

Windows 客户端下载：

https://download.wireguard.com/windows-client/wireguard-amd64-0.1.0.msi

MacOS 客户端下载：

https://itunes.apple.com/us/app/wireguard/id1451685025?ls=1&mt=12

安卓 客户端下载：

https://play.google.com/store/apps/details?id=com.wireguard.android



hello world:

52:  
wget -q -O wgs.sh https://raw.githubusercontent.com/chinashiyu/wireguard/master/wg.txt  
sed -i "s/10.10.20/10.10.52/g" \`grep 10.10.20 -rl ./wgs.sh\`  
chmod +x wgs.sh  
./wgs.sh  
service firewalld start  





53:
wget -q -O wgs.sh https://raw.githubusercontent.com/chinashiyu/wireguard/master/wg.txt  
sed -i "s/10.10.20/10.10.53/g" \`grep 10.10.20 -rl ./wgs.sh\`  
chmod +x wgs.sh  
./wgs.sh  
service firewalld start  



54:
wget -q -O wgs.sh https://raw.githubusercontent.com/chinashiyu/wireguard/master/wg.txt  
sed -i "s/10.10.20/10.10.54/g" \`grep 10.10.20 -rl ./wgs.sh\`  
chmod +x wgs.sh  
./wgs.sh  
service firewalld start  
