This is a shell script whose purpose is to test for 
internet access.  This is for when something's not working and
you're not sure if a site's down or your connection's down or 
something else.

It works by pinging a series of sites (which you can specify).

If all the sites are unreachable, it reports that there's no
access and then starts retrying every 15 seconds or so.
After each test it tells you if there's no access, or there's
access to at least one site or if everything's up.

If at least one site is up for 3 tries in a row, then it reports that
you have access, and rings a bell to let you know.

Otherwise it keeps testing until it times out (2 hours I think)
or you type ctrl-C to halt the script.

The audio uses the  mac afplay command.  
Don't know how to make sounds on other systems.  Ctrl-G I guess?

Also, theres' a place in the script where it tests for the gnu
timeout command, which macs don't have.  Uses a timed ping instead.
(You can install gnu utils on a mac with brew).

Also, there is a second script called elapsed_time.  This just
converts tics to a human-readable days, hours, minutes.  There's
probably a better way to do this but this was my way. The amiup
script uses this to report the total down time.


I'm not very good at this stuff so no guarantees, but I've used it
for a long time when I'm in doubt, and continue to find it useful..

J.
johnmx@digitalmx.com


