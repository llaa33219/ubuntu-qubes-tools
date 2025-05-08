# XFCE 환경 설치
sudo apt update
sudo apt install -y xfce4 xfce4-terminal xfce4-notifyd network-manager-gnome

# 심리스 모드 지원 폴더 생성
sudo mkdir -p /etc/qubes-rpc

# 필요한 스크립트 생성
sudo bash -c 'echo "#!/bin/bash" > /etc/qubes-rpc/qubes.WindowIconUpdater'
sudo bash -c 'echo "true" >> /etc/qubes-rpc/qubes.WindowIconUpdater'
sudo chmod +x /etc/qubes-rpc/qubes.WindowIconUpdater
