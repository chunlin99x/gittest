##### ����Github��user name ��emial

* �� Git Bash��������������
 
```
$ git config --global user.name "�û���"
$ git config --global user.email "����"
```

* �������ˣ�����ͨ�����������в鿴git����

```
$ git config --list
```


* ����SSH key

�鿴�����Ƿ����SSH keys,��Git Bash,������:

```
cd ~/.ssh
```

�������������ʾ�� No such file or directory
����Ѿ������������~/.sshĿ¼�����ݵ�ǰkey��.sshĿ¼����Ȼ��ɾ����

* ��Gti bash�����������������ssh key
$ ssh-keygen -t rsa -C "your_email@example.com"
�м����������ʾ���룬�ֱ��ʾkey�ı���Ŀ¼�٣�˽Կ���룬˽Կȷ������
�����ζ�����ֱ���ûس����ɡ�

ֱ���ûس����ɵ���Կ·����C:\Users\xbting.ssh

����C:\Users\xbting.sshĿ¼����id_rsa.pub�����������key������key
�ص�gitub������ Account Settings���˻����ã������ѡ��SSH Keys��Add SSH Key,title����ճ��������������ɵ�key��

Ϊ����֤�Ƿ�ɹ�������git bash�������������

``` 
$ ssh -T git@github.com 
```


##### ����ǵ�һ�εĻ���ʾ�Ƿ�continue������yes�ͻῴ����
You've successfully authenticated, but GitHub does not provide shell access ��

�����ѳɹ�����github��github����ssh�ɹ�

���ߣ�Hifate
���ӣ�https://www.jianshu.com/p/861f1ce33f6a
��Դ������
��������Ȩ���������У��κ���ʽ��ת�ض�����ϵ���߻����Ȩ��ע��������

