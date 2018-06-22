##### 设置Github的user name 和emial

* 打开 Git Bash，输入如下命令
 
```
$ git config --global user.name "用户名"
$ git config --global user.email "邮箱"
```

* 设置完了，可以通过下面命令行查看git配置

```
$ git config --list
```


* 配置SSH key

查看本机是否存在SSH keys,打开Git Bash,并运行:

```
cd ~/.ssh
```

如果不存在则提示： No such file or directory
如果已经存在了则进入~/.ssh目录，备份当前key（.ssh目录），然后删除。

* 再Gti bash里输入下面命令，生产ssh key
$ ssh-keygen -t rsa -C "your_email@example.com"
中间会有三次提示输入，分别表示key的保存目录再，私钥密码，私钥确认密码
这三次都可以直接敲回车即可。

直接敲回车生成的密钥路径：C:\Users\xbting.ssh

进入C:\Users\xbting.ssh目录，打开id_rsa.pub，复制里面的key，复制key
回到gitub，进入 Account Settings（账户配置），左边选择SSH Keys，Add SSH Key,title随便填，粘贴在你电脑上生成的key。

为了验证是否成功，可在git bash里输入下面命令：

``` 
$ ssh -T git@github.com 
```


##### 如果是第一次的会提示是否continue，输入yes就会看到：
You've successfully authenticated, but GitHub does not provide shell access 。

表明已成功连上github，github配置ssh成功

作者：Hifate
链接：https://www.jianshu.com/p/861f1ce33f6a
來源：简书
简书著作权归作者所有，任何形式的转载都请联系作者获得授权并注明出处。

