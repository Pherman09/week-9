How saturated is the retail market in different areas of Philadelphia?

Streamlining store location site selection analysis would help commercial developers

I have an excel spreadsheet with the names and locations of every retail business in Philadelphia organized by NAICS code. There is a different NAICS code for clothing retail, bars, supermarkets, etc.
I'll have to convert the spreadsheet into a CSV then into GeoJSON, probably by using Ogre.

The website I'm envisioning would have the user enter a Philadelphia address and choose a type of store they're interested in opening from a dropdown menu. Then using Turf, I would either:
1. Generate a hex grid with each hex representing the density of the type of stores they're interested in.
2. Or, more likely, measure the distance to the nearest X number of stores of that type.
It would also be really great to overlay this with the OpenDataPhilly zoning layer. The user could get an
error thrown at them if the address they enter is not in a commercially zoned area. The income of the census tract would also be of interest to commercial developers, and any other census data related to consumer spending. Point is, eventually the end user would receive a score assigned to the address they enter, representing how likely a store opened at that address would succeed. I don't know much about store location theory, but it might actually be synergistic in some cases for stores of a similar type to be located near one another. This is certainly the case for clothing retailers, but NOT the case for supermarkets, for instance.

Walkscore.com does something like what I'd like my site to do. Instead of assigning an address a score based on it's retail density, however, walkscore assigns scores based on "walkability" weighing factors like access to public transportation.
https://www.walkscore.com/

As far as layout is concerned: I really love the look of http://museumstat.org/
I'd like my website to look similarly, a logo and search bar on the header, a map in the middle of the page,
and some graphs and charts at the bottom of the page. More than just assigning a retail development score, the website should present information about zoning, local demographics, and maybe even the names of the nearby competitor stores. I used Chart.js on the midterm, but I'm interested in starting to mess around with D3 for my visualizations this time around.

As far as anticipated problems are concerned:
I was lucky enough to have a great team at the Code for Democracy Hackathon who really helped me out with geocoding and calling the Census (and other) APIs. This is a Turf heavy assignment, and I'm not that well versed in Turf yet, especially the intersection tool.
The biggest problem I can foresee at the moment is how to build retail development scores that actually make sense and are helpful. It's pretty easy to just check Google Maps for similar stores to the one you're interested in opening in the area you're interested in, so I want to evaluate as many factors related to retail as possible in order to make my site worth visiting!
