# Laravel Spigot Permissions

The idea here is simple: implement a permission system within Laravel with similar functionality to Spigot and the various permission plugins that exist. 

There are a few specific goals
* Permission syntax: `module.group.group.action`, where there can be as many groups chained as necessary
* Allow permissions to be registered with a default value of `true`/`false`
* Allow permissions to be assigned to users with a defined value of `true`/`false`
* Allow permissions to be assigned to user roles with a defined value of `true`/`false`
* Allow permissions such as `module.group.*` to be assigned to explicitly allow/deny any permissions within a group
* Allow a sytax such as `$user->hasPermission('a.b.c')`, where permissions are checked as follows:
    1. check if the user has the permission allowed directly
    2. Check if the user's role allows this permission
    3. Return the default value of the permission

In the ideal, this would all run through Laravel's guards, allowing permission checks to work in Blade templates as well.
