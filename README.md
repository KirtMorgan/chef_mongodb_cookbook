# Chef Configuration Lab

## Timings

60 - 90 Minutes

## Summary

Our Mongo cookbook currently only install mongodb but it is not configured or started. Let's used templates and attributes to configure the cookbook

## Tasks

Add new ChefSpec tests for the following:

* Create a mongod.conf file in /etc/mongod.conf - TEST COMPLETE + PASSING
* Create a mongod.service file in /lib/systemd/system/mongod.service - TEST COMPLETE + PASSING
* MongoDB service should be enabled - TEST COMPLETE + PASSING
* MongoDB service should be started - TEST COMPLETE + PASSING

And InSpec tests for the following:

* MongoDB is running - TEST COMPLETE + PASSING
* MongoDB is enabled - TEST COMPLETE + PASSING
* MongoDB is listening on 27017 by default - TEST COMPLETE + PASSING
* MongoDB is listening on 0.0.0.0 by default - TEST COMPLETE + PASSING

Create a recipe that installs and configures this cookbook correctly to pass all these tests.

Use attributes to allow the port number and ip to be configurable.
