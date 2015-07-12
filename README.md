# Potassium Bootstrapping Template
[![ion install --local template-potassium](https://img.shields.io/badge/ion%20install%20----local-template--potassium-blue.svg?style=flat-square)](https://github.com/IodineLang/Ion)
![version v1.0.0](https://img.shields.io/badge/version-v1.0.0-blue.svg?style=flat-square)
![deps](https://img.shields.io/badge/dependencies-potassium-blue.svg?style=flat-square)

An installable template for a Potassium project.

## After Installing
- Rename src/myapp/ to your application name
- Change .myapp.urls to .newappname.urls in src/application
- Change src/myapp/views.id to suit your own app's views and change MyAppViews to
NewAppNameViews
- Change `func MyAppViews (self)` to `func NewAppNameViews (self)`
- Change `use MyAppViews from .views;` to `use NewAppNameViews from .views;` in src/myapp/urls.id.

Then, you're done, and you've got a lovely, neatly-formatted Potassium 
application. You can run a development server with ./runserver.py (assuming you
have Python 2 installed). Then, access your application at `localhost:8000/src/application/route`.

When you want to serve your app in production, you can use apache's `mod_rewrite`
to redirect all requests to src/application, and give the illusion of files.

Enjoy! 
