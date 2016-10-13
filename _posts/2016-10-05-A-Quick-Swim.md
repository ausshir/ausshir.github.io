---
published: false
layout: post
description: CaNoRock Part Four
keywords: 'CaNoRock, Norway, Andoya Space Center, Oslo'
imgfolder: /assets/images/canorock
images:
  - name: aurora1.jpg
    thumb: aurora1.jpg
    text: Spaceship Aurora
  - name: aurora2.jpg
    thumb: aurora2.jpg
    text: Spaceship Aurora
  - name: tour_sign.jpg
    thumb: tour_sign.jpg
    text: Charred by rocket flames is the best way to have a sign.
  - name: tour_launcher.jpg
    thumb: tour_launcher.jpg
    text: >-
      The ASC Launch Rail. This device tilts up and folds back the roof when
      launching a rocket.
  - name: tour_science_command.jpg
    thumb: tour_science_command.jpg
    text: >-
      Science mission command room. Mission control, coms and the launch bunkers
      are not shown.
---
## Revistiting TM
The rocket is getting much closer to completion, and we were able to run out first system test. We did this by wiring up all sensors to the main computer board and radio card, and placing dummy load attenuators on the antennas (as to not overload the receiver from too much gain). The FM tuner was able to demodulate the signals, pass it through the antenna polarization selector to the bit-synchronizer, and finally onto the computer where the PCM (pulse-code modulation) was decoded and displayed.

Result: All the sensors are go! For this launch we managed to include a pressure sensor, magnetometer, accelerometer, dual temperature sensors in the nose and body, an IR Light sensor, and internal battery voltage. There aslo is a signal that records the launch command so we can get a precise start to our sensor readings.

## Hello NOAA
With a bit of spare time the Telemetry group set up an antenna and a USB SDR (Software Defined Radio) to download live images from NOAA sattelites. We were able to get NOAA-15, 18, and 19. Currently, NOAA is [only operating these three polar orbiters](http://www.ospo.noaa.gov/Operations/POES/status.html) (POES), and Andoya's proximity to the pole means it is in an excellent position to track them each orbit (as opposed to once-per day for most other places on earth).

The newest, NOAA-19, was launched February 07, 2009. NOAA-19 is classified as the "operational" satellite. This is the one with which we got the best results.

There are a lot of other operational earth observing sattelites, many can be seen here: http://www.ospo.noaa.gov/Operations/.

#### Where are NOAA-16 and 17?
NOAA-17 was decomissioned on 10 April 2013 after being replaced by newer sattelites and many of its key systems degrading beyond operation.

NOAA-16 was decommissioned on 9 June 2014 after a critical anomaly, and on 23 November 2015, it suffered a breakup event which is currently being tracked by the Joint Space Operations Center as over 200 peices of debris!

## 4D Space and Orbital Physics

## Swimming
As is apparently tradition, some of the Canadians (myslef included) went swimming in the Arctic Ocean. Of coruse we picked the stormiest, coldest night to do so!
