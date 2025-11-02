# Installer
```
sysctl -w net.ipv6.conf.all.disable_ipv6=1
sysctl -w net.ipv6.conf.default.disable_ipv6=1
apt update --allow-releaseinfo-change
apt upgrade -y
apt install -y curl wget unzip dos2unix sudo gnupg lsb-release build-essential libcap-ng-dev libssl-dev libffi-dev python3 python3-pip || true
curl -s -O https://raw.githubusercontent.com/Isdar008/dhorexl/main/gerhana
chmod +x gerhana
./gerhana
```
# DNS
```
echo "nameserver 1.1.1.1" > /etc/resolv.conf
```
# MESG for deb13
```
sed -i '/mesg n/d' ~/.bashrc ~/.profile 2>/dev/null
```
