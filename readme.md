1.  在Ubuntu上安装git

	$ sudo apt-get install git
	
2.  设置

	$ git config --global user.name meihao1203
	
	$ git config --global user.email meihao19931203@outlook.com
	
3.  安装Vundle(vim插件管理器)

	$ git clone https://github.com/VundleVim/Vundle.vim.git   ~/.vim/bundle/Vundle.vim

	$ cd ~/
	
	$ mv .vimrc vimrc.bak
	
	$ cd ~/.vim/bundle/Vundle.vim
	
	$ cp vimrc ~/.vimrc
	
	$ vim
	
	:PluginInstall


----------
配置.bashrc文件，ssh协议登陆Linux系统显示效果：![img.png](https://github.com/meihao1203/Vim/blob/master/img.png)
	
	$ vim ~/.bashrc
最后一行添加：
	
	`export PS1="\[\e[32;1m\][\u@\h \w\a]$>\[\e[0m\]"`
