---
date: 2024-07-09
---
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
### 比较文件
```
git diff
```
