# 一、github 新手教程

**1、git 新手使用手册: https://www.jianshu.com/p/bf95d885978e**

**2、廖雪峰git教程：https://www.liaoxuefeng.com/wiki/896043488029600/896067074338496**

**3、Markdown基本语法：https://www.jianshu.com/p/191d1e21f7ed/**

**4、git 命令总结: https://www.jianshu.com/p/dd7f18ed0bb1**

**5、如何在同一台电脑上使用 github 和 gitlab: https://www.jianshu.com/p/d97c6121952a**

**6、github 简单使用视频教程：https://www.youtube.com/watch?v=iX_T7EK-Dk0**

# 二、上传本地文件到Github新手教程

<a href="https://github.com/" target="_blank">github账号注册 官网</a>
 
<a href="https://git-scm.com/" target="_blank">git软件下载 官网</a>


```bash
1、创建个github账号，然后Create a new repository，假设repository name为: test

2、本地电脑创建个文件夹，名称任意取，但最好不要使用中文字符，假设文件夹名称为：test

3、本地电脑安装git软件，保持默认安装选项即可,安装完成后，在开始菜单里找到“Git”->“Git Bash”，蹦出一个类似命令行窗口的东西，就说明Git安装成功

4、安装完成后，还需要最后一步设置，在命令行输入：
git config --global user.name "Your account"             ----使用注册github账号
git config --global user.email "email@example.com"    ----使用注册github账号时所用的邮箱

5、进入test 目录里面，在命令行输入：
echo "# test" >> read.md
git init
git add read.md
git commit -m "first commit"
git remote add origin https://github.com/fj2020/test.git    ---gj2020是我注册的github账号
git push -u origin master

6、上传完成后，刷新页面：https://github.com/fj2020/test， 可以看到刚刚readme.md文件，内容为test
```
#### 注意：第一次上传，可能会弹出对话框，需要输入github账号和github密码


# 三、使用linux从github上面clone文件


```bash
yum -y update
yum -y install httpd php git
chkconfig httpd on
git clone https://github.com/fj2020/simple-web-app.git /var/www/html
service httpd start
```
