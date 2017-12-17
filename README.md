
基于 Django 1.10 和 Python 3.5搭建的博客系统

效果看这里：[kaming.xyz](http://kaming.xyz)

## 功能

 - 富文本编写([django-ckeditor](https://github.com/django-ckeditor/django-ckeditor))
 - 支持Markdown语法([markdown](https://github.com/Python-Markdown/markdown))
 - 后台管理([django](https://github.com/django/django))

## 环境配置
 - [django 1.10](https://github.com/django/django)
 - [python 3.5](https://www.python.org/)

## 安装

1. 克隆项目到本地
	```
	git clone https://github.com/JiamingWu233/blogproject.git
    ```

2. 创建并激活虚拟环境
在命令行进入到保存虚拟环境的文件夹，输入如下命令创建并激活虚拟环境：
	```
	virtualenv blogproject_env
	windows：
	blogproject_env\Scripts\activate
    linux：
    source blogproject_env/bin/activate
    ```
3. 安装项目依赖
   如果使用了虚拟环境，确保激活并进入了虚拟环境，在命令行进入项目所在的 django-blog-tutorial 文件夹，运行如下命令：
	```
   pip install -r requirements.txt
	```

4. 迁移数据库

   在上一步所在的位置运行如下命令迁移数据库：
   ```
   python manage.py migrate
   ```


5. 创建后台管理员账户

   在上一步所在的位置运行如下命令创建后台管理员账户

   ```
   python manage.py createsuperuser
   ```


6. 运行开发服务器

   在上一步所在的位置运行如下命令开启开发服务器：

   ```
   python manage.py runserver
   ```

   在浏览器输入：127.0.0.1:8000

7. 进入后台发布文章

   在浏览器输入：127.0.0.1:8000/admin

   使用第 5 步创建的后台管理员账户登录


## 感谢

 - [django-blog-tutorial](https://github.com/zmrenwu/django-blog-tutorial)


```text
Copyright 2017 Kaming

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```