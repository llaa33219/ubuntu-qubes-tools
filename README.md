sudo apt update
sudo apt install xfce4 xfce4-terminal xfce4-notifyd

sudo mkdir -p /etc/qubes-rpc
sudo bash -c 'echo "#!/bin/bash" > /etc/qubes-rpc/qubes.WindowIconUpdater'
sudo bash -c 'echo "true" >> /etc/qubes-rpc/qubes.WindowIconUpdater'
sudo chmod +x /etc/qubes-rpc/qubes.WindowIconUpdater

systemctl status qubes-gui-agent
