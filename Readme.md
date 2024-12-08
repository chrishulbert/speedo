# Speedo

A simple and free speedometer.

No need to install ad-ware apps from the app/play store!

## HTTPS

To use Geolocation, HTTPS is essential. When developing, use Caddy to get https, like so:

* Install caddy: brew install caddy
    * Downloads from the caddyserver.com site/github don't seem to work.
* To host locally with https, run this from the same folder as index.html:
    * caddy file-server --domain localhost
    * It might ask for password for setting up the certs
* Then open https://localhost in browser, should be ok
* The Makefile has a target to automate this:
    * `make serve`
