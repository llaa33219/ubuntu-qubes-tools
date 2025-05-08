sudo sh -c 'echo "deb [arch=amd64] https://deb.qubes-os.org/r4.2/vm noble main" > /etc/apt/sources.list.d/qubes-r4.2.list'
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 0x36879494
sudo apt update
