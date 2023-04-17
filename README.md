# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from github.


### STEP 2:
Create a new app

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Create django app and add student details.


## PROGRAM
models.py

from django.db import models
from django.contrib import admin

class Student(models.Model):
   referencenumber=models.CharField(primary_key=true,max_length=20,help_text="reference num
   name=models.CharField(max_length=100)
   age=models.IntegerField()
   email=models.EmailField()
   
class StudentAdmin(admin.ModelAdmin):
   list_display=('referencenumber','name','age','email')
   
admin.py
from django.contrib import admin
from myapp.models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin)

## OUTPUT
## SERVER OUTPUT
![django orm](https://user-images.githubusercontent.com/120431120/232536036-b53178f9-99b2-4c34-b103-68c99158580f.jpeg)

## CLIENT OUTPUT
![Screenshot _29_](https://user-images.githubusercontent.com/120431120/232534961-64e433be-f131-4e70-bdc3-7359d98280fc.jpg)

## RESULT
Program executed successfully
