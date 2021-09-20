# Lubridate-ggplot-date-helpers

The details of the codeset and plots are included in the attached Microsoft Word Document (.docx) file in this repository. 
You need to view the file in "Read Mode" to see the contents properly after downloading the same.

A Brief Introduction
=====================
This post collates a couple of functions to help with dates. I often work with daily data which spans multiple years, but want to visualise annual patterns. To do this I can extract the julian day for each date – i.e. the day of the year. Here are a couple of ways to do this:

# Olden days
format(Sys.Date(), format="%j")

# Tidyverse
library(lubridate)
yday(Sys.Date())

This site is a great resource for more date formats. Otherwise, you can view the lubridate website for guides.

Great, so far. However, most folk like their axis labels spelt out for them and prefer to see month labels on an annual axis instead of a numeric day. Let’s grab some data to demonstrate. 

Python strftime Documentation: https://strftime.org/
