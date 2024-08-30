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

## apps.py ##

🦁💬 Application configuration data for application and subclasses import, asynchronize application running need to compose of identification method or the number of application instance object, an application running and update working task progress where user status and message communication carry information data synchronize process and support of calling by asynchronize process as events. Deploy applications in ```app.py``` or ```WSGI application``` or ```native application``` need consideration for programming code transforming because application behavior, priority order, status update, and communication methods are different. </br>     
🧸💬 Application code migration is aware of this problem by working at the library level, queue message, identification identity for application working threads, and overall process monitoring and statistical reports because it is easier in code migration. For web applications asynchronized applications can have multiple message and events handling methods especially with telecommunication programs but with the Django application platform message communication is built with events status support, application, and user attributes and works with web appliation by utilizing the same message communication object that is fast and easy. </br>

```
from django.apps import AppConfig


class OnlinecourseConfig(AppConfig):
    name = 'onlinecourse'
```

## models.py ##

🐑💬 ➰ Data model with data table fields, relationship, column definition, default values, foreign key, primary key, null enabled value, user define values, and authentication if applicable. </br>
🐯💬 By data table and database definition encoding and Culture-INFO, the model and application can apply logical functions for data validation or data transformation for datetime, running number, verification key, and encoding value but they have significant usages. By applying the configuration settings and text format ```culture INFO``` at the database and database table the database or data management services will validate data and return the data insertion, modification, update, or delete results with the same communication method invoke the method but it is working at the database level and application need to handle or the insertion errors and modification by themself. When data model validation you can handle with codes and have instance response with specific information and utilize the same connection and working process for handling the insertion errors also the application when it is running asynchronously can multiply access or utilize the ```database connection management services``` or use of building database connection management services such as ```MongoDB``` or ```Message queue management```. </br>
🦭💬 Define the data model as a class similar to the dataset class so that we can create a build-in function for internal logic and exchange values with ```security method protection```. Working with the standard level the data model or classes will not exposed but the data requirements are with a ```description``` where ```calculation fields``` or ```integration values``` are internal programming logics. </br>

```
import sys
from django.utils.timezone import now
try:
    from django.db import models
except Exception:
    print("There was an error loading django modules. Do you have django installed?")
    sys.exit()

from django.conf import settings
import uuid


# Instructor model
class Instructor(models.Model):
    user = models.ForeignKey(
        settings.AUTH_USER_MODEL,
        on_delete=models.CASCADE,
    )
    full_time = models.BooleanField(default=True)
    total_learners = models.IntegerField()

    def __str__(self):
        return self.user.username


# Learner model
class Learner(models.Model):
    user = models.ForeignKey(
        settings.AUTH_USER_MODEL,
        on_delete=models.CASCADE,
    )
    STUDENT = 'student'
    DEVELOPER = 'developer'
    DATA_SCIENTIST = 'data_scientist'
    DATABASE_ADMIN = 'dba'
    OCCUPATION_CHOICES = [
        (STUDENT, 'Student'),
        (DEVELOPER, 'Developer'),
        (DATA_SCIENTIST, 'Data Scientist'),
        (DATABASE_ADMIN, 'Database Admin')
    ]
    occupation = models.CharField(
        null=False,
        max_length=20,
        choices=OCCUPATION_CHOICES,
        default=STUDENT
    )
    social_link = models.URLField(max_length=200)

    def __str__(self):
        return self.user.username + "," + \
               self.occupation


# Course model
class Course(models.Model):
    name = models.CharField(null=False, max_length=30, default='online course')
    image = models.ImageField(upload_to='course_images/')
    description = models.CharField(max_length=1000)
    pub_date = models.DateField(null=True)
    instructors = models.ManyToManyField(Instructor)
    users = models.ManyToManyField(settings.AUTH_USER_MODEL, through='Enrollment')
    total_enrollment = models.IntegerField(default=0)
    is_enrolled = False

    def __str__(self):
        return "Name: " + self.name + "," + \
               "Description: " + self.description


# Lesson model
class Lesson(models.Model):
    title = models.CharField(max_length=200, default="title")
    order = models.IntegerField(default=0)
    course = models.ForeignKey(Course, on_delete=models.CASCADE)
    content = models.TextField()


# Enrollment model
class Enrollment(models.Model):
    AUDIT = 'audit'
    HONOR = 'honor'
    BETA = 'BETA'
    COURSE_MODES = [
        (AUDIT, 'Audit'),
        (HONOR, 'Honor'),
        (BETA, 'BETA')
    ]
    user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
    course = models.ForeignKey(Course, on_delete=models.CASCADE)
    date_enrolled = models.DateField(default=now)
    mode = models.CharField(max_length=5, choices=COURSE_MODES, default=AUDIT)
    rating = models.FloatField(default=5.0)
```

## test.py ##

🐑💬 ➰ To perform Python test functions, or included libraries such as RobotFrameworks, Selenium, and many automation test applications. </br> 

```
from django.test import TestCase

# Create your tests here.
```

## views.py ##

🐑💬 ➰ The class ```CourseDetailsView``` inherits of class ```generic.DetailView``` with create a new definition ```get``` to render return context into ```onlinecourse/course_detail.html``` . </br> 
🐑💬 ➰ The class ```EnrollView``` inherits of class ```View``` import from ```django.views``` with create a new definition ```post``` to return by redirect to ```course_details``` with argrument ```course.id``` . </br> 

```
from django.shortcuts import render
from django.http import HttpResponse, HttpResponseRedirect
from django.shortcuts import get_object_or_404, render, redirect
from .models import Course, Lesson, Enrollment
from django.urls import reverse
from django.views import generic, View
from django.http import Http404

# Create your class based views here.
# Note that we are subclassing CourseListView from base View class
# Note that CourseDetailsView is now subclassing DetailView 
class CourseDetailsView(generic.DetailView):
    model = Course
    template_name = 'onlinecourse/course_detail.html'

    # Handles get request
    def get(self, request, *args, **kwargs):
        context = {}
        # We get URL parameter pk from keyword argument list as course_id
        course_id = kwargs.get('pk')
        try:
            course = Course.objects.get(pk=course_id)
            context['course'] = course
            return render(request, 'onlinecourse/course_detail.html', context)
        except Course.DoesNotExist:
            raise Http404("No course matches the given id.")

class EnrollView(View):

    # Handles post request
    def post(self, request, *args, **kwargs):
        course_id = kwargs.get('pk')
        course = get_object_or_404(Course, pk=course_id)
        # Increase total enrollment by 1
        course.total_enrollment += 1
        course.save()
        return HttpResponseRedirect(reverse(viewname='onlinecourse:course_details', args=(course.id,)))

# Note that CourseListView is subclassing from generic.ListView instead of View
# so that it can use attributes and override methods from ListView such as get_queryset()
class CourseListView(generic.ListView):
    template_name = 'onlinecourse/course_list.html'
    context_object_name = 'course_list'

    # Override get_queryset() to provide list of objects
    def get_queryset(self):
       courses = Course.objects.order_by('-total_enrollment')[:10]
       return courses

# Function based views

# Function-based course list view
# def popular_course_list(request):
#    context = {}
#    if request.method == 'GET':
#        course_list = Course.objects.order_by('-total_enrollment')[:10]
#        context['course_list'] = course_list
#        return render(request, 'onlinecourse/course_list_no_css.html', context)

# Function-based course_details view
# def course_details(request, course_id):
#    context = {}
#    if request.method == 'GET':
#        try:
#            course = Course.objects.get(pk=course_id)
#            context['course'] = course
#            return render(request, 'onlinecourse/course_detail.html', context)
#        except Course.DoesNotExist:
#            raise Http404("No course matches the given id.")

# Function-based enroll view
# def enroll(request, course_id):
#    if request.method == 'POST':
#       course = get_object_or_404(Course, pk=course_id)
#       # Create an enrollment
#       course.total_enrollment += 1
#       course.save()
#       return HttpResponseRedirect(reverse(viewname='onlinecourse:course_details', args=(course.id,)))
```

## # Lab - 1 ##

### course.css ###

🐑💬 ➰ HTML style sheet .css with filter and action ```.row:after```, ```input[type=text]:focus, input[type=password]:focus```, and ```.dropdown:hover``` </br>
🥺💬 Nice question when you need to create interactive user control without building them as a user control interface with script manager, javascript with embedded pictures, local library, COM API, etc. </br>
🐯💬 ```Culture-INFO``` data management services should handle data when user interaction services have multiple of user interaction controls, data services team knows about the user interaction but by design, the data should perform at the data communication level before transmitted, and the user interface display of the data with less of effort for ```data manipulation``` and should not access by the background working process that creates ```background infomration loop problem``` . </br>

```
body {font-family: Arial, Helvetica, sans-serif;}
* {box-sizing: border-box}


/* Add a gray background color with some padding */
body {
  font-family: Arial;
  padding: 10px;
  background: #ececec;
}

/* Header/Blog Title */
.header {
  padding: 30px;
  font-size: 40px;
  text-align: center;
  background: white;
}


/* Create two unequal columns that floats next to each other */
/* Left column */
.leftcolumn {
  float: left;
  width: 75%;
}

/* Right column */
.rightcolumn {
  float: left;
  width: 25%;
  padding-left: 20px;
}

/* Fake image */
.fakeimg {
  background-color: #aaa;
  width: 100%;
  padding: 20px;
}

/* Add a card effect for articles */
.card {
   background-color: white;
   padding: 20px;
   margin-top: 20px;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Footer */
.footer {
  padding: 20px;
  text-align: center;
  background: #ddd;
  margin-top: 20px;
}

/* Responsive layout - when the screen is less than 800px wide, make the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 800px) {
  .leftcolumn, .rightcolumn {
    width: 100%;
    padding: 0;
  }
}


.button {
  border: none;
  color: white;
  padding: 14px 28px;
  font-size: 16px;
  cursor: pointer;
  background-color: #005493;
}

.container {
  padding: 64px;
}

.small-container {
  padding: 16px;
}

.rightalign {
    float: right;
}


.column {
  float: left;
  width: 33.33%;
  padding: 5px;
}


/* 2/3 column */
.column-66 {
  float: left;
  width: 66.66666%;
  padding: 20px;
}

/* 1/3 column */
.column-33 {
  float: left;
  width: 33.33333%;
  padding: 20px;
}

/* Add responsiveness - make the columns appear on top of each other instead of next to each other on small screens */
@media screen and (max-width: 1000px) {
  .column-66,
  .column-33 {
    width: 100%;
    text-align: center;
  }
}

/* Full-width input fields */
input[type=text], input[type=password] {
  width: 100%;
  padding: 15px;
  margin: 5px 0 22px 0;
  display: inline-block;
  border: none;
  background: #dadfe1;
}

input[type=text]:focus, input[type=password]:focus {
  background-color: #ddd;
  outline: none;
}

.red{
    color:red
}

.dropbtn {
  background-color: #005493;
  color: white;
  padding: 16px;
  font-size: 16px;
  border: none;
}

.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f1f1f1;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

.dropdown-content a:hover {background-color: #ddd;}

.dropdown:hover .dropdown-content {display: block;}

.dropdown:hover .dropbtn {background-color: darkblue;}
```

### course_detail.html ###

🐑💬 ➰ Iterative of results set to return over the integration scopes of the target application, running of integration method support of for loop and simple aggregate functions. </br>
🥺💬 I submitted my javascript, react.js assignment with ```!``` existence condition for integration fields but I had some feedback about using javascript rather than fixed value variables. </br>
🦭💬 There is always have if then may assign conditions as promised but it may transform as in ```C language``` or ```syntax``` to warn you about the coding style or expected coding behavior. </br>

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    {% load static %}
    <link rel="stylesheet" type="text/css" href="{% static 'onlinecourse/course.css' %}">
</head>
<body>
    <div class="card">
        <h2>{{ course.name }}</h2>
        <h5>{{ course.description }}</h5>
    </div>
    <h2>Lessons: </h2>
    {% for lesson in course.lesson_set.all %}
    <div class="card">
        <h5>Lesson {{lesson.order}} : {{lesson.title}}</h5>
        <p>{{lesson.content}}</p>
    </div>
    {% endfor %}
</body>
</html>
```

### course_list.html ###

🐑💬 ➰ More than data population you can perform module functions from the HTML element by the integration script area and correct syntax, this allows you to create interaction response elements on the web page without creating ```a script manager``` for each integration area or they are create ```integration area``` as the script manager do it for you. </br>
🦭💬 Create ```a category``` or ```table of contents``` with images banner by the ```for loop iterations``` and ```dynamics content``` . </br>

```
<!DOCTYPE html>
<html lang="en">
<head>
    {% load static %}
    <link rel="stylesheet" type="text/css" href="{% static 'onlinecourse/course.css' %}">
    <meta charset="UTF-8">
    <title>Online Courses</title>
</head>
<body>
<h2>Popular courses list</h2>
<hr>
{% if course_list %}
    <ul>
    {% for course in course_list %}
        <div class="container">
          <div class="row">
              <div class="column-33">
                <img src="{{MEDIA_URL}}/{{ course.image }}" width="360" height="360" >
            </div>
            <div class="column-66">
                <h1 class="xlarge-font"><b>{{ course.name }}</b></h1>
                <p style="color:MediumSeaGreen;"><b>{{course.total_enrollment}} enrolled</b></p>
                <p> {{ course.description }}</p>
                <form action="{% url 'onlinecourse:enroll' course.id %}" method="post">
                    {% csrf_token %}
                <input class="button"  type="submit"  value="Enroll">
              </form>
            </div>
          </div>
        </div>
        <hr>
    {% endfor %}
    </ul>
{% else %}
    <p>No courses are available.</p>
{% endif %}
</body>
</html>
```

## # Lab - 2 ##

### models.py ###

```
import sys
from django.utils.timezone import now
try:
    from django.db import models
except Exception:
    print("There was an error loading django modules. Do you have django installed?")
    sys.exit()

from django.conf import settings
import uuid


# Instructor model
class Instructor(models.Model):
    user = models.ForeignKey(
        settings.AUTH_USER_MODEL,
        on_delete=models.CASCADE,
    )
    full_time = models.BooleanField(default=True)
    total_learners = models.IntegerField()

    def __str__(self):
        return self.user.username


# Learner model
class Learner(models.Model):
    user = models.ForeignKey(
        settings.AUTH_USER_MODEL,
        on_delete=models.CASCADE,
    )
    STUDENT = 'student'
    DEVELOPER = 'developer'
    DATA_SCIENTIST = 'data_scientist'
    DATABASE_ADMIN = 'dba'
    OCCUPATION_CHOICES = [
        (STUDENT, 'Student'),
        (DEVELOPER, 'Developer'),
        (DATA_SCIENTIST, 'Data Scientist'),
        (DATABASE_ADMIN, 'Database Admin')
    ]
    occupation = models.CharField(
        null=False,
        max_length=20,
        choices=OCCUPATION_CHOICES,
        default=STUDENT
    )
    social_link = models.URLField(max_length=200)

    def __str__(self):
        return self.user.username + "," + \
               self.occupation


# Course model
class Course(models.Model):
    name = models.CharField(null=False, max_length=30, default='online course')
    image = models.ImageField(upload_to='course_images/')
    description = models.CharField(max_length=1000)
    pub_date = models.DateField(null=True)
    instructors = models.ManyToManyField(Instructor)
    users = models.ManyToManyField(settings.AUTH_USER_MODEL, through='Enrollment')
    total_enrollment = models.IntegerField(default=0)
    is_enrolled = False

    def __str__(self):
        return "Name: " + self.name + "," + \
               "Description: " + self.description


# Lesson model
class Lesson(models.Model):
    title = models.CharField(max_length=200, default="title")
    order = models.IntegerField(default=0)
    course = models.ForeignKey(Course, on_delete=models.CASCADE)
    content = models.TextField()


# Enrollment model
class Enrollment(models.Model):
    AUDIT = 'audit'
    HONOR = 'honor'
    BETA = 'BETA'
    COURSE_MODES = [
        (AUDIT, 'Audit'),
        (HONOR, 'Honor'),
        (BETA, 'BETA')
    ]
    user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
    course = models.ForeignKey(Course, on_delete=models.CASCADE)
    date_enrolled = models.DateField(default=now)
    mode = models.CharField(max_length=5, choices=COURSE_MODES, default=AUDIT)
    rating = models.FloatField(default=5.0)
```

### views.py ###

```
from django.shortcuts import render
from django.http import HttpResponse, HttpResponseRedirect
from .models import Course, Lesson, Enrollment
from django.contrib.auth.models import User
from django.shortcuts import get_object_or_404, render, redirect
from django.http import Http404
from django.urls import reverse
from django.views import generic, View
from collections import defaultdict
from django.contrib.auth import login, logout, authenticate
import logging
# Get an instance of a logger
logger = logging.getLogger(__name__)

# Create authentication related views
def logout_request(request):
    # Get the user object based on session id in request
    print("Log out the user `{}`".format(request.user.username))
    # Logout user in the request
    logout(request)
    # Redirect user back to course list view
    return redirect('onlinecourse:popular_course_list')


# Add a class-based course list view
class CourseListView(generic.ListView):
    template_name = 'onlinecourse/course_list.html'
    context_object_name = 'course_list'

    def get_queryset(self):
       courses = Course.objects.order_by('-total_enrollment')[:10]
       return courses


# Add a generic course details view
class CourseDetailsView(generic.DetailView):
    model = Course
    template_name = 'onlinecourse/course_detail.html'


class EnrollView(View):

    # Handles get request
    def post(self, request, *args, **kwargs):
        course_id = kwargs.get('pk')
        course = get_object_or_404(Course, pk=course_id)
        # Create an enrollment
        course.total_enrollment += 1
        course.save()
        return HttpResponseRedirect(reverse(viewname='onlinecourse:course_details', args=(course.id,)))

def login_request(request):
    context = {}
    # Handles POST request
    if request.method == "POST":
        # Get username and password from request.POST dictionary
        username = request.POST['username']
        password = request.POST['psw']
        # Try to check if provide credential can be authenticated
        user = authenticate(username=username, password=password)
        if user is not None:
            # If user is valid, call login method to login current user
            login(request, user)
            return redirect('onlinecourse:popular_course_list')
        else:
            # If not, return to login page again
            return render(request, 'onlinecourse/user_login.html', context)
    else:
        return render(request, 'onlinecourse/user_login.html', context)

def registration_request(request):
    context = {}
    # If it is a GET request, just render the registration page
    if request.method == 'GET':
        return render(request, 'onlinecourse/user_registration.html', context)
    # If it is a POST request
    elif request.method == 'POST':
        # Get user information from request.POST
        username = request.POST['username']
        password = request.POST['psw']
        first_name = request.POST['firstname']
        last_name = request.POST['lastname']
        user_exist = False
        try:
            # Check if user already exists
            User.objects.get(username=username)
            user_exist = True
        except:
            # If not, simply log this is a new user
            logger.debug("{} is new user".format(username))
        # If it is a new user
        if not user_exist:
            # Create user in auth_user table
            user = User.objects.create_user(username=username, first_name=first_name, last_name=last_name,
                                            password=password)
            # Login the user and redirect to course list page
            login(request, user)
            return redirect("onlinecourse:popular_course_list")
        else:
            return render(request, 'onlinecourse/user_registration.html', context)
```

### urls.py ###

```
from django.urls import path
from django.conf import settings
from django.conf.urls.static import static
from . import views

app_name = 'onlinecourse'
urlpatterns = [

    path(route='course/<int:pk>/enroll/', view=views.EnrollView.as_view(), name='enroll'),
    path(route='', view=views.CourseListView.as_view(), name='popular_course_list'),
    path(route='course/<int:pk>/', view=views.CourseDetailsView.as_view(), name='course_details'),
    # Authentication related urls
	path('logout/', views.logout_request, name='logout'),
    path('login/', views.login_request, name='login'),
    path('registration/', views.registration_request, name='registration'),

] + static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)\
 + static(settings.STATIC_URL, document_root=settings.STATIC_ROOT)
```

### course_detail.html ###

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    {% load static %}
    <link rel="stylesheet" type="text/css" href="{% static 'onlinecourse/course.css' %}">
</head>
<body>
    <div class="card">
        <h2>{{ course.name }}</h2>
        <h5>{{ course.description }}</h5>
    </div>
    <h2>Lessons: </h2>
    {% for lesson in course.lesson_set.all %}
    <div class="card">
        <h5>Lesson {{lesson.order}} : {{lesson.title}}</h5>
        <p>{{lesson.content}}</p>
    </div>
    {% endfor %}
</body>
</html>
```

### course_list.html ###

```
<!DOCTYPE html>
<html lang="en">
<head>
    {% load static %}
    <link rel="stylesheet" type="text/css" href="{% static 'onlinecourse/course.css' %}">
    <meta charset="UTF-8">
    <title>Online Courses</title>
</head>
<body>
<!--Authentication section-->
{% if user.is_authenticated %}
    <div class="rightalign">
        <div class="dropdown">
            <button class="dropbtn">{{user.first_name}}</button>
            <div class="dropdown-content">
                <a href="{% url 'onlinecourse:logout' %}">Logout</a>
            </div>
        </div>
    </div>
    {% else %}
    <div class="rightalign">
        <div class="dropdown">
            <form action="{% url 'onlinecourse:registration' %}" method="get">
                <input class="dropbtn"  type="submit" value="Visitor">
                <div class="dropdown-content">
                    <a href="{% url 'onlinecourse:registration' %}">Signup</a>
                    <a href="{% url 'onlinecourse:login' %}">Login</a>
                </div>
            </form>
        </div>
    </div>
{% endif %}

<h2>Popular courses list</h2>
<hr>
{% if course_list %}
    <ul>
    {% for course in course_list %}
        <div class="container">
          <div class="row">
              <div class="column-33">
                <img src="{{MEDIA_URL}}/{{ course.image }}" width="360" height="360" >
            </div>
            <div class="column-66">
                <h1 class="xlarge-font"><b>{{ course.name }}</b></h1>
                <p style="color:MediumSeaGreen;"><b>{{course.total_enrollment}} enrolled</b></p>
                <p> {{ course.description }}</p>
                <form action="{% url 'onlinecourse:enroll' course.id %}" method="post">
                    {% csrf_token %}
                <input class="button"  type="submit"  value="Enroll">
              </form>
            </div>
          </div>
        </div>
        <hr>
    {% endfor %}
    </ul>
{% else %}
    <p>No courses are available.</p>
{% endif %}
</body>
</html>
```

### user_login.html ###

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    {% load static %}
    <link rel="stylesheet" type="text/css" href="{% static 'onlinecourse/course.css' %}">
</head>
<body>
<!--- Add a login form here  --->
<form action="{% url 'onlinecourse:login' %}"  method="post">
    {% csrf_token %}
    <div class="container">
      <h1>Login</h1>
      <label for="username"><b>User Name</b></label>
      <input type="text" placeholder="Enter User Name: " name="username" required>
      <label for="psw"><b>Password</b></label>
      <input type="password" placeholder="Enter Password: " name="psw" required>
      <div>
        <button class="button" type="submit">Login</button>
      </div>
    </div>
  </form>
</body>
```

### user_registration.html ###

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    {% load static %}
    <link rel="stylesheet" type="text/css" href="{% static 'onlinecourse/course.css' %}">
</head>
<body>
<!--- Add a registration form here  --->
<form action="{% url 'onlinecourse:registration' %}" method="post">
    <div class="container">
      <h1>Sign Up</h1>
      <hr>
      <label for="username"><b>User Name</b></label>
      <input type="text" placeholder="Enter User Name: " name="username" required>
      <label for="firstname"><b>First Name</b></label>
      <input type="text" placeholder="Enter First Name: " name="firstname" required>
      <label for="lastname"><b>Last Name</b></label>
      <input type="text" placeholder="Enter Last Name: " name="lastname" required>
      <label for="psw"><b>Password</b></label>
      <input type="password" placeholder="Enter Password: " name="psw" required>
      <div>
          {% csrf_token %}
          <button class="button" type="submit">Sign Up</button>
      </div>
    </div>
  </form>
</body>
```

## # Lab - 3 ##

### views.py ### 
- update context

```
from django.shortcuts import render
from django.http import HttpResponse, HttpResponseRedirect
from .models import Course, Lesson, Enrollment
from django.contrib.auth.models import User
from django.shortcuts import get_object_or_404, render, redirect
from django.http import Http404
from django.urls import reverse
from django.views import generic, View
from collections import defaultdict
from django.contrib.auth import login, logout, authenticate
import logging
# Get an instance of a logger
logger = logging.getLogger(__name__)

# Create your views here.

# Create authentication related views


def registration_request(request):
    context = {}
    if request.method == 'GET':
        return render(request, 'onlinecourse/user_registration.html', context)
    elif request.method == 'POST':
        # Check if user exists
        username = request.POST['username']
        password = request.POST['psw']
        first_name = request.POST['firstname']
        last_name = request.POST['lastname']
        user_exist = False
        try:
            User.objects.get(username=username)
            user_exist = True
        except:
            logger.debug("{} is new user".format(username))
        if not user_exist:
            user = User.objects.create_user(username=username, first_name=first_name, last_name=last_name,
                                            password=password)
            login(request, user)
            return redirect("onlinecourse:popular_course_list")
        else:
            context['message'] = "User already exists."
            return render(request, 'onlinecourse/user_registration.html', context)


def login_request(request):
    context = {}
    if request.method == "POST":
        username = request.POST['username']
        password = request.POST['psw']
        user = authenticate(username=username, password=password)
        print(user)
        if user is not None:
            login(request, user)
            return redirect('onlinecourse:popular_course_list')
        else:
            context['message'] = "Invalid username or password."
            return render(request, 'onlinecourse/user_login.html', context)
    else:
        return render(request, 'onlinecourse/user_login.html', context)


def logout_request(request):
    logout(request)
    return redirect('onlinecourse:popular_course_list')


# Add a class-based course list view
class CourseListView(generic.ListView):
    template_name = 'onlinecourse/course_list.html'
    context_object_name = 'course_list'

    def get_queryset(self):
       courses = Course.objects.order_by('-total_enrollment')[:10]
       return courses


# Add a generic course details view
class CourseDetailsView(generic.DetailView):
    model = Course
    template_name = 'onlinecourse/course_detail.html'


class EnrollView(View):

    # Handles get request
    def post(self, request, *args, **kwargs):
        course_id = kwargs.get('pk')
        course = get_object_or_404(Course, pk=course_id)
        # Create an enrollment
        course.total_enrollment += 1
        course.save()
        return HttpResponseRedirect(reverse(viewname='onlinecourse:course_details', args=(course.id,)))
```

### urls.py ###
- update logout

```
from django.urls import path
from django.conf import settings
from django.conf.urls.static import static
from . import views

app_name = 'onlinecourse'
urlpatterns = [

    path(route='course/<int:pk>/enroll/', view=views.EnrollView.as_view(), name='enroll'),
    path(route='', view=views.CourseListView.as_view(), name='popular_course_list'),
    path(route='course/<int:pk>/', view=views.CourseDetailsView.as_view(), name='course_details'),

    # Authentication related urls
    path('registration/', views.registration_request, name='registration'),
    path('login/', views.login_request, name='login'),
    path('logout/', views.logout_request, name='logout'),

] + static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)\
 + static(settings.STATIC_URL, document_root=settings.STATIC_ROOT)
```

### Navigation bar - navbar navbar-light ###

```
<nav class="navbar navbar-light bg-light">
    <div class="container-fluid">
        <div class="navbar-header">
            <a class="navbar-brand" href="#">Online Course</a>
        </div>
        <ul class="nav navbar-nav navbar-right">
            {% if user.is_authenticated %}
            <li>
                <a class="btn btn-link" href="#">{{ user.first_name }}({{ user.username }})</a>
                <a class="btn btn-link" href="{% url 'onlinecourse:logout' %}">Logout</a>
            </li>
            {% else %}
            <li>
                <form class="form-inline" action="{% url 'onlinecourse:login' %}" method="post">
                    {% csrf_token %}
                    <div class="input-group">
                        <input type="text" class="form-control" placeholder="Username" name="username" >
                        <input type="password" class="form-control" placeholder="Password" name="psw" >
                        <button class="btn btn-primary" type="submit">Login</button>
                        <a class="btn btn-link" href="{% url 'onlinecourse:registration' %}">Sign Up</a>
                    </div>
                </form>
            </li>
            {% endif %}
        </ul>
    </div>
</nav>
```

---

<p align="center" width="100%">
    <img width="30%" src="https://github.com/jkaewprateep/advanced_mysql_topics_notes/blob/main/custom_dataset.png">
    <img width="30%" src="https://github.com/jkaewprateep/advanced_mysql_topics_notes/blob/main/custom_dataset_2.png"> </br>
    <b> 🥺💬 รับจ้างเขียน functions </b> </br>
</p>
