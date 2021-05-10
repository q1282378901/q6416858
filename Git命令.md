# Git命令

## 1.配置用户信息

```shell
git config --global user.name "你的名字"
git config --global user.email "你的邮箱"
```

## 2.检查配置信息

```shell
git config --list --global
```

## 3.初始化仓库

```shell
git init
```

## 4.检查文件状态

```shell
git status
git status -s ##以精简的形式展示
```

## 5.添加到暂存区

```shell
git add 文件名字
```

## 6.提交到仓库

```shell
git commit -m  "描述信息"
```

## 7.撤销去文件的修改

```shell
git checkout -- 文件名
```

## 8.一次添加多个文件

```shell
git add .
```

## 9.取消暂存区的文件

```shell
git reset HEAD 文件名
git reset HEAD -- 文件名(用这个)
git reset HEAD . ## 取消全部暂存区的文件
```

## 10.跳过暂存区

```shell
git commit -a -m "描述信息"  #一定要是追踪过的文件才行
```

## 11.删除文件

```shell
git rm -f 文件名 #全部删除
git rm --cached 文件 #只删除仓库里面的保留本地文件
```

## 12.查询提交历史

```shell
git log
git log  -数量
git log --pretty=oneline #展示所有历史记录
```

## 13.回退到指定版本

```shell
git log --pretty=oneline #展示所有历史记录

git reset --hard id #回退到指定id的版本

git reflog --pretty=oneline #在旧版本中展示所有历史记录

git reset --hard id #回退到指定id的版本
```

## 14.上传代码到github

```shell
git remote add origin https://github.com/nikoo007/zzitcast_35.git
git push -u origin master
git push #第二次以上提交
```

## 15.生成SSH-key

```shell
ssh-keygen -t rsa -b 4096 -C "your_email@example.com" #敲击3次回车
```

## 16.测试ssh-key是否设置成功

```shell
ssh -T git@github.com
```

## 17.查看分支

```shell
git branch
```

## 18.创建分支

```shell
git branch 分支名字
```

## 19.快速创建和切换分支

```shell
git checkout 分支名字
git checkout -b 分支名字
```

## 20.合并分支	

```shell
git merge 分支名字
```

## 21.删除分支

```shell
git branch -d 分支名字
git branch -D 分支名字  #强制删除
```

## 22.拉取最新的代码

```shell
git pull
```

## 23.删除远程分支

```shell
git push origin(远程仓库的名字) --delete 远程分支的名字
```











