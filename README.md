# Ex02 Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a student database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

![student](https://user-images.githubusercontent.com/121998147/234515928-8b4604ec-aa54-41a9-af78-d6fb09a508a2.jpg)

## DESIGN STEPS

### STEP 1:
Give the input programs
### STEP 2:
Folloe the given steps
### STEP 3:
End the program


## PROGRAM
```
admin.py
from django.contrib import admin
from .models import Student,StudentAdmin
# Register your models here.

admin.site.register(Student,StudentAdmin)

models.py
from django.db import models
from django.contrib import admin
# Create your models here.
class Student (models.Model):
    rollno=models.IntegerField(primary_key=True,max_length=20,help_text="rollno")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('rollno','name','age','email')

```


## OUTPUT
![employee](https://user-images.githubusercontent.com/121998147/234511093-0e89f19f-f9a8-49e4-86f5-4120ef07cf73.jpg)




## RESULT
Thus the program executed successfully.
