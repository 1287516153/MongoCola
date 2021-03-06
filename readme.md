#Release Note
       
* 可执行版本[需要 NET Framework 4.6] 更新时间:2015/12/31 16:00
* 下载地址:  <http://files.cnblogs.com/files/TextEditor/ReleaseVersion.zip>
* GitHub 项目地址 <https://github.com/magicdict/MongoCola/>
* 版本号：Ver 1.5(Beta)
 
***

# 开发和测试环境
## 操作系统：
* Windows 7
* Mac OSX 10.11.2
***
## 运行时：
* NET Framework 4.6
* Mono 4.5
* MongoDB 3.2.0 

***

## 驱动程序
CSharp Mongo Driver 2.2.0

***

# 项目说明
* ExternalTools:外部工具  
1. ConfigurationFile 配置文件编辑器
2. MultiLanEditor 多语言文件编辑器
* Assistant:业务逻辑和辅助类  
* Winform:窗体和控件  

# 计划
0. Fix Bug  
	解决所有发现的Bug 
1. Config Options  
	一个MongoService用Config File文件的生成工具 
2. 扩大Model.TryUpdate的使用范围  
	Winform使用了MVC的概念，自动将Model和UI双向绑定
	已经在frmConnnection/frmOption里面尝试了
3. MutliLanguage  
	进一步改进多语言系统
4. User System  
	用户系统

***

# 发布履历

##Ver 1.5(Beta)  2015/12/31 @ Shanghai China 
###MongoDB 3.2.0 新功能对应版本
1. Text Search V3 的对应：大小写敏感
2. Partial Index 的创建  
3. 独立外部工具 Configuration Creator 初版
4. 创建Collection时候可以设定DocumentValidation参数
5. MongoDump 增加 --gzip --archive
6. 修复添加Collection后UI没有实时更新的BUG 

***

##Ver 1.5(Alpha)  2015/07/09 @ Shanghai China
1. 重构代码，Mongo业务代码和界面代码分开
2. 新代码尽可能适配MongoDriver2.0.1
3. MongoServer尽可能用MongoClient代替
4. 窗体TabPage管理功能的独立化
5. TextSearch功能的修改（MongoDB 2.6之后使用不同的方法）
6. 各种Status改用树型结构表示
7. 新建数据库无效,删除数据库错误等问题.

***

# 已知BUG
1. 新建数据库时,必须要新建一个数据集.
2. MONO  Windows API Crash!
3. ZedGraph For Mono Chart
4. Status里面的列无效，MMVP和WireTiger数据集状态不同
5. MongoBin没有设置的时候，非Windows的时候，Cmd命令无法执行的问题
6. User命令未完成
7. JS文件等不应该保存到Mongo数据库中，如果没有获得客户允许的时候