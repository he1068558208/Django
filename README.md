# Django
MVC:Model View Controller

MVT:Model View Template

B/S:Browser Server

C/S:Client Server

安装虚拟环境:pip install virtualenv

建立虚拟环境:virtualenv --no-site-packages testenv

切换目录:cd testenv

        cd Scripts

进入虚拟环境:activate

安装pymysql:pip install pymysql

退出虚拟环境:deactivate

查看虚拟环境下安装的所有包:pip list

安装django:pip install django==1.11

在虚拟环境下执行:django-admin startprotject helloworld

cd helloworld

启动django项目:python manage.py runserver (IP:端口)

创建app:python manage.py startapp appname

配置：settings.py文件中INSTALLED_APPS中写的name属性

模型：在models.py文件中定义class 模型名称

db_tables:定义数据库中的表名称

app:__init__.py 初始化,配置pymysql链接的地方

admin.py:管理后台注册模型

apps.py:settings.py里面注册app的时候需要使用到。一般不推荐这样使用。
		               配置信息位置，databases等

urls.py:url路由

wsgi.py:网关

from app.apps import Appconfig

AppConfig.name
model.py:写模型的地方

views.py:写处理业务逻辑的地方

迁移数据库 ：python manage.py makemigrations
	                  python manage.py migrate

保持数据
stu = Student()
stu.name = 'XXX'
stu.save()
