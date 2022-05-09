# UFOs
For learning Java Script from Module 11

## Project Overview
Dana wants build a webpage with dynamic table to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. Table filters dana considers are for the date, city, state, country, and shape

## Resources
- javascript, HTML, Bootstrap, Visual Code, Browser Edge
- data for table from data.js, index.html

## Challenge Overview
Prerequisite:
1.  Download the ufo_starterCode.ipynb file 


## Deliverable 1:  Filter UFO sightings on multiple criteria

Follow the instructions below and the numbered comments in the starter code to complete Deliverable 1.

1.	Download the ufo_starterCode.js, rename it app.js, and place it in the js folder of your UFOs GitHub repository. The starter code includes the code used to 
    populate the table from this module.
2.	In the index.html file, remove the list (<li></li>) element that creates the button.
3.	Create four more list elements: city, state, country, and shape. These will be similar to the "Enter Date" list element. Each element should have the same "id" 
    as the object properties in the data.js file.
4.  In the app.js file, create an empty filters variable to keep track of all the elements that change when a search is entered. This variable will be used in Step  
    5 to store the property “id” and the value that was entered from user input.
5.  Next, you will need to write code for two functions whose names we’ve provided in the starter code, updateFilters() and filterTable().
6.  The updateFilters() function will replace your handleClick() function and update the filters variable you created in Step 1.
7.  The filterTable() function will filter the table data by the value that is entered for the "id" that has changed.
8.  At the end of the starter code (located before the buildTable(tableData) function), modify the event listener from this module so that it detects a "change" on 
    each input element and calls the updateFilters() function.
9.  Inside updateFilters function, you’ll write code in Steps 4-5 to update the filters based on user input.
10. Create a variable that saves the element that was changed using d3.select(this).
11. Create a variable that saves the value of the changed element’s property.
12. Create a variable that saves the attribute of the changed element’s id.
13. Write an if-else statement that checks if a value was changed by the user (variable from Step 11). If a value was changed, add the element’s id (variable from 
    Step 12) as the property and the value that was changed to the filters variable you created in Step 1. If a value was not entered, then clear the element id from the filters variable.
14. Inside the updateFilters() function, call the filterTable() function that will be used in Step 15.
15. In the filterTable() function, write code to filter the table based on the user input that is stored in the filters variable.
15. Create a variable for the filtered data that is equal to the data that builds the table. This variable will hold the updated table data based on the user input.
16. Loop through the filters object and store the data that matches the filter values in the variable created in Step 15.
17. Rebuild the table with the filtered data by passing the variable created in Step 15.


## UFO sightings-Analysis Results
1.  

- UFO sightings initial load
    ![image_name](https://github.com/raneymjohnGit/UFOs/blob/main/static/Images/UFO_Sightings.png)

- UFO sightings with Date filter
    1.  Enter a date and press enter.
        -   The table data will be filtered on that date.
    ![image_name](https://github.com/raneymjohnGit/UFOs/blob/main/static/Images/UFO_Sightings_date_filter.png)

- UFO sightings with Date and state filter
    1.  Enter a date and state code and press enter.
        -   The table data will be filtered on that date and state.
    ![image_name](https://github.com/raneymjohnGit/UFOs/blob/main/static/Images/UFO_Sightings_dateAndState_filter.png)
 
- UFO sightings with Date,State and Shape filter
    1.  Enter a date,state code and shape press enter.
        -   The table data will be filtered on that date,state and shape.
    ![image_name](https://github.com/raneymjohnGit/UFOs/blob/main/static/Images/UFO_Sightings_DateStateShape_filter.png)

- UFO sightings with Date,State,Shape and City filter
    1.  Enter a date,state code, shape and city press enter.
        -   The table data will be filtered on that date,state, shape and city. 
    ![image_name](https://github.com/raneymjohnGit/UFOs/blob/main/static/Images/UFO_Sightings_DateStateShapeCity_filter.png)

- UFO sightings with country filter
    1.  Enter a country code press enter.
        -   The table data will be filtered on that country. 
    ![image_name](https://github.com/raneymjohnGit/UFOs/blob/main/static/Images/UFO_Sightings_Country_filter.png)

## UFO sightings-Analysis Summary

Drawbacks:
1.  We have limited data available with data from countries like US and Canada only.
2.  The UFO sightings are pretty old and from the year 2010, that too from first 13 days only.
3.  There is no clear button to clear the search.
4.  The search is done by one at a time.  

Additional recommendations:

1.  We could have added a chart also for better presentation.
2.  instead of type in the values, we could have added a drop down and select from the list.