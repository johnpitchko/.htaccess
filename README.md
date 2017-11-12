# .htaccess

Custom .htaccess file **Inspired by: https://github.com/h5bp/server-configs-apache**

Several enhancements and modifications were made to the standard version linked above.

1. Configured for WordPress (these are commented out by default)
  * Including configuration for WordFence plugin
2. Redirecting naked URLs to www
3. Forcing HTTPS
4. Allow URLs without extensions (i.e. `www.server.com/webpage` is the same as `www.server.com/webpage.html`)
  * Accessing webpages using the file extension will still work; no redirect happens.
5. Support automatic generation of Let's Encrypt certificates by cPanel

## Installation

Download the .htaccess file and install to the domain folder (e.g. ~/public_html or what ever folder your domain is mapped to on your webserver).

**Highly recommend** you backup your original .htaccess file, as some web hosts may have configured their Apache server to not accept some configurations included in the file. This can sometimes cause 500 Internal Server Errors.
