Authors: Alexander (Xander) Riga, Abdul

Assumptions:

       This model assumes that the sailings are static and that they will not change the ships on each route, the times of the sailings, 
       or the locations of the stations

What:

We are given a static table of data with:

   Categorical attributes: 
   
      The vessel, and station names

   Ordered attributes:

      Ordinal: The days of the week(cyclic)
		
      Quantitative: The times of the sailings(sequential)

   Spatial:

      The locations of the stations

Why:

      This model is effective for identifying the sailings based on location of the stations, so it is a topology map with the edges 
      representing the routes, and the information showing the ships and their sailing times is written along the specified routes.

How might you use this?

      This would be an effective model for understanding when sailings are happening at each station. It could be upgraded to include a 
      map underneath the stations in the visualization so that it would be even more clear which stations are which. This is a very 
      strong model for being able to quickly and easily determine when the sailings are for each route.

Pitfalls:

      It can still be difficult to compare the times of various sailings from different stations. If someone wanted to see all of the 
      sailings at a certain time of day, then this model would not be very effective.
