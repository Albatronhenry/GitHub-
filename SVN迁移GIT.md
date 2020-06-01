# SVN迁移GIT

切记，不管什么时候不要用中文作为项目路径，不然导致未知错误！

## 1.迁移记录如下（window环境下）

1. gitbash 在相应目录右键 gitbash to here,然后执行

   ```java
   git svn clone https://192.168.1.250:8443/svn/江西财政一体化3.0.5/fap_sync_client/trunk/fap_sync_client
   
   ！！！！！方法一：如果项目记录太多/大，请使用如下命令（有可能没用）
       
   git svn clone -r  version_start:HEAD https://192.168.1.250:8443/svn/江西财政一体化3.0.5/fap_sync_client/trunk/fap_sync_client
   
   ！！！！！方法二：
   查看svn日志：
       git svn rebase
       svn log --stop-on-copy https://192.168.1.250:8443/svn/江西财政一体化3.0.5/fap_sync_client/trunk/fap_sync_client
   
   到目前为止，-rN选项，其中N是拉的修订。例：
   git svn clone -r143 https://192.168.1.250:8443/svn/江西财政一体化3.0.5/fap_sync_client/trunk/fap_sync_client
   
   ```

2. 因项目路径包含中文导致乱码，找不到路径而无法clone，需要到创建的fap_sync_client目录下找到.git目录下的config,编辑对应乱码路径为正常路径

   ```java
   [svn-remote "svn"]
   	url = https://192.168.1.250:8443/svn/%BD%AD%CE%F7%B2%C6%D5%FE%D2%BB%CC%E5%BB%AF3.0.5/fap_sync_client/trunk/fap_sync_client
   	fetch = :refs/remotes/git-svn
   更改并保存：
   [svn-remote "svn"]
   	url = https://192.168.1.250:8443/svn/江西财政一体化3.0.5/fap_sync_client/trunk/fap_sync_client
   	fetch = :refs/remotes/git-svn
   ```

   4. cd fap_sync_client 执行 git svn fetch

   5.  关联本地clone代码同时关联git项目

      ```java
      git remote add origin http://git.yonyou.com/abu/fap_sync_client.git
      ```

   6. ```java
      git remote -v 
      查看关联情况，如果关联有误，可以删除关联 git remote rm origin
      ```

   7. 提交记录之前，先拉取远程git项目文件(README.md)，否则直接提交会报错 

      ```java
      git pull --rebase origin master
      ```

   8. 拉取成功后，执行push命令

      ```java
      git push -u origin master
      ```

## 2.git如何删除已经提交的文件夹

在项目相应目录，执行一下语句实现删除

首先进入你的master文件夹下, Git Bash Here

> $ git pull origin master                    # 将远程仓库里面的项目拉下来
>
> $ dir                                                # 查看有哪些文件夹
>
> $ git rm -r --cached .idea              # 删除.idea文件夹
> $ git commit -m '删除.idea'        # 提交,添加操作说明
> $ git push -u origin master        # 将本次更改更新到git项目上去

## 3.git clone out of memory

git config --global pack.windowMemory 256m

### 4.创建分支

```cmd
# 创建分支
git branch dev
# 切换分支
git checkout dev
# 等同于上面两句
git checkout -b dev
```

加入单个文件：

```cmd
git add xxx.php
```

加入整个目录：

```
git add xxx/
```

加入所有目录及文件夹：

```
git add -A
```

### 5.查看操作日志 git log 查看状态 git status

### 6.回退某次提交节点

```cmd
git reset --soft commitID  
//只删除commitID之后的提交记录log，代码的改动还在。

git reset --hard commitID  
//彻底删除commitID之后所做的改动，代码也一起回退回来了。 (慎重用，用前最好备份一下代码，或者用git diff 生成一个patch)
```

> git push 到gitlab远程仓库的时候，出现报错”Everything up-to-date”，严格来说也不算报错，它只是在告诉你，提交区所有的东西都是最新的。
>
> $ git push origin master
> Everything up-to-date
>
> 之所以引起这个信息的原因有：
> 1）没有git add;
> 2）git add 了，但忘了git commit -m “提交信息”。
>
> 我是第1种情况。

### 7.git tag使用

> 1.从远程仓库地址获取指定标签版本
>
> git clone --branch v1.6 http://git.yonyou.com/qingcloud/git/testone.git
>
> 2.创建标签
>
> git tag -a v1.7 -m "tag1.7"
>
> 3.显示标签
>
> git tag      /               git tag -l
>
> 4.显示标签详细信息
>
> git show v1.6
>
> 5.删除标签
>
> git tag -d v1.6
>
> 6.删除远程仓库标签
>
> git push origin :v.16
>
> 7.提交到远程仓库
>
> git push origin  v.17

> 创建分支并检出
>
> git  checkout -b henry  http://git.yonyou.com/qingcloud/git/testone.git

### 8.代码冲突处理

当我们clone/checkout项目后，在本地修改后，可能与另外一个分支产生冲突

> 方法一：

> 1.提交之前，缓存到本地stash
>
> git stash save "冲突提交前保存" 
>
> 2.本地提交git commit
>
> 3.git pull 拉取分支最新
>
> 4.根据stashed,选择对应stash，解决对应冲突
>
> 5.git push ....

> 方法二：

> 1.直接先本地提交 git commit
>
> 2.git pull 
>
> 3.获取冲突文件，git reset远程仓库最新分支
>
> 4.修正冲突文件，重新git push

#### 9.git迁移git

git push --mirror 新的git地址