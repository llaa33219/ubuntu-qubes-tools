# 저장소 디렉토리 생성
sudo mkdir -p /etc/apt/keyrings

# 키 다운로드 및 저장
curl -fsSL https://keys.gnupg.net/pks/lookup?op=get&search=0x36879494 | sudo gpg --dearmor -o /etc/apt/keyrings/qubes-os-archive-keyring.gpg

# 저장소 추가
sudo sh -c 'echo "deb [arch=amd64 signed-by=/etc/apt/keyrings/qubes-os-archive-keyring.gpg] https://deb.qubes-os.org/r4.2/vm noble main" > /etc/apt/sources.list.d/qubes-r4.2.list'

# 업데이트
sudo apt update
