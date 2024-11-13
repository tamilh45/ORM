# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![DBMS INDEX](https://github.com/user-attachments/assets/809d6dec-3abe-45c2-b936-81a9d2e8efe3)



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```

admin.py

from django.contrib import admin from .models import loan,loanadmin admin.site.register(loan,loanadmin)

models.py

from django.db import models from django.contrib import admin class loan (models.Model): loan_id=models.IntegerField(primary_key=True) loan_type =models.CharField(max_length=30) loan_amnt =models.FloatField() cust_acntno =models.IntegerField() cust_name=models.CharField(max_length=50)

class loanadmin(admin.ModelAdmin): list_display=('loan_id','loan_type','loan_amnt','cust_acntno','cust_name')


```


## OUTPUT

![Screenshot 2024-03-05 110658 (1](https://github.com/user-attachments/assets/dba0483e-8999-4de7-af70-08300ecd9c6e)



Include the screenshot of your admin page.


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
