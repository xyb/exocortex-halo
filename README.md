# exocortex-halo
Various and sundry additional pieces of software I've written to incorporate into my exocortex that extend the functionality of Huginn (https://github.com/cantino/huginn).  You never know what you're going to find in here because I do a lot of idiosyncratic stuff and as I get ideas for functionality to incorporate new things will appear in here.  Not all of them will make sense.

exocortex_gps_mapper/

A relatively simple web application that uses web.py (http://webpy.org/) to implement a REST API.  An application running on a smartphone periodically pings an endpoint with its current GPS coordinates.  Contacting the web app throws up a Google Map with the GPS coordinates.  It's far from complete because I don't know JavaScript.

exocortex_sip_client/

A command line application (mostly) that can be used to place calls into the PSTN via a Voice-Over-IP provider and play a .wav file into the call.  I designed it to work as part of a larger toolkit of utilities.

Special thanks to The Test Call (http://thetestcall.blogspot.com/) for providing the default phone number for debugging.  I got kind of tired of rickrolling myself...

