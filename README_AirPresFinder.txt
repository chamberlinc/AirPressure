AirPresFinder.R

This file contains 3 functions: FindNearestAirPres, CollectNearestAirPres, and FindandCollect_airpres

1) FindNearestAirPres(lat, long, start_datetime, end_datetime) : this function calculates the distance between specified coordinates and all local ISD sites which have available air pressure data for the specified year range. It returns the closest site with it’s ID and attributes.

2) CollectNearestAirPres(USAF, WBAN, start_datetime, end_datetime) : this function will pull the data from a known site (specified with the USAF and WBAN codes) for the desired date range.  It returns a tibble with the date/time, air pressure in kPa and air temperature.

3) FindandCollect_airpres(lat, long, start_datetime, end_datetime) : this function combines and streamlines the previous two functions to allow pulling data from an unknown (to the researcher) site.  It prints the site description and returns a tibble with the date/time, air pressure in kPa and air temperature.

This is my first time writing code for other people to use, so feedback on style and efficiency is welcomed!
