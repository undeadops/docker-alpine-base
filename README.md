Docker Alpine Linux Base Images
===============================


### Purpose

Purpose is to minimise linked image build times.
Instead of having to rebuild all the the base OS image layers with 
each of my applications, they will just import for these images.

Should make my blogs Travis-CI tests run cocnsiderably faster since it
won't have to build the full docker images, just the application layer.


##### Images

- alpinebase

    Base Image with just Alpine Linux all other Images will link off of this one

- alpine-java

    Base Image plus OpenJDK 8 + wget + supervisor

- alpine-nginx

    Base Image plus Latest Nginx Stable, might eventually get around to including
    the lets encrypt wrappers, as well as some form of service discovery.

- alpine-python

    Base Image plus python with pip + wget + supervisor

I'm sure more images will follow, but that wraps up my immediate needs
