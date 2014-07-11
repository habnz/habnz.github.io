---
layout: post
title:  "CantHAB payload transmission testing - Sun July 13th"
date:   2014-07-06 14:05:11
categories: flights
---

In the run up to our first flight, we will be performing some payload
testing.  Would-be trackers are heartily encouraged to try out their set-up
during these tests.

We are intending on testing our payload transmission from the Port Hills
on Sun July 13th 2014.

Weather permitting we will have the payload operational from around 11am to
2pm.  You will be able to test end to end decoding of the payload telemetry
sentences during this time.  Range is unknown at this time, but if you have
line of sight to Sugar Loaf you should be able to pick up the payload with
a beam antenna.

If you are planning on tracking any of our flights
this is a great opportunity to test your system.  Details of how to track
our payloads is on the [tracking](/tracking/) page.

Once you have installed [dl-fldigi](http://ukhas.org.uk/projects:dl-fldigi), you
can do the following to configure it for our payload:

- Go to _DL Client -> Configure_ on the menu
- Select the _All payloads (testing)_ tab
- Select _CANTHAB-MOA-1_ from the (long) list
- Click _Autoconfigure_

This should set up dl-fldigi to decode the payload correctly.  Follow the
instructions at [the UKHAS tracking
guide](http://ukhas.org.uk/guides:tracking_guide) until you get a 'green'
decode.  Once that is working, provided you are online you should see your
telemetry appearing on the [Spacenear.us tracker](http://spacenear.us/tracker/)

![dl-fldigi green decode](/assets/green-decode-screenshot.png)

If you want to try decoding the payload without dl-fldigi, the transmision
details are:

- Frequency 434.500 MHz LSB (FSK with 500Hz shift)
- RTTY 50 baud, 7 bit ascii, no parity, 2 stop bits
- Telemetry sentances are `$$CALLSIGN,sentence_id,time,lat,lon,altitude,speed,course,temperature,checksum`

