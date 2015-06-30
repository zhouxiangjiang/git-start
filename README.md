# Git起步
Git / GitHub 使用样例

学习资料: [Pro Git](http://www.git-scm.com/book/) 第1,2,3章

## Git核心配置

```bash
git version  # 查看git版本 (v1.9.5+)

git config --global user.name 'Li Yun'                   # 全名
git config --global user.email leven.cn@gmail.com        # GitHub 注册邮箱
git config --global push.default simple

git config --list                                        # 查看当前配置
```

## GitHub工作流

新参与项目：

1. `Fork` 这个项目
2. 克隆项目 ```git clone <repo-url>```
3. 切换分支 ```git checkout test```
4. 更新文件
5. 查看更新的文件 ```git status```
6. 查看更新的内容 ```git diff```
7. 缓存更新 ```git add|rm|mv <file ... or dir>```
8. 查看更新的内容 ```git diff --cached```
9. 本地提交 ```git commit -m '<commit message>'```
10. 远程提交 ```git push```
11. 创建`Pull Request`并提交

已参与项目：

1. 切换分支 ```git checkout <branch-name>``` 或 创建分支 ```git checkout -b <branch-name>```
2. 远程同步 ```git pull```
3. 更新文件
4. 查看更新的文件 ```git status```
5. 查看更新的内容 ```git diff```
6. 缓存更新 ```git add|rm|mv <file ... or dir>```
7. 查看更新的内容 ```git diff --cached```
8. 本地提交 ```git commit -m '<commit message>'```
9. 远程提交 ```git push```
10. 创建`Pull Request`并提交

删除远程分支：

```bash
git push [-f] <remote-repo> :<remote-branch>
```

查看提交日志：

```bash
git log
```

发布

```bash
git tag -a <tag-name>
git push origin :refs/tags/<tag-name>
```


