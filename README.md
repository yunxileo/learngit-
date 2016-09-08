##  git 入门
+ 创建版本库  ``` git init ```
+ 把文件添加到版本库 ``` git add filename.txt ```  PS:先有文件才能添加 ,注意文件名称的大小写
+ 把文件提交到仓库 ``` git commit  -m "wrote a readme file" ```  


首先，登陆GitHub，然后，在右上角找到“Create a new repo”按钮，创建一个新的仓库：

在Repository name填入gitskills，其他保持默认设置，点击“Create repository”按钮，就成功地创建了一个新的Git仓库：

目前，在GitHub上的这个learngit仓库还是空的，GitHub告诉我们，可以从这个仓库克隆出新的仓库，也可以把一个已有的本地仓库与之关联，然后，把本地仓库的内容推送到GitHub仓库。

现在，我们根据GitHub的提示，在本地的learngit仓库下运行命令：

```
$ git remote add origin git@github.com:yunxileo/gitskills.git
```
之后可以用命令：

```
$ git push origin master
```

请千万注意，把上面的yunxileo替换成你自己的GitHub账户名，否则，你在本地关联的就是我的远程库，关联没有问题，但是你以后推送是推不上去的，因为你的SSH Key公钥不在我的账户列表中。

添加后，远程库的名字就是```origin```，这是Git默认的叫法，也可以改成别的，但是```origin```这个名字一看就知道是远程库。

下一步，就可以把本地库的所有内容推送到远程库上：