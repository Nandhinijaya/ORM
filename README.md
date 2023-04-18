# Ex02 Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a student database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

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
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')

```


## OUTPUT

![Screenshot from 2023-04-18 23-05-15](https://user-images.githubusercontent.com/121998147/232859508-6a11eea3-3322-4611-a57e-c9c75af7d361.png)


## RESULT
Thus the program executed successfully.
