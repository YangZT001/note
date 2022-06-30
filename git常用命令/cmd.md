## 常用命令

### 设置用户名

git config --global user.name 用户名

### 设置邮箱

git config --global user email 邮箱

### 初始化本地库

git init

### 查看本地库状态

git status

### 添加到暂存区

git add <文件名>

### 从暂存区删除

git rm --cached \<file\>...

### 提交到本地库

git commit -m "日志信息" <文件名>

### 查看历史记录

git reflog

### 查看详细日志

git log

### 版本穿梭

git reset --hard 版本号

------

## 分支操作

### 创建分支

git branch \<分支名\>

### 查看分支

git branch -v

### 切换分支

git checkout \<分支名\>

### 合并分支

git merge \<分支名\>

------

## Github操作

账号						邮箱											密码

YangZT001			2264350090@qq.com			 字母符号密码

YangZT002			15968537511@163.com     	字母符号密码

YangZT003			yzt15557539150@163.com	字母符号密码

### 查看当前所有远程库别名

git remote -v

### 创建远程库别名

git remmote add \<别名\> <地址\>

### 推送本地内容分支到远程库

git push \<别名\> \<分支\>

### 从远程库克隆

git clone \<地址\>

### 远程库分支最新内容拉去并与本地合并

git pull \<远程库地址别名> \<分支别名>
