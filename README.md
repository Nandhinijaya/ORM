# Ex02 Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a student database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

![student admin](https://user-images.githubusercontent.com/121998147/233004622-12bff9f4-e272-41b1-875a-55e165f5e17b.jpg)

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
![exp2 django pic ](https://user-images.githubusercontent.com/121998147/234515460-5bbe1e6f-6abe-442f-a516-9e373804bd51.png)





## RESULT
Thus the program executed successfully.
