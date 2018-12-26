# 一、安装
```
pip3 install djangorestframework
pip3 install markdown       # Markdown support for the browsable API.
pip3 install django-filter  # Filtering support
```

# 二、配置
Add 'rest_framework' to your INSTALLED_APPS setting.
```
INSTALLED_APPS = (
    ...
    'rest_framework',
)
```
If you're intending to use the browsable API you'll probably also want to add REST framework's login and logout views. Add the following to your root urls.py file.
```
urlpatterns = [
    ...
    url(r'^api-auth/', include('rest_framework.urls'))
]
```

参考文档：

https://www.django-rest-framework.org/#installation