# API Deployment
## Configuring Django Settings: Best Practices
### Managing Django Settings
- Different environments. You need an approach that allows you to keep all these Django setting configurations
- Sensitive data. You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs
- Sharing settings between team members. You need a general approach to eliminate human error when working with the settings
### Setting Configuration
#### settings_local.py. The basic idea of this method is to extend all environment-specific settings in the settings_local.py file, which is ignored by VCS
#### Separate settings file for each environment. It allows you to keep all configurations in VCS and to share default settings between developers
#### Environment variables. To solve the issue with sensitive data, you can use environment variables
#### 12 Factors. 12 Factors is a collection of recommendations on how to build distributed web-apps that will be easy to deploy and scale in the Cloud. It was created by Heroku, a well-known Cloud hosting provider. the collection consists of twelve parts:
- Codebase
- Dependencies
- Config
- Backing services
- Build, release, run
- Processes
- Port binding
- Concurrency
- Disposability
- Dev/prod parity
- Logs
- Admin processes
#### django-environ. Writing code using os.environ could be tricky sometimes and require additional effort to handle errors. It’s better to use django-environ instead. it merges:
- envparse
- honcho
- dj-database-url
- dj-search-url
- dj-config-url
- django-cache-url
#### This app gives a well-functioning API for reading values from environment variables or text files, handful type conversion, etc
#### Setting Structure. Instead of splitting settings by environments, you can split them by the source: Django, third- party apps (Celery, DRF, etc.), and your custom settings

