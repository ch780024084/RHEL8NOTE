# 环境配置

关闭VMware dhcp ：编辑 -> 虚拟网络编辑器

<img src="../img/image-20201010130745674.png" alt="image-20201010130745674" style="zoom:50%;" />

关闭杀毒软件

内存需求：至少3G

# 虚拟机启动

```
查看虚拟机状态 ：rht-vmctl status
```

![image-20201010134237205](../img/image-20201010134237205.png)

```
启动虚拟机： rht-vmctl start 
```

![image-20201010134526201](../img/image-20201010134526201.png)

![image-20201010134538202](../img/image-20201010134538202.png)

```
登录虚拟机 ：rht-vmview view 
```

![image-20201010134841466](../img/image-20201010134841466.png)

```
检查命令是否执行正确 echo $?
```

![image-20201010140316782](../img/image-20201010140316782.png)

# 终端切换

|      |               |              |
| ---- | ------------- | ------------ |
| 字符 | <Ctrl+Alt+Fx> | x in（2，6） |
| 桌面 | <Ctrl+Alt+F1> |              |

# prompt

```
who am i :查看当前用户
hostname :查看当前主机名
pwd :查看当前路径
<Ctrl+d>:注销
```

