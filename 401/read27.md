# Django Models
## Models
#### Models define the structure of stored data, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms,... etc. Models are usually defined in an application's `models.py` file. 

## Fields
#### A model can have an arbitrary number of fields, of any type where each field represents a column of data. Common field arguments: 
- help_text
- default
- null
- blank
- primary_key
#### and the common field types:
- CharField
- TextField 
- IntegerField 
- DateField 
- EmailField
## Methods
#### at least, every model you should define the standard Python class method __str__() to return a human-readable string for each object. Another common method to include in Django models is get_absolute_url()
## Model management
#### Model classes can be used to create, update, or delete records, and to run queries to get all records or particular subsets of records as in the following:
- Creating and modifying records by defining an instance of the model then calling save():
    - record = MyModelName(my_field_name="Instance #1")
    - record.save()
- Searching for records by using the model's objects attribute
## Re-run the database migrations
#### re-run the database migrations and add them to in the database then
- `python3 manage.py makemigrations`
- `python3 manage.py migrate`
## Registering models 
#### Register the models by copying the following text into the bottom of the file:
```
from .models import Author, Genre, Book, BookInstance

admin.site.register(Book)
admin.site.register(Author)
admin.site.register(Genre)
admin.site.register(BookInstance)
```