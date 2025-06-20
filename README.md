# 更新软件源
apt-get 更新

# 安装 ash shell
apt-get install ash

# dd命令：

curl -sSL 'https://raw.githubusercontent.com/sdlw7757/dd/main/InstallNET.sh' | tr -d '\r' > install.sh
chmod +x install.sh
./install.sh -u 20.04 -v 64 -p 密码


命令中的 -d 后面为 Debian 版本号，-v 后面为 64 位 / 32 位，【7、8、9、10、10】
命令中的 -u 后面为 Ubuntu 版本号，-v 后面为 64 位/32 位，【14.04、16.04、18.04、20.04、22.04、24.04暂时】


ash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/MoeClub/Note/master/InstallNET.sh') -d 9 -v 64 -p 密码

例：bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/MoeClub/Note/master/InstallNET.sh') -d 9 -v 64 -p Sdlw53953


# 这个系统装BBR前先走这个命令

apt update -y && apt install -y curl && apt install -y socat && apt install wget -y

apt install -y git   ### 安装 git 环境

# 担心网站使用率不高被回收，可以配合保活脚本：

bash <(wget -qO- --no-check-certificate https://gitlab.com/spiritysdx/Oracle-server-keep-alive-script/-/raw/main/oalive.sh


