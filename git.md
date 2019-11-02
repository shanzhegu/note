# git


### .gitignore
建立仓库时，.gitignore 文件是必须的，可以避免上传一些无用文件，常见的忽略项
```shell
  .DS_Store
  /dist

  # node
  node_modules

  # local env files
  .env.local
  .env.*.local

  # Log files
  npm-debug.log*
  yarn-debug.log*
  yarn-error.log*

  # Editor directories and files
  .idea
  .vscode
  *.suo
  *.ntvs*
  *.njsproj
  *.sln
  *.sw?
```

### 常用命令
git config --global user.name "Your name"
  全局设置用户名
git config --global user.email "email@email.cn"
  全局设置用户邮箱
git config --list/-l
  查看设置项
git config --global --list/-l
  查看全局设置项

### 远程仓库相关
git remote add origin git@github.com:liao/learn.git
  和远程仓库 git@github.com:liao/learn.git 建立连接，并命名为 origin ，这个名字是 github、dev 等
git remote -v
  和远程仓库的关联，及对应的权限(fetch/push)
git remote rm origin
  删除和 远程仓库origin 的连接

### 分支相关
- 查看当前分支 和 远程分支的映射关系。有没有分支、和哪个分支关联
git branch -vv
  有关系则 * master ccc8e96 [origin/master] update axios
  没有关系，分支名后不会显示中括号的内容
- 把'当前分支'和'远程仓库origin的dev分支'关联起来
git branch -u origin/dev
  关联成功后会有提示，Branch dev set up to track remote branck dev from origin
