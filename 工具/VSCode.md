## 快捷键

| 快捷键 | 描述 |
| ------ | ------ |
| Ctrl + P | 直接输入字符串，搜索文件名；输入?，查看帮助信息 |
| Ctrl + G | 在当前文件中，跳转到行号 |
| Ctrl + T | 在整个工作区中，搜索符号(变量及函数) |
| Ctrl + Shift + O | 在当前文件中，搜索符号(变量及函数) |
| Ctrl + Y | 恢复 |
| Ctrl + W | 关闭当前窗口（文件）|
| Ctrl + F4 | 关闭当前文件 |
| Alt + ← | 向前导航编辑位置 |
| Alt + → | 向后导航编辑位置 |
| Alt + ↑ | 将当前行上移一行 |
| Alt + ↓ | 将当前行下移一行 |
| Shift + Alt + ↑ | 向上复制一行 |
| Shift + Alt + ↓ | 向下复制一行 |
| Alt + ↑ | 将当前行上移一行 |
| Alt + ↓ | 将当前行下移一行 |
| Ctrl + L | 选中当前行 |
| Shift + Alt + → | 展开选中内容 |
| Shift + Alt + ← | 缩小选中内容 |
| Ctrl + Shift + K | 删除当前行 |
| Ctrl + Enter | 在当前行下插入新行 |
| Ctrl + Shift + Enter | 在当前行上插入新行 |
| Ctrl + ] | 向左缩进 |
| Ctrl + \[ | 向右缩进 |
| Shift + Alt + F | 添加/取消注释 |
| Ctrl + / | 向左缩进 |
| Ctrl + Shift + \[ | 以递归的方式折叠代码 |
| Ctrl + Shift + ] | 向左缩进 |
| Ctrl + \[ | 以递归的方式展开代码 |
| Ctrl + K + J | 以递归的方式展开代码 |
| Ctrl + \[ | 展开代码 |
| Ctrl + Shift + Y | 打开调试控制台 |
| Ctrl + B | 显示/隐藏侧边栏 |

## 常用插件
* 中文  
* C/C++
* 代码提示 snip
* Remote SSH  
远程调试插件，左侧菜单栏-远程资源管理器-新建连接-选择配置文件-输入登录用户名、密码，连接成功后，可进行远程操作。保存登录密码，在windows主机上输入cmd命令（win10自带ssh client）：
* 括号颜色  
Bracket Pair Colorizer  
```shell
ssh-keygen -t rsa -b 4096
SET REMOTEHOST=root@192.168.1.245
scp C:\Users\Administrator\.ssh\id_rsa.pub %REMOTEHOST%:~/tmp.pub
ssh %REMOTEHOST% "mkdir -p ~/.ssh && chmod 700 ~/.ssh && cat ~/tmp.pub >> ~/.ssh/authorized_keys && chmod 600 ~/.ssh/authorized_keys && rm -f ~/tmp.pub"
```
