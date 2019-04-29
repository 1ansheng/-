# 使用git/github
## git基本操作
1. 下载桌面版git

2. git config --global user.name 'myname'
   git config --global user.email 'email@example.com'
   //设置 用户名称 邮箱
3. git init  //在文件夹下创建中央仓库
4. touch 1.cpp //创建文件
   git status //查看状态
   git add 1.cpp //添加到暂存区（**每次修改文件后需要执行此步骤**）
   git commit -m "init commit" //提交到仓库
5. cat 1.cpp //编辑文档后更新 -> 添加到暂存区 -> 提交到仓库
6. rm -rf 1.cpp //删除文件
7. git rm 1.cpp //从git仓库删除

##  git连接远端GitHub

1. ssh-keygen -t rsa -C "mail@example.com" 
2. clip < ~/.ssh/id_rsa.pub   // 复制密钥
3. 将密钥添加到GitHub SSH key里面
4. git remote add  origin git@github.com:ansheng/repository.git //这里创建项目远端连接 GitHub库
5. git push -u origin master  //把 origin 上传到 上一步连接仓库的 master分支上

