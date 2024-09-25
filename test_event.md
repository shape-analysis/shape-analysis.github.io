---
layout: null
permalink: /events.ics
paragraphs: false
---
BEGIN:VCALENDAR
VERSION:2.0
PRODID:-//Your Site//NONSGML v1.0//EN
CALSCALE:GREGORIAN
METHOD:PUBLISH
{% for event in site.data.seminar %}
BEGIN:VEVENT
UID:{{ event.date | date: "%Y%m%dT%H%M%SZ" }}@yourdomain.com
DTSTART:{{ event.date | date: "%Y%m%dTH%M%SZ" }}
DTEND:{{ event.date | date: "%Y%m%dT%%H%M%SZ" }}
SUMMARY:{{ event.title }}
LOCATION:{{ event.location }}
DESCRIPTION:{{ event.title }}
END:VEVENT
{% endfor %}
END:VCALENDAR

