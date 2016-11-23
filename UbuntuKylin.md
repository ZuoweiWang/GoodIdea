[Ubuntu软件源详解](http://woshijpf.github.io/2016/10/23/Ubuntu%E8%BD%AF%E4%BB%B6%E6%BA%90%E8%AF%A6%E8%A7%A3/)
vmtools setup
-
open-vm-tools
-

$ sudo apt install open-vm-tools open-vm-tools-desktop


Ubuntu使用ppa源安装最新版git
-
1. 添加git源

$ sudo add-apt-repository ppa:git-core/ppa
2. 更新软件列表

$ sudo apt-get update
3. 安装git

$ sudo apt-get install git -y

NVM setup[https://github.com/creationix/nvm]
-
sudo apt install build-essential libssl-dev -y

wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.32.1/install.sh | bash

