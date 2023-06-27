# ThaparSummerSchool_2k23 Cheat Sheet

## Step1. Install , create and activate virtualenv<br>

## Step2. Start Django project<br>
```bash
   django-admin startproject <project name>
```
## Step3. Start django app<br>
inside the project folder
```bash
  > cd <project name>
  > python manage.py startapp <app name>
```
## Step4. configuring settings.py<br>
### Step4.1 Add app name to installed apps list<br>

```bash
  > INSTALLED_APPS = [
  >    ....
  >  <app name>
  > ]
```

### Step4.2 Give templates folder path and create folder<br>
```bash
  > import os
  >
  > 'DIRS': [os.path.join(BASE_DIR,'templates')],
```

### Step4.3 Give static folder path and create folder inside the app[important]<br>
```bash
  > STATIC_URL = 'static/'
  > STATIC_ROOT = BASE_DIR / 'static'
  > STATICFILES_DIR = [os.path.join(BASE_DIR, 'static')]
```
## Step5. Configuting the urls.py in project folder<br>
```bash
  > from django.urls import path, include
  >
  > urlpatterns = [
  > ...
  > path('',include('members.urls'))
  > ]
```
## Step6. Create and populate urls.py in app folder<br>

```bash
  > from django.urls import path
  > from . import views
  > urlpatterns = [
  > ...
  > path('',views.index,name='index'),
  > ...
  > ]
```

## Step7. Populate viwes.py in app folder<br>

```bash
  > from django.shortcuts import render
  >
  >def index(request):
  >   #any operations you want to do
  >    return render(request,'graph.html')
```


## Step8> Create and register model <br>

in models.py of app
```bash
  > from pyexpat import model
  > from django.db import models
  >
  > class QUESTION(models.Model):
  >   q1=models.IntegerField(blank=False,default=9)
```

in admin.py of app
```bash
  > from <app name>.models import QUESTION
  > 
  > admin.site.register(QUESTION)
```

## Step9. Collect Static files and Migrate database<br>

```bash
  > python manage.py makemigrations
  > python manage.py migrate
  > 
  > python manage.py collectstatic
```

## Step10. Create SuperUser<br>

```bash
  > python manage.py createsuperuser
```

![admin](https://github.com/harjasdt/ThaparSummerSchool_2k23/assets/68768529/aa3f1dc5-708b-402b-8470-ca051cae866a)


Login by going to the prebuilt django admin panel at  http://127.0.0.1:8000/admin/


![adm](https://github.com/harjasdt/ThaparSummerSchool_2k23/assets/68768529/360dd40c-9907-4245-8437-49ecd9d065cf)


![ad2](https://github.com/harjasdt/ThaparSummerSchool_2k23/assets/68768529/80dd5b48-8c21-4dad-b0d2-a10d9c7048ce)

