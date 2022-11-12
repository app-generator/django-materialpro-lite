# [Django Material Lite](https://appseed.us/product/material-wpx/django/)

Open-Source **Django Dashboard** coded with basic modules, database, ORM and deployment scripts on top of MaterialPro Bootstrap Lite, a modern Bootstrap dashboard design. [WrapPixel](https://appseed.us/agency/wrappixel)'s **MaterialPro Bootstrap Lite** is one of the best Bootstrap templates for admin dashboards and control admin panels. This powerful and competent Bootstrap 4 admin template is based on HTML and is built with the CSS framework. 

- 👉 [Django Material Lite](https://appseed.us/product/material-wpx/django/) - product page
- 👉 [Django Material Lite](https://django-materialpro-lite.appseed-srv1.com) - LIVE deployment

<br />

## `PROMO` [Black Friday 2022](https://blog.appseed.us/black-friday-2022-vote-your-discount/)

> This [campaign](https://blog.appseed.us/black-friday-2022-vote-your-discount/) starts on `15-NOV` and the users are able to `vote their discount`: **50, 60, 70%**: 

- 👉 [Discord](https://discord.gg/fZC6hup) `announcements` channel
- 👉 [Twitter](https://twitter.com/webappseed) (official account) 

[![black-friday-2022-cover](https://user-images.githubusercontent.com/51070104/201459148-7561df9f-0a7d-4d1a-bf44-a1ac5e89c175.jpg)](https://blog.appseed.us/black-friday-2022-vote-your-discount/)

<br />

> 🚀 Built with [App Generator](https://appseed.us/generator/), Timestamp: `2022-09-18 07:49`

- ✅ `Up-to-date dependencies`
- ✅ UI-Ready app, `SQLite Database`, Django Native ORM
- ✅ `Session-Based authentication`, Forms validation
- ✅ `Deployment`: **Docker**, Gunicorn / Nginx, HEROKU
- ✅ Support via **Github** (issues tracker) and [Discord](https://discord.gg/fZC6hup).

<br />

![MaterialPRO Lite - Starter generated by AppSeed.](https://user-images.githubusercontent.com/51070104/172007029-0e7c6df5-95d1-4b88-8831-5d35c5c37005.png)

<br />

## ✨ Quick Start in `Docker`

> 👉 **Step 1** - Download the code from the GH repository (using `GIT`)

```bash
$ git clone https://github.com/app-generator/django-materialpro-lite.git
$ cd django-materialpro-lite
```

> 👉 **Step 2** - Start the APP in `Docker`

```bash
$ docker-compose up --build
```

Visit `http://localhost:5085` in your browser. The app should be up & running.

<br />

## ✨ How to use it

```bash
$ # Get the code
$ git clone https://github.com/app-generator/django-materialpro-lite.git
$ cd django-materialpro-lite
$
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv env
$ # .\env\Scripts\activate
$
$ # Install modules - SQLite Storage
$ pip3 install -r requirements.txt
$
$ # Create tables
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
$
$ # Start the app - custom port
$ # python manage.py runserver 0.0.0.0:<your_port>
$
$ # Access the web app in browser: http://127.0.0.1:8000/
```

> Note: To use the app, please access the registration page and create a new user. After authentication, the app will unlock the private pages.

<br />

## ✨ Code-base structure

The project is coded using a simple and intuitive structure presented bellow:

```bash
< PROJECT ROOT >
   |
   |-- core/                               # Implements app configuration
   |    |-- settings.py                    # Defines Global Settings
   |    |-- wsgi.py                        # Start the app in production
   |    |-- urls.py                        # Define URLs served by all apps/nodes
   |
   |-- apps/
   |    |
   |    |-- home/                          # A simple app that serve HTML files
   |    |    |-- views.py                  # Serve HTML pages for authenticated users
   |    |    |-- urls.py                   # Define some super simple routes  
   |    |
   |    |-- authentication/                # Handles auth routes (login and register)
   |    |    |-- urls.py                   # Define authentication routes  
   |    |    |-- views.py                  # Handles login and registration  
   |    |    |-- forms.py                  # Define auth forms (login and register) 
   |    |
   |    |-- static/
   |    |    |-- <css, JS, images>         # CSS files, Javascripts files
   |    |
   |    |-- templates/                     # Templates used to render pages
   |         |-- includes/                 # HTML chunks and components
   |         |    |-- navigation.html      # Top menu component
   |         |    |-- sidebar.html         # Sidebar component
   |         |    |-- footer.html          # App Footer
   |         |    |-- scripts.html         # Scripts common to all pages
   |         |
   |         |-- layouts/                   # Master pages
   |         |    |-- base-fullscreen.html  # Used by Authentication pages
   |         |    |-- base.html             # Used by common pages
   |         |
   |         |-- accounts/                  # Authentication pages
   |         |    |-- login.html            # Login page
   |         |    |-- register.html         # Register page
   |         |
   |         |-- home/                      # UI Kit Pages
   |              |-- index.html            # Index page
   |              |-- 404-page.html         # 404 page
   |              |-- *.html                # All other pages
   |
   |-- requirements.txt                     # Development modules - SQLite storage
   |
   |-- .env                                 # Inject Configuration via Environment
   |-- manage.py                            # Start the app - Django default start script
   |
   |-- ************************************************************************
```

<br />

> The bootstrap flow

- Django bootstrapper `manage.py` uses `core/settings.py` as the main configuration file
- `core/settings.py` loads the app magic from `.env` file
- Redirect the guest users to Login page
- Unlock the pages served by *app* node for authenticated users

<br />

---
[Django Material Lite](https://appseed.us/product/material-wpx/django/) - Provided by **AppSeed** [App Generator](https://appseed.us/app-generator).
