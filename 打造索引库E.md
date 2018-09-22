# 本地私有索引库 和 远程私有索引库的打造

### 1.打造本地私有索引库
1.创建一个locaLib的文件夹 （到指定目录）
  a。 pod lib create pod的库名称         创建一个pod 的模版库  
            （1.使用哪门语言，  是否需要一个测试 demo   是否需要frameworks（no） 是否需啊哟测试（no）是否需要类前缀（可以给一个库的类前缀））
  b。   spec 文件进行相关的配置。
  
  
 ### 2.远程私有索引库
 1. pod repo add 地址        将远程私有库克隆到本地
 2. pod lib create 库名称      核心代码拉入库中，    pod install 测试一下
 3. git add.      git commit -m ‘’    git remote add origin 对应的url     git push origin master   git tag ‘tag值’    git push -tags
 4. pod lib lint     和  pod spec lint   和 pod repo push 库名称.spec          本地远程都进行校验  然后提交spec 文件 
 3. 
















###远程索引库 和 本地索引库的区别
1.打造本地私有索引库， s.homepage 不需要配置， 但是必须填写（可以添加假的）
2.打造本地私有索引库  s.source 不会验证，也不需要配置 本地源码路径写空 
