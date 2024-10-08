---
lang: en
title: 'Timewarrior - Duration Syntax'
viewport: 'width=device-width, initial-scale=1'
hide_toc: true
---

# Syntax: Duration

Timewarrior supports the following duration formats based on ISO-8601:

```console
'P' [nn 'Y'] [nn 'M'] [nn 'D'] ['T' [nn 'H'] [nn 'M'] [nn 'S']]
PnnW
```

Examples:

```console
P1Y           1 year
P1.5M         1.5 months
PT1S          1 second
PT4.5H        4.5 hours
PT4H30M       4.5 hours
P600D         600 days
P3W           3 weeks
P1Y1DT1H1M1S  1 year and 25 hours, 61 seconds (imprecise term)
```

Note that the year and month terms are imprecise, being defined as 365d and 30d respectively.
For precision use the other terms.

In addition to the standard duration formats, the following are supported:

```console
n[.n]<unit>
```

Where the `<unit>` is one of:

```console
annual
biannual
bimonthly
biweekly
biyearly
daily
days, day, d
fortnight
hours, hour, hrs, hr, h
minutes, minute, mins, min
monthly, months, month, mnths, mths, mth, mos, mo, m
quarterly, quarters, quarter, qrtrs, qtr, q
semiannual
sennight
seconds, second, secs, sec, s
weekdays
weekly, weeks, week, wks, wk, w
yearly, years, year, yrs, yr, y
```

Examples:

```console
1hour         60 minutes
1.5h          90 minutes
3mo           3 months
10d           10 days
```

Note that the year, quarter and month terms are imprecise, being defined as 365d, 91d and 30d respectively.
For precision use the other terms.
