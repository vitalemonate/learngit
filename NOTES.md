# 创建版本库
## 指令：
git init

git add xxx

git commit -m "balabala"
# 版本回退：
## 指令：
git status: 用于显示工作目录和暂存区的状态


git diff: 当工作区有改动，临时区为空，diff的对比是“工作区与最后一次commit提交的仓库的共同文件”；当工作区有改动，临时区不为空，diff对比的是“工作区与暂存区的共同文件”。


git log: 按时间先后顺序列出所有的提交，最近的更新排在最上面

## 总结：
1.HEAD指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，使用命令git reset --hard commit_id


2.穿梭前，用git log可以查看提交历史，以便确定要回退到哪个版本。


3.要重返未来，用git reflog查看命令历史，以便确定要回到未来的哪个版本。

# 工作区和暂存区:
git add命令实际上就是把要提交的所有修改放到暂存区（Stage），然后，执行git commit就可以一次性把暂存区的所有修改提交到分支