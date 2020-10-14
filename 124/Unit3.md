# 权限

|      |       | 文件 |  文件夹  |
| :--: | :---: | :--: | :------: |
|  r   | read  |  看  |  看内容  |
|  w   | write |  写  |   新建   |
|  x   | 执行  | 脚本 | 进文件夹 |

| rwx  |      |      |
| ---- | ---- | ---- |
| r--  | 4    |      |
| -w-  | 2    |      |
| --x  | 1    |      |

| u    | user  |      |
| ---- | ----- | ---- |
| g    | Group |      |
| o    | other |      |
| a    | all   |      |



```bash
#ls -l
[root@foundation0 ~]# ls -l /etc/fstab 
-rw-r--r--. 1 root root 996 Oct 18  2019 /etc/fstab
#chmod 
[kiosk@foundation0 ~]$ chmod g+w,o=- a.txt 
[kiosk@foundation0 ~]$ chmod go=rx a.txt 
[kiosk@foundation0 ~]$ chmod 755 a.txt 
[kiosk@foundation0 ~]$ chmod -R 755 a.txt  #R为递归，意思是将文件及文件内的东西权限全部改为755

#chown
chown kiosk:bin  a.txt
chown kiosk  a.txt
chown :bin  a.txt
chown -R kiosk:bin  a.txt

#suid=4=s普通用户拥有该命令所属用户的身份执行
#sgid=2=s
#stick=1=t
```

