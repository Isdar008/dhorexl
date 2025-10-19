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
bash -c 'echo -e "[Resolve]\nDNS=8.8.8.8" > /etc/systemd/resolved.conf && systemctl enable systemd-resolved'
```
