# Ex02 Django ORM Web Application
## Date: 10/10/2023

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
## admin.py
```
from django.contrib import admin
from .models import Player,PlayerAdmin
admin.site.register(Player,PlayerAdmin)
```
## models.py
```
from django.db import models
from django.contrib import admin
class Player(models.Model):
    Player_Name=models.CharField(max_length=50)
    Jersy_No=models.IntegerField()
    Team=models.CharField(max_length=20)
    Height=models.IntegerField()
    Position=models.CharField(max_length=100)

class PlayerAdmin(admin.ModelAdmin):
    list_display=('Player_Name','Jersy_No','Team','Height','Position')
```


## OUTPUT


![2fwddjano](https://github.com/VRVijaykumar123/ORM/assets/133218255/ce29dde1-a81a-4022-a59c-a4c7ee77dc13)





## RESULT
Thus the program for creating a database using ORM hass been executed successfully
