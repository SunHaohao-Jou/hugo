# github

## ssh推送

SSH 方式不仅更安全，而且有时能避开 HTTPS 端口封锁。

1. 先在 GitHub 添加你电脑的 SSH 公钥（如果没有，运行 `ssh-keygen` 生成，默认一路回车，然后把 `~/.ssh/id_rsa.pub` 内容粘贴到 GitHub 的 Settings → SSH and GPG keys）。

2. 修改仓库的远程地址：

   

```
git remote set-url origin git@github.com:SunHaohao-Jou/SunHaohao-Jou.github.io.git
```



再次推送：

```
git push -u origin main
```