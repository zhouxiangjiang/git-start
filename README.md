# Git起步
Getting started with Git (GitHub)

## Git核心配置

```bash
git version  # 查看git版本 (v1.9.5+)

git config --global user.name 'Li Yun'                   # 全名
git config --global user.email leven.cn@gmail.com        # GitHub 注册邮箱
git config --global push.default simple

git config --list                                        # 查看当前配置
```

## Git基本命令

```bash
# 创建或克隆
git clone <repo-url> [<repo-name>]
git init

# 分支
git branch [-d|-D] <branch>
git checkout <branch>
git merge <branch>
git rebase <branch-or-commit>

# 提交
git diff [--cached]
git add|rm|mv <file ... or dir>
git status
git commit -m <commit-message>
git log
git pull [--rebase]
git push
git push [-f] <remote-repo> :<remote-branch>

# Git补丁
git format-patch -M <upstream-branch> <current-branch>.patch
git am <current-branch>.patch

# 标准补丁
git diff <upstream-branch> > <current-branch>.patch
git apply --check <current-branch>.patch
git apply <current-branch>.patch

# 标签
git tag -a <tag-name>
git push origin :refs/tags/<tag-name>

# 子模块
git submodule update --init
git submodule add <submodule-repo-url> <submodule-repo-name>
```

## 参考资料

- [Pro Git](http://www.git-scm.com/book/)
