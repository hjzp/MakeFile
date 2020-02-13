Git官方文档： https://git-scm.com/docs

## 安装部署
* 服务端  
GitLab: https://docs.gitlab.com/ee/README.html
* 客户端  
TortoiseGit

## 概念

## Git **vs** SVN

## 流程
* Git flow  
清晰可控，但相对复杂，需长期维护master、dev这2个分支，适用于版本发布，即一段时间产生一个版本
* Github flow  
适用于持续发布（如网络项目）
* **Gitlab flow**  
是上述2个流程的结合，采取“上游优先”原则，尽可能在上游修改，下游去取最新代码来合并。  
11个规则：https://www.cnblogs.com/linuxprobe/p/5778525.html

## 基本操作
* clone  
git clone https://github.com/XXX.git   //注意是.git后缀

* pull **VS** fetch+merge    
  
  功能上 pull = fetch+merge ，但原理不同：pull命令相当于暴力更新，直接把远程分支的内容更新到本地仓库中的head目录（add/commit操作目录）；fetch命令只是下载远程分支代码到本地仓库中的remote目录，不更新head目录，merge命令是把remote目录合并到head目录。  
  
  pull命令会在未经确认的时候更新本地内容，fetch+merge方式更安全。

* 权限控制  

* 忽略文件（不加入版本库）

## 问题  
* 删除分支后，其它与该分支有关系的分支历史记录会不会被删除？  

* 多产品来自同一个master，此时如何作分支管理？

* 如何在Gitlab中进行issue跟踪？

* 产品发布一段时间后，线上出现了bug，从交付分支拉出hotfix分支，修复后merge到交付分支和master分支（或开发分支），如果在产品发布后的这段时间里，master分支（或开发分支）进行了重大重构，hotfix如何merger回master分支（或开发分支）？

## 应用场景
* 当前**分支A**的代码没写完，被告知紧急处理另外一个**分支B**的bug  
在A分支执行git stash，保存未写完的代码，切换到B分支（git checkout B），解决B分支的bug后（commit+push），切回到A分支，执行git stash pop，取出当时未写完的代码
