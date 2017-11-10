# 打过的命令行

## vpn客户端以及依赖的iprout安装包

	sudo dpkg -i iproute_3.12.0-2_all.deb
	sudo dpkg -i xl2tpd_1.1.12-zju2_amd64.deb

### 连接	

	sudo vpn-connect -c
	sudo vpn-connect 
	sudo vpn-connect -d

## 开发环境相关:vim, pip3, jedi, git, curl, jedi-vim

	sudo apt install vim
	sudo apt-get update
	sudo apt-get install python3-pip
	pip3 install jedi
	sudo apt install git
	sudo apt install curl
	git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
	Plugin 'davidhalter/jedi-vim'
	:PluginInstall

## DeepLearning 相关:tensorflow(cpu only), keras, 测试

	sudo pip3 install tensorflow

	pip3 install matplotlib	
	pip3 install keras	
	python3 mnist_mlp.py

### 解决方法

	sudo mkdir -p /etc/pki/tls
	sudo ln -s /etc/ssl/certs /etc/pki/tls/certs
或者自己下载mnist.npz 放入 ~/.keras/datasets

## vim-markdown
	sudo apt install nodejs
	sudo apt install npm
	sudo npm -g install instant-markdown-d
	Plugin 'suan/vim-instant-markdown'	
	:PluginInstall

## 一堆python库
	
	sudo pip3 install mistune
	
