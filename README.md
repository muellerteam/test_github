# How to play with GitHub?

## Step by step instructions

> reference link: [msdn](https://docs.microsoft.com/zh-cn/learn/modules/introduction-to-github/)(微软提供的github学习教程 os: 微软啥都教...)

1. init local repo `git init`
2. create github repo
3. push your local repo to github repo `git push`
4. os: 直接看链接吧，不搬轮子了

## Trouble shooting

1. Can't use `git push` from my terminal

> [permission denied](https://docs.github.com/en/authentication/troubleshooting-ssh/error-permission-denied-publickey)
>
> [generate ssh key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
>
> [config ssh to github](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
>
> os: config ssh and something other... daunt me really...

## Reference

1. [about git](https://docs.github.com/en/get-started/using-git/about-git#basic-git-commands)(github上对git的介绍)
2. [git-reference](https://git-scm.com/docs)(git官网命令行参考手册 os: 我就看了几分钟，啃不动硌牙)
3. [Pro Git](https://git-scm.com/book/en/v2)(很详细的官方推荐书籍，只用看前几章就可以了 os: 这个倒可以花时间认真看看，写得不错)

## 针对repo开发的指令

```command line
git add
git commit [-m] [-a]
git diff [--staged]
git status [--short]
git remove [-f] [--cache] (--cache指明从staged area删除该文件但不从working directory删除文件)
git mv (用来对文件进行重命名)
```

## 针对repo配置的指令

```command line
git init
git clone
git config
git push
```
