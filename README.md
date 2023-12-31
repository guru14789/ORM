# Ex02 Django ORM Web Application
## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).
## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM:
## models.py
```
from django.db import models
from django.contrib import admin
class Football_Player(models.Model):
    player_name=models.CharField(max_length=20)
    player_age=models.IntegerField()
    team_name=models.CharField(max_length=20)
    player_position=models.CharField(max_length=20)
    player_jersey_no=models.IntegerField()
class Football_PlayerAdmin(admin.ModelAdmin):
    list_display=('player_name','player_age','team_name','player_position','player_jersey_no')  
```
## admin.py
```
from django.contrib import admin
from .models import Football_Player,Football_PlayerAdmin
admin.site.register(Football_Player,Football_PlayerAdmin)
```

## OUTPUT:
![Screenshot 2023-12-31 202552](https://github.com/guru14789/ORM/assets/151705853/33550077-8637-412c-b5b8-5080a96600e6)

## RESULT:
Thus the program for creating a database using ORM hass been executed successfully
