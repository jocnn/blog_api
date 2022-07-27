Blog API
===
Abstract: Se desarrollo la APi Blog usando Django + Django-RestFramework realizando un CRUD completo, documentación Redoc y Swagger-UI, se agrego seguridad para que las publicaciones solo sea editado por el autor, se agrego CORS, se agrego la app Accounts y Post, la autenticación es por token y el deployment se realizo en heroku.
## Papar Information
- Title:  `Blog API`
- Authors:  `jocnn`

## Install & Dependence
- python==3.10.5
- asgiref==3.5.2
- attrs==21.4.0
- black==22.6.0
- certifi==2022.6.15
- cffi==1.15.1
- charset-normalizer==2.1.0
- click==8.1.3
- cryptography==37.0.4
- defusedxml==0.7.1
- dj-database-url==0.5.0
- dj-email-url==1.0.5
- dj-rest-auth==2.1.11
- Django==4.0.6
- django-allauth==0.48.0
- django-cache-url==3.4.2
- django-cors-headers==3.10.1
- djangorestframework==3.13.1
- drf-spectacular==0.21.2
- environs==9.5.0
- gunicorn==20.1.0
- idna==3.3
- inflection==0.5.1
- jsonschema==4.7.2
- marshmallow==3.17.0
- mypy-extensions==0.4.3
- oauthlib==3.2.0
- packaging==21.3
- pathspec==0.9.0
- platformdirs==2.5.2
- psycopg2==2.9.3
- pycparser==2.21
- PyJWT==2.4.0
- pyparsing==3.0.9
- pyrsistent==0.18.1
- python-dotenv==0.20.0
- python3-openid==3.2.0
- pytz==2022.1
- PyYAML==6.0
- requests==2.28.1
- requests-oauthlib==1.3.1
- sqlparse==0.4.2
- tomli==2.0.1
- uritemplate==4.1.1
- urllib3==1.26.10
- whitenoise==5.3.0

## Use
- for run server
  ```
  (.venv) > python manage.py runserver
  http://127.0.0.1:8000/api/v1/users/
  http://127.0.0.1:8000/api/v1/users/1/
  http://127.0.0.1:8000/api/schema/redoc/
  http://127.0.0.1:8000/api/schema/swagger-ui/
  http://127.0.0.1:8000/api/v1/dj-rest-auth/login/
  http://127.0.0.1:8000/api/v1/dj-rest-auth/logout/
  http://127.0.0.1:8000/api/v1/dj-rest-auth/password/reset/
  http://127.0.0.1:8000/api/v1/dj-rest-auth/password/reset/confirm
  http://127.0.0.1:8000/api/v1/dj-rest-auth/registration/
  ```
- for test
  ```
  (.venv) > python manage.py test
  ```
- for heroku
  ```
  https://aaa-blog-api.herokuapp.com/api/v1/users/
  https://aaa-blog-api.herokuapp.com/api/v1/users/1/
  https://aaa-blog-api.herokuapp.com/api/schema/redoc/
  https://aaa-blog-api.herokuapp.com/api/schema/swagger-ui/
  https://aaa-blog-api.herokuapp.com/api/v1/dj-rest-auth/login/
  https://aaa-blog-api.herokuapp.com/api/v1/dj-rest-auth/logout/
  https://aaa-blog-api.herokuapp.com/api/v1/dj-rest-auth/password/reset/
  https://aaa-blog-api.herokuapp.com/api/v1/dj-rest-auth/password/reset/confirm
  https://aaa-blog-api.herokuapp.com/api/v1/dj-rest-auth/registration/
  
  ```
## Directory Hierarchy
```
|—— .env
|—— .gitattributes
|—— .gitignore
|—— .venv
|—— Procfile
|—— accounts
|    |—— __init__.py
|    |—— __pycache__
|        |—— __init__.cpython-310.pyc
|        |—— admin.cpython-310.pyc
|        |—— apps.cpython-310.pyc
|        |—— forms.cpython-310.pyc
|        |—— models.cpython-310.pyc
|        |—— tests.cpython-310.pyc
|    |—— admin.py
|    |—— apps.py
|    |—— forms.py
|    |—— migrations
|        |—— 0001_initial.py
|        |—— __init__.py
|        |—— __pycache__
|            |—— 0001_initial.cpython-310.pyc
|            |—— __init__.cpython-310.pyc
|    |—— models.py
|    |—— tests.py
|    |—— views.py
|—— db.sqlite3
|—— django_project
|    |—— __init__.py
|    |—— __pycache__
|        |—— __init__.cpython-310.pyc
|        |—— settings.cpython-310.pyc
|        |—— urls.cpython-310.pyc
|        |—— wsgi.cpython-310.pyc
|    |—— asgi.py
|    |—— settings.py
|    |—— urls.py
|    |—— wsgi.py
|—— manage.py
|—— posts
|    |—— __init__.py
|    |—— __pycache__
|        |—— __init__.cpython-310.pyc
|        |—— admin.cpython-310.pyc
|        |—— apps.cpython-310.pyc
|        |—— models.cpython-310.pyc
|        |—— permissions.cpython-310.pyc
|        |—— serializers.cpython-310.pyc
|        |—— tests.cpython-310.pyc
|        |—— urls.cpython-310.pyc
|        |—— views.cpython-310.pyc
|    |—— admin.py
|    |—— apps.py
|    |—— migrations
|        |—— 0001_initial.py
|        |—— __init__.py
|        |—— __pycache__
|            |—— 0001_initial.cpython-310.pyc
|            |—— __init__.cpython-310.pyc
|    |—— models.py
|    |—— permissions.py
|    |—— serializers.py
|    |—— tests.py
|    |—— urls.py
|    |—— views.py
|—— requirements.txt
|—— runtime.txt
|—— schema.yml
|—— schema_dynamic.yaml
|—— screenshots
|    |—— Documentation_Redoc_BlogAPI.png
|    |—— Documentation_Swagger-UI_BlogAPI.png
|    |—— Login_BlogAPI.png
|    |—— Logout_BlogAPI.png
|    |—— PostList_BlogAPI.png
|    |—— Post_Instance_BlogAPI.png
|    |—— Register_BlogAPI.png
|    |—— UserInstance_BlogAPI.png
|    |—— UserList_BlogAPI.png
|—— static
|    |—— .keep
|—— staticfiles
|    |—— staticfiles.json
```
Screenshots
===

Blog API Login
===
![Image text](https://github.com/jocnn/blog_api/blob/main/screenshots/Login_BlogAPI.png)

Blog API Logout
===
![Image text](https://github.com/jocnn/blog_api/blob/main/screenshots/Logout_BlogAPI.png)

Blog API Post Instance
===
![Image text](https://github.com/jocnn/blog_api/blob/main/screenshots/Post_Instance_BlogAPI.png)

Blog API Register
===
![Image text](https://github.com/jocnn/blog_api/blob/main/screenshots/Register_BlogAPI.png)

Blog API User Instance
===
![Image text](https://github.com/jocnn/blog_api/blob/main/screenshots/UserInstance_BlogAPI.png)

Blog API User List
===
![Image text](https://github.com/jocnn/blog_api/blob/main/screenshots/UserList_BlogAPI.png)

Blog API Redoc
===
![Image text](https://github.com/jocnn/blog_api/blob/main/screenshots/Documentation_Redoc_BlogAPI.png)

Blog API Swagger-UI
===
![Image text](https://github.com/jocnn/blog_api/blob/main/screenshots/Documentation_Swagger-UI_BlogAPI.png)
