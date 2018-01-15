# uts-rest-api使用手册

* **Authentication.py**定义了Authentication类，其使用umls api-key与nih建立登录访问的过程，已经在代码中固定了api-key (b3e4c263-fc38-4d7c-aaed-17ca239beed5)。Authentication类中有两个函数如下：
	* getgt是为了获得Ticket-Granting Ticket
	* getst是为了获得Service Ticket
* **retrieve-cui-or-code.py**脚本的功能是使用CUI获得UMLS以及其他数据库中的数据。参数如下：
	* -v: UMLS数据库的版本
	* -i: UCI代码
	* -s: 指定数据库