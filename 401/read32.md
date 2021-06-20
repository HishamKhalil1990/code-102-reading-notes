# Permissions & Postgresql
## Permissions
### With authentication and throttling, permissions determine whether a request should be granted or denied access. Permission checks are always run at the very start of the view, before any other code is allowed to proceed. Permissions are used to grant or deny access for different classes of users to different parts of the API.
### Permissions in REST framework are always defined as a list of permission classes. When the permissions checks fail either a "403 Forbidden" or a "401 Unauthorized" response will be returned, according to the following rules:
- The request was successfully authenticated, but permission was denied. — An `HTTP 403` Forbidden response will be returned.
- The request was not successfully authenticated, and the highest priority authentication class does not use WWW-Authenticate headers. — An `HTTP 403` Forbidden response will be returned.
- The request was not successfully authenticated, and the highest priority authentication class does use `WWW-Authenticate headers`. — An `HTTP 401` Unauthorized response, with an appropriate `WWW-Authenticate header` will be returned.
### REST framework permissions also support object-level permissioning. Object level permissions are run by REST framework's generic views when `.get_object()` is called. As with view level permissions, an exceptions.PermissionDenied exception will be raised if the user is not allowed to act on the given object.
### The default permission policy may be set globally, using the `DEFAULT_PERMISSION_CLASSES` setting.  when you set new permission classes via the class attribute or decorators you're telling the view to ignore the default list set in the `settings.py` file.
## API Reference
### API Reference are:
- AllowAny
- IsAuthenticated
- IsAdminUser
- IsAuthenticatedOrReadOnly
### `DjangoObjectPermissions` permission class ties into Django's standard `django.contrib.auth` model permissions. This permission must only be applied to views that have a `.queryset` property or `get_queryset()` method. Authorization will only be granted if the user is authenticated and has the relevant model permissions assigned
### To implement a custom permission, override `BasePermission` and implement either, or both, of the following methods:
- `.has_permission(self, request, view)`
- `.has_object_permission(self, request, view, obj)`
### If you need to test if a request is a read operation or a write operation, you should check the request method against the constant SAFE_METHODS, which is a tuple containing `GET`, `OPTIONS` and `HEAD`.
