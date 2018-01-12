Authors: Alexander (Xander) Riga, Abdul

# Assumptions 

1. Stations coordinate are available.
2. Vessel capacity is available
3. Number of sold ticket is known
4. Number of  berth is available
5. Number of occupied berth is known

From now each of those assumption will be referred in this document by **An**, n being the number of the assumption.

# What type of dataset is at our disposal?

We are given  *tables* containing vessels routing schedule grouped by routes and days of week. Each item of a table represent routing information with attributes of the *Vessel* which travels from station *A* at *Departure* time to station *B* at *Arrival* time. 

This dataset has mixed of  different types of attributes. For instance there are:

- Categorical attributes: vessels and stations names
- Ordered ordinal cyclic attribute: the day of week
- Ordered quantitative attributes: times

This dataset can also be seen as spatial with respect of station geographical position (**A1**).

# Why the need for a visualization?

There are some need (from Seaspan) that motivate to build a visualization of this dataset. Precisely, the visualization should enable, at least, to  

1. Adapt schedules based on current load information 
2. Manual control the schedule
3. Examine possible schedule by a visual way 
4. Visualize  the schedule of each vessel
5. Visualize The load of each vessel
6. Visualize the berth Occupation evolution

From now each of these needs will be referred in this document by **Nk**, k being the number of the need.

# How 

For the sake of clarity and efficiency we choose to provide two complementary visualization support. The first one is focused on vessel schedule and the second on routing information. Those are dynamic visualization connect to dataset. 

### Vessel Time View

This visualization represents each vessel schedule information around a 24h clock. It has the merit to pop out instantly the working/free time of vessel for each day of the week. It also address answer for those needs  **N1, N2, N3,  N4**. 

**Pitfalls** Lack of N5 and N6 and details.

### Vessels Routing View

This visualization focuses on vessels' routing visualization.  In addition of the **N1 - N4**, it also responds to those need:

- **N5** : with the help of those assumptions **A2** and **A3**. We choose to use circle progress bar to repesente the load of the vessel because we want to promote global view (cf. how full is...) over the detail one.
- **N6**: With the help A4 and A5 assumption.

**Pitfalls**: This is a daily routing view. It is difficult to have a weekly comparision. This pitfall can be partially resolve with the vessel time view
