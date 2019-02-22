# Wordpresss buildpack: (PHP required)

![php](https:////s.w.org/style/images/wporg-logo.svg?3)


This is the sample of plain and straight option for installing Wordpress on Heroku platform.

Please note that that's secondary buildpack and will not work without previously applied [Heroku-PHP-buildpack](https://elements.heroku.com/buildpacks/heroku/heroku-buildpack-php)

All it does, just a copying WP release from the off site into the WORDPRESS_DIR (env variable will be available for config)
## Usage

You can check an example of application [~Wordpress-Heroku-App~](https://github.com/2oppin/heroku-wp)

If you already have an php-starter project you can add buildpack this way:


    $ heroku buildpacks:add https://github.com/2oppin/heroku-wp-buildpack

Buildpack will add env variables to your app:

WORDPRESS_DIR place where WP codebase should reside (default ~ wordpress/)
WORDPRESS_VERSION the version of WP you need (default ~ latest)