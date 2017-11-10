# 打过的命令行

## vpn客户端以及依赖的iprout安装包

	sudo dpkg -i iproute_3.12.0-2_all.deb
	sudo dpkg -i xl2tpd_1.1.12-zju2_amd64.deb

### 连接	

	sudo vpn-connect -c  				# 连接vpn 第一次
	sudo vpn-connect 					# 连接 必须要以root身份运行
	sudo vpn-connect -d 				# 断开

## 开发环境相关

	sudo apt install vim 				# 安装vim
	sudo apt-get update 				# 换源更新
	sudo apt-get install python3-pip 	# 安装pip3
	pip3 install jedi 					# 安装jedi
	sudo apt install git				# 安装git
	sudo apt install curl				# 安装curl
	git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim		# 安装 Vundle
	Plugin 'davidhalter/jedi-vim'		# .vimrc中添加
	:PluginInstall 						# vim中执行，安装jedi-vim

## DeepLearning 相关 

	sudo pip3 install tensorflow		# 安装tensorflow

	pip3 install matplotlib				# 安装 matplotlib
	pip3 install keras					# 安装 keras
	python3 mnist_mlp.py				# 测试 在下载时失败

### 解决方法

	sudo mkdir -p /etc/pki/tls
	sudo ln -s /etc/ssl/certs /etc/pki/tls/certs
或者自己下载mnist.npz 放入 ~/.keras/datasets

## vim-markdown
	sudo apt install nodejs
	sudo apt install npm
	sudo npm -g install instant-markdown-d
	Plugin 'suan/vim-instant-markdown'	# .vimrc中添加
	:PluginInstall						# vim中执行

