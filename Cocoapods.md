# Componentizatio
Cocoapods 的基本使用




框架描述文件： （远程索引库） .spec 文件（包含框架名称， 版本号， 真是地址源码地址）
             （本地索引库） 使用命令 pod search  去检索索引文件  再去对应的 .spec 
                          pod install  根据本地索引 获取对应的 框架源码 进行安装
                          
                          
1. 第三方框架制作（将我们的。spec 文件丢到远程索引库中）   1.完成框架源码   2. 需要一个描述文件  3. 把描述文件上传到远程索引库中


1.pod lib lint     进行本地校验
2. pod spec lint  远程校验   （远程仓库一定要打了 tag，  链接tag 必须和远程一致）
3. pod trunk register 自己的邮箱号            trunk相当于自动化工具
