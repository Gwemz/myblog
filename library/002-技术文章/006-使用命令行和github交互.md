## 使用命令行和github交互

### 全局配置
```
初次配置git环境时需要进行的步骤：(配置过之后不需要再次配置)

git config --global user.name "Gwemz"

git config --global user.email "3396543978@qq.com"

git config --global push.default simple
```
### clone一个已有的仓库做开发

```
git clone https://github.com/Gwemz/myblog.git .(将项目克隆到当前文件夹下)

git --help   //git相关命令查询
git status   //查看项目的状态(是否更新)
git add *    //添加需要更新的所有内容
git status   
git commit -m 'myblog'  //每次提交的标注
git push   //提交(需要输入用户名和密码)
```

### 管理分支
(除了 https://gwemz.github.io 之外其它 https://gwemz.github.io/myblog 如果需要访问则必须进行下述操作)

```
git branch gh-pages

git checkout gh-pages

git merge master

git push --set-upstream origin gh-pages
```
`注意 多使用git status 查看自己目前所在的分支`
