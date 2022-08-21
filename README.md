This is a shell script whose purpose it to test for 
internet access.  This is for when something's not working and
you're not sure if a site's down or your connection's down or 
someth8ing else.

It works by pinging a series of sites (which can specify).

If all the sites are unreachable, it reports that there's no
access and then starts retrying every 15 seconds or so.
After each test it tells you if there's no access, or there's
access to at least one site or if everything's up.

If at least one site is up for 3 tries in a row, then it reports that
you have access, and rings a bell to let you know.

Otherwise it keeps testing until it times out (2 hours I think)
or you type ctrl-C to halt the script.

The audio is designed for a mac using afplay command.  
Don't know how yto make sounds on other systems.  Crl-G I guess?

Also, there is a second script called elapsed_time.  This just
converts tics to a human-readable days, hours, minutes.  There's
probably a better way to do thisk but this was my way.

Just needs to be you path somewhere so the first script can use it.


I'm not very good at this stuff so no guarantees, but I've used it
for a long time when I'm in doubt.

J.
johnmx@digitalmx.com


