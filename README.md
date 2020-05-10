# hello-world
#git project use mothod
#step 1:git clone https://github.com/qjx1122/hello-world.git
#step 2:cd hello-world;
#step 3:git add . #添加当前目录下所有文件,*表示提交所有有变化的文件
#step 4:git status -s #列出当前目录所有还没有被git管理的文件和被git管理且被修改但还未提交
#step 5:git commit -m "first commit" #添加本次提交的注释，双引号中的字符自定义修改.
#step 6:git push #提交代码到远程git仓库

#git status #列出还没有被git管理的文件和被git管理且被修改但还未提交的文件
#git branch -a #查看远程项目所有分支，红颜色分支代表当前所在分支，其他的所列的就是所有分支了
#git log #查看历史提交信息
#git remote show origin #查看当前仓库基本信息
#git remote -v #查看项目远程地址
#git push -u origin master   （注：此操作目的是把本地仓库push到github上面，此步骤需要你输入帐号和密码）
#git remote rm origin #删除远程配置
#git remote add origin https://github.com/WebCrawlers.git #重新配置git远程地址

#git add -u: 把所有tracked文件中被修改过或已删除文件的信息添加到索引库。它不会处理untracted的文件。
#git add -A: 表示把中所有tracked文件中被修改过或已删除文件和所有untracted的文件信息添加到索引库。

#撤销操作
#1.git status #先看一下add 中的文件
#2.git reset HEAD #如果后面什么都不跟的话 就是上一次add 里面的全部撤销了 
#3.git reset HEAD XXX/XXX/XXX.java #就是对某个文件进行撤销了

#上传一个独立的分支（比如代码是从工程中直接DOWNLOAD ZIP，该文件与原MASTER分支是独立的）
#1.Git init #在本地工程目录下,生成.git 文件夹
#2.git add * #上传修改的文件,*可替换成具体要上传的文件名，*表示提交所有有变化的文件
#3.git commit -m "test" #添加上传文件的描述
#4.git branch test #创建分支
#5.git checkout test #切换分支
#6.git remote add origin https://github.com/yangxiaoyan20/BowlingScore.git #与远程分支相关联
#7.git push origin test #将分支上传


#上传一个与MASTER相关的分支（该分支是从MASTER中git clone 得到，相关信息在 .git 文件中）
#修改后源码后，在进行如下操作
#1、git add . #添加当前目录下所有文件,*表示提交所有有变化的文件
#2、git commit -m "test" #test为分支名
#3、git branch test #创建分支
#4、git checkout test #切换分支
#5、git push origin test:test
