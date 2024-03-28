# git开发全流程
假如出现了类似下面的报错
```
fatal: unable to access 'https://github.com/homura-yw/01Group_docs.git/': Failed to connect to github.com port 443 after 21082 ms43 after 21082 ms: Couldn't connect to server
```
大概率是因为网络不好，多试几次就行。
**新入门项目的时候建议使用这条命令**
```
git clone https://github.com/homura-yw/01Group_docs.git
```

**开一条你自己的分支**
```
git branch <new branch>
git checkout <new branch>
```
然后进行code就行了
**注意一点就是，假如远程仓库更新了，本地同步远程仓库建议用下面这条命令**
```
git pull origin main
```

**假如要提交代码，移动到项目主目录，采用下面的命令**
```
git add . ## 即将这个目录下的所有改动加入进去,不要忘记后面那个点
```
**然后在本地提交改动**
```
git commit -m "my message"
```
**最后将提交推送到对应的远程仓库，切记不要提交到main分支**
```
git push origin <new branch>
```
