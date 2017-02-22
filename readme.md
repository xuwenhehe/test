客户端下载（要vpn）：
https://github-windows.s3.amazonaws.com/GitHubSetup.exe
使用过程：
登录web端新建一个project
ssh-keygen -t rsa -C username@z.com 生成c/users/w/.ssh/id_rsa.pub，将内容贴到web上(setting-SSH and GPG keys-New SSH key)
git clone ssh://git@172.16.0.250:10022/username/projectname.git
将目录下的所有文件拷贝到本地git项目的存储目录(readme.md为说明文件)
git add *
(git status; git config --global user.email "username@z.com"; git config --global user.name "username")
git commit -m "description"
git push
最后设置project的属性权限等