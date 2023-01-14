# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![output](/ORM%20PICTURE.jpg)


## DESIGN STEPS

### STEP 1:
Create a project and inside the project folder, create an application using - django-admin startproject and django-admin startapp .Inside the applicaton folder, open setiings.py and allow all the hosts.

### STEP 2:
Now in the application folder, open models.py and write the code for your desired table here. Go to admin.py and migrate all your data.


### STEP 3:
On running the server, open the html page.Here you can add or get the desired data from the table you have created.

## PROGRAM
```
from django.db import migrations models
from django.contrib import admin
class Migration(models.model):
    id = models.Autofield()
    employmentnumber = models.Integerfield()
    employmentname = models.Charfield(max_length=100)
    age = models.Integerfield()
    email = models.Emailfield()
    place = models.Charfield(max_length=100)
    designation = models.Charfield(max_length=100)
    salary = models.Charfield(max_length=100)
class Migrationadmin(admin.ModelAdmin):
list_display=("Id","employementnumber","employementname","age","email", "place","designation","salary")
```



## OUTPUT
![output](/WhatsApp%20Image%202022-12-29%20at%2000.46.42.jpg)






## RESULT
Thus Django application to store and retrieve data from a database using Object Relational Mapping(ORM) is successfully executed.

