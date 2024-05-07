~~~
 Ex03 Time Table
 Date: 26.3.2024

 AIM
 To write a html webpage page to display your slot timetable.

 ALGORITHM

 STEP 1: Create a Django-admin Interface.
 STEP 2: Create a static folder and inert HTML code.
 STEP 3: Create a simple table using ```<table>``` tag in html.
 STEP 4: Add header row using ```<th>``` tag.
 STEP 5: Add your timetable using ```<td>``` tag.
 STEP 6: Execute the program using runserver command.

PROGRAM

Models.py

from django.db import models
from django.contrib import admin
class Player(models.Model):
    Player_Name=models.CharField(max_length=50)
    Jersy_No=models.IntegerField()
    Team=models.CharField(max_length=20)
    Height=models.IntegerField()
    Position=models.CharField(max_length=100)

class Player_Admin(admin.ModelAdmin):
    list_display=('Player_Name','Jersy_No','Team','Height','Position')

admi.py

from django.contrib import admin
from .models import Player,Player_Admin
admin.site.register(Player,Player_Admin)
~~~
## OUTPUT

![image](https://github.com/niranjanadevi-s/slot/assets/141748873/e6306a0e-4656-42fd-94d9-c0040de2d658)


![image](https://github.com/niranjanadevi-s/slot/assets/141748873/6e092d5e-9fc5-4cfe-a684-565288db84ec)

## RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
