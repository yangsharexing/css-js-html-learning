VS 使用 git 教程&emsp;以windows为例子

1 、首先：下载安装git（略）
2 、打开 Git Bash 命令行  设置全局用户信息
	&emsp;&emsp;git config --global user.name "yangsharexing" 
	&emsp;&emsp;git config --global user.email "1621456923@qq.com"
3、创建项目目录 
   &emsp; &emsp;mkdire test
4、进入目录，并初始化为git标准目录
    &emsp;&emsp;cd test
    &emsp; &emsp;git init
5、新建一个新文件并新增到配置
    &emsp;&emsp;touch README.md
    &emsp;&emsp;git add README.md
6、提交到本地仓库
   &emsp; &emsp;git commit -m "first commit"
7、设置提交66666
    &emsp;&emsp;git remote add origin https://github.com/yangsharexing/learning.git   &emsp;&emsp;//用你仓库的url   
8、更新远程仓库到本地（如果远程有提交就需要更新，不然第9步会失败）
   &emsp;&emsp;git pull origin master
9、git push -u origin master  //提交到你的仓库

10、VS打开项目目录
11、修改或新增文件
12、点击左侧的代码分支管理（VS会自动解析到目录下的git配置，并获取仓库地址等信息）
13、点击文件右侧的加号 相当于 commit
14、push文件即可

 
VS克隆项目到本地

1 、首先：下载安装git（略）
2 、打开 Git Bash 命令行  设置全局用户信息
	&emsp;&emsp;git config --global user.name "yangsharexing" 
	&emsp;&emsp;git config --global user.email "1621456923@qq.com"
    &emsp;&emsp;git config --global credential.helper store      
3、创建项目目录 
   &emsp; &emsp;mkdire test
4、克隆项目就可以用VS打开了
   git clone https://github.com/yangsharexing/   //你的仓库地址
