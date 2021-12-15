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

## 针对repo开发的常规指令

```command line
git add
git commit [-m] [-a]
git diff [--staged]
git status [--short]
git rm [-f] [--cache](--cache指明从staged area删除该文件但不从working directory删除文件)
git mv (用来对文件进行重命名)
```

## 显示repo开发commit历史记录

```command line
git log [--patch] [--stat] 
[--pretty=oneline(short/full/fuller/format:"%h - %an, %ar : %s")] 
[--graph] [-<n>](e.g. -2) [--since=2.weeks] [--until=] [--auther] [--grep] 
[-S <string>](pickax option, 用来显示指定字符串次数改变的commit os: 建议通过实例理解) 
[-- <path>](重要，用于显示路径文件或文件夹更改过的commit)

e.g. (os: 经典叠buff)
For example, if you want to see which commits modifying test files in the Git source code history were committed by Junio Hamano in the month of October 2008 and are not merge commits, you can run something like this:
git log --pretty="%h - %s" --author='Junio C Hamano' --since="2008-10-01" \
   --before="2008-11-01" --no-merges -- t/
```

## 进行repo操作回退

```command line
git commit [--amend](对上次commit进行修补工作)
```

## 针对repo配置的指令

```command line
git init
git clone
git config
git push
```
