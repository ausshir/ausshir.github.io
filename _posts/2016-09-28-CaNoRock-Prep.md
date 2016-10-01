---
published: true
layout: post
description: CaNoRock Part One
keywords: 'CaNoRock, Norway, Andoya Space Center'
---
## Off to CaNoRock
For the a week between September 30 and October 8, 2016 I am attending an a student
collaboration between Canada and Norway to build and test a research sounding rocket.
All you need to know is in the name!

The event takes place at the Andoya Space Center in Andennes, Norway. This is a
rocket range which also takes part in High Altitude Balloon experiments and other
space-based research. No doubt this will be an intense week, but my goal is to
keep the entire project documented, with a bit of focus on the interesting details
along the way.

### Programming Your Travel
This time around I do not need to take care of all the booking details, but the
nature of the trip leaves tiny bursts of free time interspersed between intense
projects. To make the most of my time I thought I'd try out the new Google Trips
app, which just made it's official transition from Inbox to a standalone tool and
[seems to be targeted directly at me](https://googleblog.blogspot.no/2016/09/see-more-plan-less-try-google-trips.html)!

https://3.bp.blogspot.com/-ck_mwUQmsY4/V9x944vTcxI/AAAAAAAAS_A/gJDda7S3r1MNvpc6ipdcaYTULiu_Pf1vQCLcB/s1600/06_61_combo.png

A very useful feature of Google Trips is the ability for it to scan metadata or
schemas from your reservation emails. There is a vaguely standard format for This
metadata but Google claims it should just work (and it has for me in the past).

Unfortunately, I haven't made any personal bookings for this trip and had no emails
for it to scan! Furthermore, Google decided users didn't need the feature to manually
input trip bookings. Thankfully there's a [terribly complicated hack](http://www.scottgreenstone.com/2016/03/manuallycreatetrips.html) from Scott Greenstone!

One of my flight bookings looked like this:

    function manuallyCreateTrips() {
      var htmlBody = HtmlService.createHtmlOutputFromFile('flight').getContent();

      MailApp.sendEmail({
        to: Session.getActiveUser().getEmail(),
        subject: 'Flight Confirmation - Tromso 2' + new Date(),
        htmlBody: htmlBody,
      });
    }

    <html>
      <body>
        <script type="application/ld+json">
    {
      "@context": "http://schema.org",
      "@type": "FlightReservation",
      "reservationNumber": "11",
      "reservationStatus": "http://schema.org/Confirmed",
      "underName": {
        "@type": "Person",
        "name": "Austin"
          },
      "reservationFor": {
        "@type": "Flight",
        "flightNumber": "4431",
        "airline": {
          "@type": "Airline",
          "name": "Scandinavian",
          "iataCode": "SAS"
        },
        "departureAirport": {
          "@type": "Airport",
          "name": "Tromsø Langnes Arpt",
          "iataCode": "TOS"
        },
        "departureTime": "2016-10-07T18:40:00+02:00",
        "arrivalAirport": {
          "@type": "Airport",
          "name": "Oslo Arpt",
          "iataCode": "OSL"
        },
        "arrivalTime": "2016-10-07T20:35:00+02:00"
      }
    }


    </script>

        <p>
          Dear Google, Please let me manually enter flights.
        </p>
        <p>
          Test body!
        </p>
      </body>
    </html>

*Was it worth it? Apart from the offline trip guides, probably not.. ;)*

### To the skies!
After a lovely turboprop and 
