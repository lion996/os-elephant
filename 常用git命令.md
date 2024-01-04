## 以下是一些常用的 Git 命令：

### 初始化本地 Git 仓库（创建新仓库）：
git init

### 配置用户名和邮箱：
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"

### 克隆远程仓库：
git clone <repository-url>

### 查看当前版本状态（是否修改）：
git status

### 添加文件至索引：
git add <file-name>  # 添加指定文件
git add .  # 添加当前目录下所有更改过的文件

### 提交：
git commit -m 'commit message'  # 提交
git commit --amend -m 'new message'  # 修改上一次提交的信息
git commit -am 'commit message'  # 将添加和提交合为一步

### 删除文件：
git rm <file-name>  # 删除指定文件
git rm -r *  # 删除所有文件

### 显示提交日志：
git log

### 显示某个提交的详细内容：
git show <commitId>

### 比较与上一个版本的差异：
git diff HEAD^

### 将当前分支推送到远程分支：
git push origin <branch-name>

### 获取所有远程分支（不更新本地分支，另需 merge）：
git fetch --all

### 获取远程分支并合并到当前分支：
git pull origin <branch-name>

### 显示所有已存在的标签：
git tag

### 显示所有本地分支：
git branch

### 切换到指定分支：
git checkout <branch-name>

### 从当前分支创建新分支并检出：
git checkout -b <new-branch-name>

### 删除分支：
git branch -d <branch-name>  # 删除已合并的分支
git branch -D <branch-name>  # 强制删除分支

### 合并指定分支到当前分支：
git merge <branch-name>