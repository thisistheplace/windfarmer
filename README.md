# windfarmer
This is a Python Flask app intended to use public APIs to provide an interactive
viewer / google maps overlay to help figure out where a good place to become a wind
farmer is...

The public APIs used are:
- windy API
- metoffice API
- CEDA archive

The method uses Windy API to get wind data at locations, matches up with what3words, and databases the windspeeds against the what3words names.
Runs every 2 hours.
Data which is > 10 years old is averaged per week from 1 day averages.
Data which is > 2 years old is averaged per day from 2 hour averages.
Recent data is stored per 2 hours.

There's a good chance a lack of public APIs is going to kill this...
