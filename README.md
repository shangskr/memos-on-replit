# Memos on replit
基于[sxbai/memos-on-replit](https://github.com/sxbai/memos-on-replit)修改，利用github action构建最新版本Memos ||
fork于[SinzMise/memos-on-replit](https://github.com/SinzMise/memos-on-replit)，SinzMise利用github action构建最新版本Memos

## 使用教程
1.新建一个replit项目，环境选择`Bash`或`Blank Repl`

2.运行一键安装脚本：
```
bash <(curl -s https://raw.githubusercontent.com/shangskr/memos-on-replit/main/install.sh)
```
3.点击“Run”按钮

开始使用吧！

## 更新教程
运行一键更新脚本：
```
bash <(curl -s https://raw.githubusercontent.com/shangskr/memos-on-replit/main/update.sh)
```
4.利用github action构建最新版本Memos（通过[SinzMise](https://github.com/SinzMise/memos-on-replit)的教学习得此技能！）
 （1） 打开https://github.com/settings
 （2） 找到Developer settings打开Personal access tokens的Tokens (classic)创建一个不过期的Tokens待用 
       (注意勾选repo的全部选项和勾选workflow)
 （3） 打开你fork的项目点击settings找到Actions中的General选中Read and write permissions和Allow GitHub Actions to create and approve pull requests
保存
       然后打开Secrets and variables中的Actions点击New repository secret创建3个New repository secret
       分别为`GH_EMAIL``GH_NAME``GH_TOKEN`分别对应GitHub绑定的邮箱，GitHub的名称，和刚才（2）中创建的Tokens
 （4） 点击`Actions-->I understand my workflows, go ahead and enable them`
       之后点击`update-memos`并启用`workflow`然后点击`Run workflow--->Run workflow`进行第一次运行
 （5） 等待运行完毕即刻就可以使用一键更新脚本了
