# Laravel Eloquent Dart Port

I like the way that Laravel's Eloquent ORM works, defining models and relations on the classes, as well as the way Laravel handles migrations with the Schema builder. I'd like to port that to Dart, in a way where it could be used both on the server and in a Flutter app by passing in different "drivers". In that way you could use a MySQL or PostgreSQL driver on the server for connecting directly to a remote database, or a SQLite or LocalStorage driver for handling some local data caching in mobile apps or websites, respectively.

There could be a `dart pub` cli for handling migrations when it comes to the server side, as well as a way to run the migrations at runtime for instances like a mobile app, in order to setup a SQLite database when the user installs or updates the app.
