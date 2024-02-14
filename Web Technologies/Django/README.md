# Django


## Topic: Django Models

### 1. Introduction to Django Models:

Django models represent database tables. </br>
Each model class corresponds to a table and each attribute to a field. </br>
Models define the structure and behavior of data. </br>


### 2. Creating Models:

Define models in models.py file of Django app. </br>
Use Django's models.Model class as a base class for custom models. </br>
Define fields using various field types such as CharField, IntegerField, DateField, etc. </br>


### 3. Relationships in Models:

Django supports various types of relationships: OneToOne, ForeignKey, ManyToMany. </br>
Use ForeignKey for many-to-one relationships and ManyToManyField for many-to-many relationships. </br>
Related objects can be accessed using attribute notation or querysets. </br>


### 4. Migrations:

Migrations are Django's way of propagating changes you make to your models (adding a field, deleting a model, etc.) into your database schema. </br>
Create migrations using python manage.py makemigrations. </br>
Apply migrations to the database using python manage.py migrate. </br>


### 5. Model Methods and Properties:

Define custom methods in models to encapsulate business logic. </br>
Use properties to create computed fields. </br>
Model's __str__ method for string representation. </br>


### 6. Meta Options:

Meta class allows you to specify some ordering options, database table name, and other metadata. </br>
Common Meta options include ordering, verbose_name, verbose_name_plural.</br> 


### 7. Model Managers:

Model managers allow you to encapsulate complex query logic. </br>
Custom managers can be defined by extending models.Manager class. </br>
Managers provide methods for querying data from the database. </br>


### 8. Abstract Models:

Abstract models are base models that contain common fields and methods. </br>
They are not created as database tables. </br>
Other models can inherit from abstract models to reuse fields and methods. </br>


### 9. Inheritance in Models:

Django supports model inheritance. </br>
Abstract base classes provide a way to inherit common fields and methods. </br>  
Multi-table inheritance creates separate database tables for each model. </br>


### 10. Django Admin and Models:

Django admin interface automatically generates a UI for managing models. </br>
Register models with admin using admin.site.register(ModelName). </br>
Customize admin interface using ModelAdmin class. </br>


### 11. Model Forms:

ModelForms are a convenient way of creating forms from Django models. </br>
Automatically creates form fields based on model fields. </br>
Handles validation and saving data to the database. </br>
