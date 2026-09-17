# POWER-BI-ASSIGNMENT 
## Session 7 - Task 4 - Query Dependencies
The boxes represent the different queries or tables used in the Power BI report, while the arrows show how one query depends on another. The Merge1 query depends on the Restaurants and Customer Reviews queries, and the Append1 query depends on the This Month and Last Month order queries. The IPL_Match_Scores query is created using the Folder Combine process, which uses the Transform File, Sample File, and Transform Sample File queries to combine multiple IPL files into one table.

## Session 8 - Task 4 - Many to Many Relationship
The Users and Playlists tables have a many-to-many relationship because multiple users can collaborate on multiple playlists. The Collaborators table acts as a bridge table, with one-to-many relationships from Users and Playlists to Collaborators, allowing Power BI to correctly handle the many-to-many scenario.

## Session 8 - Task 5 - Relationship Fix
The Orders table was not correctly connected to the Dish table, which caused incorrect totals when analyzing orders by dish. I created an active one-to-many relationship using DishID, with Dishes on the one side and Orders on the many side, and identified an unmatched DishID (999) in the Orders table that should be corrected in the source data.
