sudo tee /etc/apt/sources.list.d/qubes-r4.list << EOF
deb [arch=amd64] https://deb.qubes-os.org/r4.2/vm/pool/vm/main focal main
EOF

sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 0x36879494
sudo apt update
