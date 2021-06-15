# Django Custom User
## User model
### Django ships with a built-in User model for authentication. To start, create a new Django project from the command line then:
- create and navigate into a dedicated directory called accounts for our code
- install Django
- make a new Django project called config
- make a new app accounts
- start the local web server
### However we don't run migrate to configure our database until we create our new custom user model.
## AbstractUser vs AbstractBaseUser
### There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser. In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires more work.
## Custom User Model
### To custom user model then:
1. update config/settings.py
2. create a new CustomUser model
3. create new UserCreation and UserChangeForm
4. update the admin
## Superuser
### we can create a superuser so that we can use it to log in to the admin and test out log in/log out.
## Templates/Views/URLs
### we start by updating settings.py to use a project-level templates directory. then we create a new project-level templates folder and within it a registration folder as that's where Django will look for the log in template. after that we create a urls.py file in the accounts app. 