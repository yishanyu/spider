# spider

配置好数据库连接conn
配置好表名（包括表前缀），字段名（可用英文逗号隔开多个字段）

直接运行python3 multiple.py即可

输入线程数，可输入1至无限，把结果集平均分配到N个线程并行处理，爬取字段中通过正则表达式匹配到的URL资源存到本地

然后就泡杯茶，慢慢让他爬吧，如有疑问，欢迎留言交流。

----
conn配置参数：
hostname：数据库地址
username：用户名
password：密码
database：数据库名
hostport：数据库端口

cfgs配置参数：
table：表名
column：字段名，可多个
offset：开始游标（当输入的线程数大于1则该项无效，大于1表示游标由线程数自动分配）
vmode：控制台显示模式，可选为full/standard/simple
limit：每次从数据库取多少条记录（内存大可设大，内存小可设小）
sleep：每次处理完limit条记录后休息多少秒


