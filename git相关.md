# Componentization
  1. git add .    添加本地所有文件
  2. git commit --m '添加你的记录信息'           都会产生一个版本号（实际是 40 位的哈希值）
  3。 git tag ‘版本号： 如 0.1.0’               
  4. git push --tags      将本地所有tag 上传到远程仓库
  5. git tag -d 0.1.0      删除对应版本的对应tag
  6. git remote add origin 对应git的远程地址        将本地仓库与远程链接 ， 链接完 拉代码 然后push 到远程仓库
  7. git push origin 对应的分支号        例如  git push origin master
  
  
  
  git 基本结构
  
  .git 代码仓库
  
  工作区  （提交完代码commit）  暂存区（有对应的分支）  （push） 远程仓库
  
