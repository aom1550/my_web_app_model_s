# Django

## คำสั่ง runserver 
    python manage.py runserver 

## คำสั่ง สร้างแอพ
    python manage.py startapp <ชื่อแอพ>

## คำสั่งสร้าง admin 
    python manage.py createsuperuser


## สร้าง models



```python
from django.db import models

# Create your models here.

class Student(models.Model):
    
    std_id = models.IntegerField()
    first_name = models.CharField(max_length=256)
    last_name = models.CharField(max_length=256)
    
    phone = models.CharField(max_length=10)

```

## Admin register models
```python

@admin.register(models.Student)
class StudentAdmin(Admin.ModelAdmin):
    list_display = (

    )


```สวัสดีครับ นาย วัณรุวรระน์ สรีวงศ์แผน ผมมีความตั้งใจที่จะทำโปรเจคชิ้นนี้ครับ