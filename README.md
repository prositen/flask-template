# flask-template

Template flask application with
* database migrations
* offline user management
* date-rotated access logs


## Setup

### Config file

Copy config.skeleton.py to config.py and add your own settings

Generate the secret key in a python shell
```
import os
import binascii
binascii.hexlify(os.urandom(32)
```

### Database

Create database

`python manage.py db upgrade`

Create an admin user

`python manage.py add_admin` 
