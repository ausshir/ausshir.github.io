---
published: true
layout: post
description: CaNoRock Part Four
keywords: 'CaNoRock, Norway, Andoya Space Center, Oslo'
imgfolder: /assets/images/canorock
images:
  - name: installing_sensors.jpg
    thumb: installing_sensors.jpg
    text: Installing sensors in the rocket payload.
  - name: adjusting_tm.jpg
    thumb: adjusting_tm.jpg
    text: >-
      Adjusting settings on the telemetry hardware to tune into the rocket
      payload signal.
---
## Revisiting TM: Testing
The rocket is getting much closer to completion, and the telemetry team was able to run the first system test. We did this by wiring up all sensors to the main computer board and radio card, and placing a [Dummy Load](https://en.wikipedia.org/wiki/Dummy_load) on the antenna as an attenuator, as to not overload the receiver from too much gain.

{% include gal.html image="installing_sensors.jpg" %}
{% include gal.html image="adjusting_tm.jpg" %}

As a result of this test, we confirmed that all the sensors are operational! I had heard from the payload team that they struggled with a few of the sensors, but with all of them working at this stage, we should be able to solve any new problems that arise.

For this launch, we have outfitted the rocket with a few environmental sensors which we can then use to determine many properties about the rocket's trajectory:

1. pressure sensor
2. magnetometer
3. accelerometer
4. dual temperature sensors
5. light sensor

The payload also transmits a signal that records the battery voltage and launch command for diagnostic purposes on the launchpad.

## Hello NOAA
With a bit of spare time, the Telemetry group set up an antenna and a USB SDR (Software Defined Radio) to download live images from NOAA satellites. We were able to get NOAA-15, 18, and 19. Currently, NOAA is [only operating these three polar orbiters](http://www.ospo.noaa.gov/Operations/POES/status.html) (POES), and our proximity to the pole means it is in an excellent position to [track them on each orbit](https://www.youtube.com/watch?v=y_jM_BxQGvE).

The newest, NOAA-19, was launched February 07, 2009. NOAA-19 is classified as the "operational" satellite. We also got the best results with NOAA-19.

There are a lot of other earth observing satellites; many [can be seen here](http://www.ospo.noaa.gov/Operations/). The general approach we took is very similar to what is shown in [this video](https://www.youtube.com/watch?v=zWEiOI33emY). I have always found the sounds of these digital transmissions mesmerising!

#### Where are NOAA-16 and 17?
NOAA-17 was decommissioned on 10 April 2013 after being replaced by newer satellites and many of its critical systems degrading beyond operation.

NOAA-16 was decommissioned on 9 June 2014 after a critical anomaly, and on 23 November 2015, it suffered a breakup event which is currently being tracked by the Joint Space Operations Center as over 200 pieces of debris!

Some other old NOAA satellites are shut down as space radiation and obsolescence have taken their toll. But they're [still up there](https://www.youtube.com/watch?v=JvkSS-a5mqM) and I'd be very interested in trying to find a few myself.

## 4D Space and Launch Vehicle Physics
There were two more lectures today. One was introducing 4D Space (a strategic research initiative to study space weather at the Universtiy of Oslo), and the second covered the physics behind getting something into space!

[This webpage](http://www.mn.uio.no/fysikk/english/research/projects/4dspace/) can do a better job at explaining 4D space than I can. The program is an interesting initiative to me because of how it brings high-level space research (plasma physics!) to multidisciplinary departments, and even to undergraduates at UiO designing the CubeSTAR nanosatellite. I believe that having a sharp focus and high level of collaboration adds meaning and impact to the Norwegian space program, and is a great way to do outreach and gain recognition even outside of its borders.

## Swimming
As is (what seems to be) tradition, some of us went swimming in the Arctic Ocean. Of course, we picked the stormiest, coldest night to do so - perhaps so the wind would dry us off quickly?

Not to brag, but I think I have been in colder lakes! I have also never been in the Atlantic/Artic ocean before and it was noticeably saltier. As it turns out [Western Canada has a very low salinity level compared to other parts of the world](https://www.nasa.gov/sites/default/files/images/591162main_pia14786-43_full.jpg)!

This ocean [temperatures map](http://www.ospo.noaa.gov/data/sst/contour/global.c.gif) at the time of writing suggests the water was about 10 degrees Celsius, which seems to be appropriate. A big lake in Saskatchewan, Lake Diefenbaker [would be 6-10 degrees at the start of the camping season](http://wldb.ilec.or.jp/data/databook_html/nam/nam-58.html). I certainly wish there was a sauna on the beach!
