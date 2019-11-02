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
