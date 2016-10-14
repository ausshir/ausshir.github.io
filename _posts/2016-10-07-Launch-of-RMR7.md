---
published: false
---
## Rocket Launch Logistics
The day started off with a gathering of all students to discuss the launch. Group A (Numerical Simulation) focused on calculating a trajectory and launch angle by taking the weather into account, as well as giving us some predicted flight statistics. Next, group C (Payload) gave us a status report. As we had tested the day before, all the sensors were working well, and now everything was fully assembled, balanced, and decorated.

The flight was expected to take approximately 90 seconds, and reach an altitude of over 11km. The weather had started to turn sour with dark clouds and heavy rain, but it was still good enough for a launch.

Of course, we still had to name the rocket. As this was a group of goofy physics nerds, we were more interested in making a good joke than anything else. [Unencumbered](https://www.theguardian.com/environment/2016/apr/17/boaty-mcboatface-wins-poll-to-name-polar-research-vessel) by [common sense](http://www.bbc.com/news/uk-36225652), we chose the name Rockety McRocketface by a narrow margin. Other great options were [ICI-7](https://www.mn.uio.no/fysikk/english/research/projects/ici/) to tease the Universtiy of Oslo's upcoming project, or [Up-Goer-7](https://xkcd.com/1133/) fro, the webcomic XKCD.

## Preparing for The Launch
We started the launch procedures by doing a quick overview of the countdown. We were using the conventional Andoya process, which is approximately the same as the one NASA uses ([NASA launches research rockets at ASC as well](http://andoyaspace.no/?p=2099)). ASC technicians would oversee the launch, but ultimately the students were in control of the entire thing! We had our own Head of Operations in the control tower, a Payload Supervisor, Project Scientists, and many other positions. As Main Telemetry Supervisor, my job was to confirm over the radio that the rocket was powered, run all safety checks and send a GO-signal to approve the launch.

The Main Telemetry station was already set up for our rocket, and a lot of the process is automated. The NAROM telemetry station had fully manual equipment, and so the students there had a much more involved job during launch.

## Delay in the Countdown
All good projects can't go without a hitch, and ours had a nice big one in the last few minutes before launch! The payload was set to the incorrect bit rate for data transmission, and since the student telemetry equipment we tested is not sensitive enough to notice a difference, we were not able to get it corrected.

At the Main Telemetry station, the recording equipment was reading out a bitrate of 262.5kBit/s well above the specification of 250kBit/s. This difference was too large for the recording gear to synchronise with the incoming stream, and therefore was not able to decode the data frames. After reconfiguring all the recorders to the new bitrate, we were up and running again. Luckily it was a very straightforward solution to a problem that added just a bit of spice to the launch!

Overall the countdown was delayed about 10 minutes. Many people have the misconception that everyone is rushing to get the countdown done as soon as possible, but in practice, it is just the opposite! The countdown exists to make sure everything is given the appropriate amount of care and specifies the absolute minimum amount of time to do each task. If one part is delayed, the entire countdown is paused to let that task complete and keep everything synchronised.

## Launch
Loud and fast! I'll let this video do the talking.

The launch lasted only 90 seconds, and my station confirmed it lost signal as the rocket plunged into the ocean. Now the science begins!

## Analysing Launch Results
The telemetry groups main task was to ensure all data was collected and archived, and it was mainly up to the other groups to sort out the data processing. As an aside, we set out to verify the simulation of the rocket physics group by calculating the maximum altitude from the outside air pressure.

Because most atmospheric pressure derived from the weight of the air above the point of measurement (also referred to as hydrostatic pressure), it is straightforward to determine your altitude. Pressure varies smoothly from the Earth's surface all the way to the top of the mesosphere and is the standard method of determining aircraft altitude. For altitudes below 11km, it can be much more accurate than consumer GPS solutions as well.

### Anomaly
When going through our recorded data, most of the teams noticed a small glitch at approximately 1 second after launch. After looking closely at the launch video, we identified a small piece of flaming debris exit the rocket.

As seen in this [old-school research paper](http://www.dtic.mil/cgi-bin/GetTRDoc?Location=U2&doc=GetTRDoc.pdf&AD=AD0596285) or a [much more recent one](http://my.fit.edu/~chintals/index_files/A32358.pdf), rocket exhaust (ionised gas) has a significant impact on both attenuation of radio signals and wideband noise generation. The net effect of this is the auto-tracking antennas lost connection with the rocket's transmitters and then locked onto the RF power from the flaming debris for a split second. It recovered quickly, but we did lose a few frames of diagnostic data during launch.

The CRV-7 C-14 rocket motor came in many different forms. The original version smoke production from the Aluminum fuel and therefore had higher amounts of debris expelled from the nozzle. An updated version C-15 changes the fuel mixture to reduce smoke, but it also contains an internal igniter that gets ejected after launch. I believe we had one of these revisions, and the debris is either the igniter or large piece of debris in the smoke.