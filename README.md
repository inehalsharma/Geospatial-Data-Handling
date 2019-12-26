# Geospatial-Data-Handling-
Implementing spatial queries using Postgres SQL on Google Cloud Platform

In this project, we are going to work with spatial data - we will create some data, visualize it, do queries on it, and visualize the query results.

1.We create (generate) latitude,longitude pairs (ie. spatial coordinates) for 7 locations. One of those will be where our home/apartment/dorm room is. The other six would have to be spread out - at least 100 feet between adjacent locations (and at most 200 or 300 or even 400 feet between neighboring points)

2. Now that we have 7 coordinates and their label strings, we are going to create a KML file (.kml format) out of them using a text editor. Specifically, each location will be a 'placemark' in our .kml file (with a label, and coords). 

3.(a)Compute the convex hull for our 7 points [a convex hull for a set of 2D points is the smallest convex polygon that contains the point set]. Use the query's result polygon's coords, to create a polygon in our .kml file. Load this into Google Earth, visually verify that the 7 points are inside the convex hull, then take a screenshot. 
(b) Compute the three nearest neighbors of the home/apt/dormroom location. Use the query's results, to create three line segments in the .kml file: line(home,neighbor1), line(home,neighbor2), line(home,neighbor3). Verify this looks correct using Google Earth, take a snapshot.
4. Using SGM 123 as the center, compute a set (sequence) of lat-long (ie. spatial) co-ordinates that lie along a pretty Spirograph(TM) curve :) Create a new KML file with these points, visualize it on Google Earth.
