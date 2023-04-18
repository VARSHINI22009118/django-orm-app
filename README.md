# Django ORM Web Application

## AIM

To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:

Create a django application

### STEP 2:

Write your code in models.py and admin.py

### STEP 3:
End of the program

Write your own steps

## PROGRAM
```html
<html>
    <head></head>
    <body>
        <h1>
            Welcome to Saveetha Engineering College
        </h1>
    </body>
</html>
```
### models.py
```python
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
### admin.py
```python
from django.contrib import admin
from .models import Student,StudentAdmin
# Register your models here.
admin.site.register(Student,StudentAdmin)
```
## OUTPUT

### Clientoutput
![c0](https://user-images.githubusercontent.com/119401150/232910188-1be45cae-f32c-41f3-9153-fe441cc7b4b7.png)

### Serveroutput
![so](https://user-images.githubusercontent.com/119401150/232910293-7d4678f8-9023-4ce7-8d82-8a83c930fde6.png)

## RESULT
Thus the program has been executed successfully.
