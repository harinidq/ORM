# Ex02 Django ORM Web Application
# AIM
To develop a Django application to store and retrieve data from a student database using Object Relational Mapping(ORM).

# Entity Relationship Diagram
![image](https://user-images.githubusercontent.com/113497680/236613300-47059628-fd7c-42da-bb7a-5c6efabfee7b.png)

# DESIGN STEPS
# STEP 1:
Clone the repository from github.

# STEP 2:
Create an admin interfacefor Django.

# STEP 3:
Create an app and edit settings.py.

# STEP 4:
Makemigrations and migrate the changes.

# STEP 5:
Create admin user and write pythoncode for admin and models.

# STEP 6:
Make all the migrations to 'myapp'.

# STEP 7:
Create an student database with 10 feilds using runserver command.

# PROGRAM
```
admin.py 

from django.contrib import admin
from .models import student,studentAdmin 
admin.site.register(student,studentAdmin)

models.py

from django.db import models
from django.contrib import admin
class student (models.Model):
    sid=models.CharField(max_length=28)
    name=models.CharField(max_length=30)
    regno=models.IntegerField()
    marks=models.IntegerField()
    email=models.EmailField()

class studentAdmin(admin.ModelAdmin):
    list_display=('sid','name','regno','marks','email')

```

# OUTPUT
![image](https://user-images.githubusercontent.com/113497680/236613200-385cfebf-c9b4-43de-9938-0770929acfa6.png)


# RESULT
The code executed successfully
