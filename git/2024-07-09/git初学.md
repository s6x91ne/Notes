---
date: 2024-07-09
---
## 源视频：[Git 和 GitHub 零基礎快速上手](https://www.youtube.com/watch?v=FKXRiAiQFiY&t=620s)
### 建立仓库
#### 设置用户名
```
git config --global user.name "s6x91ne"
```
#### 设置邮箱
```
git config --global user.email "xiaomianyangkk@gmail.com"
```
- 邮箱是否需要真实填写？
- 邮箱后期在上传github时，虽然不会被真正核实，但是不建议填写一个错误的邮箱。注册github时会要求校验邮箱，如果本地仓库的邮箱和github的邮箱不一致，则会导致github显示上传信息时，只会显示用户名，不会显示邮箱。
### 初始化
```
git init
```
- 会在当前建立.git的隐藏文件夹
- 将其删掉，也就实现了取消本地仓库
### 查看仓库状态
```
git status
```
### 将文件从Untracked变为tracked
```
git add <文件名.后缀>
```
提交
```
git commit -m "修改说明"
```
- m：message
### 查看log
```
git log
```
- 简化版
```
git log --oneline
```

## 源视频[# GeekHour教程 # Git教程07](https://www.youtube.com/watch?v=9oV9PVoeJX4&list=PLDBEQHWAyt9FbN7TANIXlUvtRhdoBCEQ5&index=7)

### 比较文件
```
git diff
```
- git diff默认什么都不加的话，比较的是工作区和暂存区的差异

```
git diff head
```
- 比较工作区和版本库之间的差异

```
git diff --cached
```
- 比较暂存区和版本库之间的差异

```
git diff <提交ID1> <提交ID2>
```
- 比较两个版本之间的差异

```
git diff HEAD~ HEAD
```
- 比较最近一次提交和上一次提交的差异

```
git diff HEAD~2 HEAD
```
- 比较最近一次提交和上上次提交的差异

```
git diff HEAD~2 HEAD <filename>
```
- 比较最近一次提交和上次提交的差异，并且只比较filename的差异，其他文件的差异不会比较