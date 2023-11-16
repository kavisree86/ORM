# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM
Models.py

from django.db import models
from django.contrib import admin
class Players(models.Model):
    pid=models.CharField(max_length=20,help_text="Player ID")
    name=models.CharField(max_length=100)
    team=models.CharField(max_length=50)
    age=models.IntegerField()
    rating=models.IntegerField()

class PlayerAdmin(admin.ModelAdmin):
    list_display=('pid','name','team','age','rating')

admin.py

from django.contrib import admin
from .models import Players,PlayerAdmin
admin.site.register(Players,PlayerAdmin)



## OUTPUT

%![Screenshot (2)](https://github.com/kavisree86/ORM/assets/145759687/6f0a4a9b-1c43-44f8-be9d-d7e3c01691c3)
20(2).png)
Include the screenshot of your admin page.


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
