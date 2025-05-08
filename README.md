curl -fsSL https://qubes.3isec.org/repo/3isec.asc | gpg --dearmor | sudo tee /usr/share/keyrings/qubes-archive-keyring.gpg > /dev/null

echo "deb [arch=amd64 signed-by=/usr/share/keyrings/qubes-archive-keyring.gpg] https://qubes.3isec.org/repo/ubuntu plucky main" | sudo tee /etc/apt/sources.list.d/qubes.list > /dev/null
