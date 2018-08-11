I'm going to take general mumble notes here so that when I have to actually work on the mumble server, I have a reference of common crap I have to do.


#Web Interface config
So it mostly just works, but you have to manually bootstrap the django db.

Once everything is online:
1. docker exec -it <name of webhead container> bash
1. cd /usr/src/app/pyweb
1. python manage.py syncdb
** When it asks about the ice/dbus thing, enter Meta:tcp -h head -p 6502, no secret; and your good to go.
