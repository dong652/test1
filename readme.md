欢迎使用JSPGOU v6版，请按照以下步骤进行软件安装：

一、安装运行环境（JDK7+TOMCAT7+MYSQL5及以上，具体安装过程请参考本下载包中的相关说明文档）;

二、在mysql数据库中创建jspgou数据库(推荐使用此数据库名，否则参照第三条修改对应的数据库链接信息)，字符集为utf-8，

三、更改数据库链接,程序包内ROOT\WEB-INF\config\jdbc.properties文件第20行左右
	jdbc.url=jdbc:mysql://127.0.0.1:3306/创建好的数据库名?characterEncoding=UTF-8
	jdbc.username=登录数据库用户名
	jdbc.password=登录密码

三、将压缩包内 DB文件中jspgou.sql文件导入至创建好的jspgou数据库中，如导入中出现执行sql语句过长问题，请修改
    mysql配置文件my.ini,linux下为my.cnf文件中max_allowed_packet参数为64m，默认为1m

二、将程序解压后的ROOT文件夹拷贝到tomcat安装目录下的webapps文件夹下（例如：D:\Tomcat7\webapps\），启动tomcat，
	输入附录中的地址，如能正常显示，即表示部署成功


附：
	系统管理后台登录：http://localhost:8080/jeeadmin/jspgou/index.do
	用户名：admin
	密  码：12345
