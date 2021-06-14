# Django CRUD and Forms
## Forms
### An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server. The form is defined in HTML as a collection of elements inside `<form>...</form>` tags, containing at least one input element of `type="submit"` as in:
``` 
<form action="/team_name_url/" method="post">
    <label for="team_name">Enter name: </label>
    <input id="team_name" type="text" name="name_field" value="Default name for team.">
    <input type="submit" value="OK">
</form> 
```
### The submit input will be displayed as a button (by default) that can be pressed by the user to upload the data. The form attributes define the HTTP method used to send the data and the destination of the data on the server (action):
- `action`: The resource/URL where data is to be sent for processing when the form is submitted
- `method`: The HTTP method used to send the data: post or get.
    - `POST` method 
    - `GET` method
## Django form handling process
### Django's form handling uses the following techniques:
![ex](https://i.ibb.co/55hYjP9/1.jpg)
## Creating Forms
### The declaration syntax for a Form is very similar to that for declaring a Model, and shares the same field types. Form data is stored in an application's forms.py file, inside the application directory. To create a Form:
```
from django import forms

class RenewBookForm(forms.Form):
    renewal_date = forms.DateField(help_text="Enter a date between now and 4 weeks (default 3).")
```
### There are many other types of form fields as:
- BooleanField
- CharField
- ChoiceField
- TypedChoiceField
### Django provides numerous places where you can validate your data. The easiest way to validate a single field is to override the method `clean_<fieldname>()` for the field you want to check.
## View
### the view renders the default form when it is first called and then either re-render it with error messages if the data is invalid, or process the data and redirect to a new page if the data is valid. In order to perform these different actions, the view has to be able to know whether it is being called for the first time to render the default form, or a subsequent time to validate data.
