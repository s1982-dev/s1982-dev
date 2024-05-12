---
layout: post
title:  "Date format string cheat sheet in Ruby?"
date:   2022-03-16 06:15:05 -0700
categories: [Development]
path: "development"
tags: ["Ruby on Rails"]
---

| Date Formatting                                           |
|:-------:|:-----------------------------------------------:|
| %Y      | Year with century (e.g. 2022, 1982, etc)        |
| %m      | Month of the year, zero-padded (01..12)         |
| %B      | The full month name (e.g. January)              |
| %b      | The abbreviated month name (e.g. Jan)           |
| %d      | Day of the month, zero-padded (01..31)          |
| %j      | Day of the year (001..366)                      |
| %C      | Year / 100 (round down. e.g. 20 in 2013)        |
| %y      | Year % 100 (00...99)                            |
| %_m     | Month of the year, blank-padded (_1..12)        |
| %-m     | Month of the year, no-padding (1..12)           |
| %^B     | The full month name uppercased (e.g. JANUARY)   |
| %^b     | The abbreviated month name uppercased (e.g. JAN)|
| %h      | Equivalent to %b (abbreviated month name)       |
| %-d     | Day of the month, no-padding (1..31)            |
| %e      | Day of the month, blank-padded (_1..31)         |


| Time Formatting                                                   |
|:-------:|:-------------------------------------------------------:|
| %H      | Hour of the day, 24-hour clock, zero-padded (00..23)    |
| %k      | Hour of the day, 24-hour clock, blank-padded (_0..23)   |
| %I      | Hour of the day, 12-hour clock, zero-padded (01..12)    |
| %l      | Hour of the day, 12-hour clock, blank-padded (_1..12)   |
| %P      | Meridian indicator, lowercase (am or pm)                |
| %p      | Meridian indicator, uppercase (AM or PM)                |
| %M      | Minute of the hour (00..59)                             |
| %S      | Second of the minute (00..59)                           |
| %L      | Millisecond of the second (000..999)                    |
| %N      | Nanosecond (9 digits)                                   |
| %3N     | Millisecond (3 digits)                                  |
| %6N     | Microsecond (6 digits)                                  |
| %12N    | Picosecond (12 digits)                                  |
| %15N    | Femtosecond (15 digits)                                 |
| %18N    | Attosecond (18 digits)                                  |
| %21N    | Zeptosecond (21 digits)                                 |
| %24N    | Yoctosecond (24 digits)                                 |

| Seconds Formatting                                                                        |
|:-------:|:-------------------------------------------------------------------------------:|
| %s      | Number of seconds since 1970-01-01 00:00:00 UTC                                 |
| %Q      | Number of milliseconds since 1970-01-01 00:00:00 UTC                            |

| Time Zone Formatting                                                                      |
|:-------:|:-------------------------------------------------------------------------------:|
| %z      | Time zone as hour and minute offset from UTC (e.g. +0900)                       |
| %:z     | Time zone hour and minute offset from UTC with a colon (e.g. +09:00)            |
| %::z    | Time zone hour, minute and second offset from UTC (e.g. +09:00:00)              |
| %:::z   | Time zone hour, minute and second offset from UTC (e.g. +09, +09:30, +09:30:30) |
| %Z      | Time zone abbreviation name or something similar information                    |

| Weekday Formatting                                              |
|:-------:|:-----------------------------------------------------:|
| %A      | The full weekday name (e.g. Sunday)                   |
| %^A     | The full weekday name uppercased (e.g. SUNDAY)        |
| %a      | The abbreviated weekday name (e.g. Sun)               |
| %^a     | The abbreviated weekday name uppercased (e.g. SUN)    |
| %u      | Day of the week starting Monday (1..7)                |
|%w       | Day of the week starting Sunday (0..6)                |

| Week Formatting                                                     |
|:-------:|:---------------------------------------------------------:|
| %G      | The week-based year                                       |
| %g      | The last 2 digits of the week-based year (00..99)         |
| %V      | Week number of the week-based year (01..53)               |
| %U      | Week number of the year. Week starts with Sunday (00..53) |
| %W      | Week number of the year. Week starts with Monday (00..53) |

| Flags 1                                             |
|:-------:|:-----------------------------------------:|
| -       | Don't pad a numerical output              |
| _       | Use spaced for padding                    |
| 0       | Use zeros for padding                     |
| ^       | Upcase the result string                  |
| #       | Change case                               |
| :       | Use colons for %z                         |

| Literal Strings                                     |
|:-------:|:-----------------------------------------:|
| %n      | Newline character (\n)                    |
| %t      | Tab character (\t)                        |
| %%      | Literal '%' character                     |

| Combination                                                         |
|:-------:|:---------------------------------------------------------:|
| %c      | Date and time (%a %b %e %T %Y)                            |
| %D      | Date (%m/%d/%y)                                           |
| %F      | The ISO 8601 date format (%Y-%m-%d)                       |
| %v      | VMS date (%e-%b-%Y)                                       |
| %x      | Same as %D                                                |
| %X      | Same as %T                                                |
| %r      | 12-hour time (%I:%M:%S %p)                                |
| %R      | 24-hour time (%H:%M)                                      |
| %T      | 24-hour time (%H:%M:%S)                                   |
| %+      | date(1) (%a %b %e %H:%M:%S %Z %Y)                         |


<style>
  table {
    display:table;
    width: 100%;
  }
  table th:nth-of-type(2) {
    width: 70%;
  }
</style>