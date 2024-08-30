# IBM-Django-Application-Development-with-SQL-and-Databases
IBM - Django Application Development with SQL and Databases

<p align="center" width="100%">
    <img width="60%" src="https://github.com/jkaewprateep/IBM-Django-Application-Development-with-SQL-and-Databases/blob/main/Django%20Application%20Development%20with%20SQL%20and%20Databases%20-%20instructors.png">
    <img width="20%" src="https://github.com/jkaewprateep/IBM-Django-Application-Development-with-SQL-and-Databases/blob/main/kid_20.jpg"> </br>
    <b> Pictures from the Internet </b> </br>
</p>

[IBM Back-End Development Professional Certificate]( https://github.com/jkaewprateep/Portfolio/blob/main/Coursera%20TFEHPZU2LP6Y.pdf ) </br>
[IBM Front-End Developer Professional Certificate]( https://github.com/jkaewprateep/Portfolio/blob/main/Coursera%206UJS9UQ5T9XV.pdf ) </br>
[IBM Full Stack Software Developer Professional Certificate]( https://github.com/jkaewprateep/Portfolio/blob/main/Coursera%20PNBKLW7T2NED.pdf ) </br>
[Meta Back-End Developer Professional Certificate]( https://github.com/jkaewprateep/Portfolio/blob/main/Coursera%20FANPMLCYFSZ2.pdf ) </br>
[Meta Database Engineer Professional Certificate]( https://github.com/jkaewprateep/Portfolio/blob/main/Coursera%20VVUULL2PK26V.pdf ) </br>
[HackerRank SQL (Advance)]( https://www.hackerrank.com/certificates/f225fa371510 ) </br>
[Board .NET FullStack Developer Specialization]( https://github.com/jkaewprateep/Portfolio/blob/main/Coursera%206DRYK7YS79ZT.pdf ) </br>

## Requirements ##

🧸💬 ```Django``` : Django library, ```Pillow``` : Python image library, ```jinja2``` : Document template library, ```gunicorn```: WSGI HTTP Server, ```contextvars``` : Task asynchronous context variables, ```typing-extensions``` : Python runtime typing extension,
```aiohttp``` : Python HTTP request API, ```click``` : Python CLI interfaces, ```wheel``` : PEP Python Enhancement Proposals, and ```multidict``` : Python dictionary key-pairs library. </br>
🐑💬 ➰ WSGI **standard interface between web applications written in Python and Webservers** is required for Python application programs working with web-server application development by working as a background process and communication for Pythong working language with the pre-complied and complied library. You can compare it with ASP.net web application development that you may be running by ```C#.net``` and ```VB.net``` codes files or you can comply with local library loading with a web application running or target library registration as in .net registration process. As recommendations when there is a problem with the web application server and there is an error message about the WSGI application re-do verify that your ```requirements are all registered```. The configuration working ```directory path``` and configuration ```version are correct```. </br>
🧸💬 ```python-3.8.13``` : run time. </br>

```
Django==3.1.3
Pillow==10.0.0
jinja2==3.0
gunicorn==20.1.0
contextvars
typing-extensions==4.1.1
aiohttp==3.8.3
click==8.0.4
wheel==0.41.1
multidict==4.5
```

## WSGI.py ##

🐑💬 ➰ Similar to application setting or ```program.cs```, where the application initializes and loads the ```required settings``` and ```modules```. In the past, if we needed to create multiple applications, such as ```clients and servers```, from a web application server, we could call from the application program.cs, which is similar to this method where WSGI called the ```registered module``` and ```initialized the value```. ```Class name modification``` here will affect the entire project. </br>
🐐💬 Some applications need to prioritize load order or pass-through value for their process or telecommunications programs may need to identify, or unique numbers at the beginning of the program before software architecture is allowed to create or utilize external queue management applications and services. </br>
🐯 One application receiver, and accepted messages from multiple receivers where they required a dedicated TCP/IP communication port as user requirements, working in a dedicated communication port required a registration process and identifier with identity INFO. </br> 

```
"""
WSGI config for myproject project.

It exposes the WSGI callable as a module-level variable named ``application``.

For more information on this file, see
https://docs.djangoproject.com/en/3.0/howto/deployment/wsgi/
"""

import os

from django.core.wsgi import get_wsgi_application

os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'myproject.settings')

application = get_wsgi_application()
```

## ASGI.py ##

🐑💬 ➰ Asynchronous Server Gateway Interface, similar to WSGI with Python asynchronous process. This approach also implements both ```Python``` and ```.net``` or web applications but they create different effects on the application running behavior because they ```work asynchronous processes```. Working with data applications may not identify problems but registration and priority order programs will need a confirmation process that creates the different behaviors but the working results are from applications in application logic. Working asynchronously capable by ```broadcasting message``` for receiver status when it is ```ready```, in some telecommunication will require one more message tell about the application ready. </br>

```
"""
ASGI config for myproject project.

It exposes the ASGI callable as a module-level variable named ``application``.

For more information on this file, see
https://docs.djangoproject.com/en/3.0/howto/deployment/asgi/
"""

import os

from django.core.asgi import get_asgi_application

os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'myproject.settings')

application = get_asgi_application()
```

## settings.py ##

🦭💬 Application settings, connection settings, registered application and modules, dynamic values and statics values, templates document, and application you want to load after the application initially started. </br>
🦁💬 Security applied to the application or application running engine should collected into one place as a ```statics file``` or ```database table```, manageable and secured with protection by system access of their policy requirements with standard re-configuration, the effect from change setting can determine for benefits of applied configuration and notification monitoring. </br>

```
"""
Django settings for myproject project.

Generated by 'django-admin startproject' using Django 3.0.4.

For more information on this file, see
https://docs.djangoproject.com/en/3.0/topics/settings/

For the full list of settings and their values, see
https://docs.djangoproject.com/en/3.0/ref/settings/
"""

import os


# Build paths inside the project like this: os.path.join(BASE_DIR, ...)
BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))


# Quick-start development settings - unsuitable for production
# See https://docs.djangoproject.com/en/3.0/howto/deployment/checklist/

# SECURITY WARNING: keep the secret key used in production secret!
SECRET_KEY = 'aay0j_9b&ky3a7(8m8il+-1ud(scw12@w5!+5-=gsk6ynzi0ls'

# SECURITY WARNING: don't run with debug turned on in production!
DEBUG = True

ALLOWED_HOSTS = []


# Application definition

INSTALLED_APPS = [
    'onlinecourse.apps.OnlinecourseConfig',
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
]

MIDDLEWARE = [
    'django.middleware.security.SecurityMiddleware',
    'django.contrib.sessions.middleware.SessionMiddleware',
    'django.middleware.common.CommonMiddleware',
    'django.middleware.csrf.CsrfViewMiddleware',
    'django.contrib.auth.middleware.AuthenticationMiddleware',
    'django.contrib.messages.middleware.MessageMiddleware',
    'django.middleware.clickjacking.XFrameOptionsMiddleware',
]

ROOT_URLCONF = 'myproject.urls'

TEMPLATES = [
    {
        'BACKEND': 'django.template.backends.django.DjangoTemplates',
        'DIRS': [],
        'APP_DIRS': True,
        'OPTIONS': {
            'context_processors': [
                'django.template.context_processors.debug',
                'django.template.context_processors.request',
                'django.contrib.auth.context_processors.auth',
                'django.template.context_processors.media',
                'django.contrib.messages.context_processors.messages',
            ],
        },
    },
]

WSGI_APPLICATION = 'myproject.wsgi.application'


# Database
# https://docs.djangoproject.com/en/3.0/ref/settings/#databases

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
    }
}


# Password validation
# https://docs.djangoproject.com/en/3.0/ref/settings/#auth-password-validators

AUTH_PASSWORD_VALIDATORS = [
    {
        'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',
    },
    {
        'NAME': 'django.contrib.auth.password_validation.MinimumLengthValidator',
    },
    {
        'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator',
    },
    {
        'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator',
    },
]


# Internationalization
# https://docs.djangoproject.com/en/3.0/topics/i18n/

LANGUAGE_CODE = 'en-us'

TIME_ZONE = 'UTC'

USE_I18N = True

USE_L10N = True

USE_TZ = True


# Static files (CSS, JavaScript, Images)
# https://docs.djangoproject.com/en/3.0/howto/static-files/

STATIC_URL = '/static/'
STATIC_ROOT = os.path.join(BASE_DIR, 'static')
MEDIA_ROOT = os.path.join(STATIC_ROOT, 'media')
MEDIA_URL = '/media/'
```

## urls.py ##

🐑💬 ➰ It is a global routes table to target addresses, paths, views, applications, and resources. </br>
👧💬 🎈 Global routes working for internal and external addresses as you may experience with proxy-server ```NGIX``` . I like this proxy application because it allows communication with application filters, message responses, and communication path configuration from the same source of TCP/IP communication and HTTP communication address. The routes table and  proxy allowed to communication filter message or working with installed application similar to firewall or network packets analysis applications for software and hardware. </br>
👧💬 🎈 Better global routes working with applications, views, and internal modules. </br>

```
"""myproject URL Configuration

The `urlpatterns` list routes URLs to views. For more information please see:
    https://docs.djangoproject.com/en/3.0/topics/http/urls/
Examples:
Function views
    1. Add an import:  from my_app import views
    2. Add a URL to urlpatterns:  path('', views.home, name='home')
Class-based views
    1. Add an import:  from other_app.views import Home
    2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
Including another URLconf
    1. Import the include() function: from django.urls import include, path
    2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
"""
from django.contrib import admin
from django.urls import include, path
from django.conf.urls.static import static
from django.conf import settings

urlpatterns = [
    path('admin/', admin.site.urls),
    path('onlinecourse/', include('onlinecourse.urls')),
] + static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)\
 + static(settings.STATIC_URL, document_root=settings.STATIC_ROOT)
```

## # Lab - 1 ##

## # Lab - 2 ##

## # Lab - 3 ##


---

<p align="center" width="100%">
    <img width="30%" src="https://github.com/jkaewprateep/advanced_mysql_topics_notes/blob/main/custom_dataset.png">
    <img width="30%" src="https://github.com/jkaewprateep/advanced_mysql_topics_notes/blob/main/custom_dataset_2.png"> </br>
    <b> 🥺💬 รับจ้างเขียน functions </b> </br>
</p>
