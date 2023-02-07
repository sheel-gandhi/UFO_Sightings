# UFO_Sightings

A project on UFO sightings using JavaScript

## Purpose
 
* **Explain the strengths and weaknesses of JavaScript "standard" and JavaScript version ES6+.**
* **Describe JavaScript syntax and ideal use cases.**
* **Build and deploy JavaScript functions, including built-in functions.**
* **Convert JavaScript functions to arrow functions.**
* **Build and deploy forEach (JavaScript for loop).**
* **Create, populate, and dynamically filter a table using JavaScript and HTML**

## Overview

Dana, a data journalist is working on writing an article on UFO sightings and need our help with a detailed table of all UFO sightings with city, state, country, type, and date. Dana wants to have the ability to filter the table using multiple criteria. With the knowledge of JavaScript we will be manipulating the table and with CSS and Bootstrap, we will make the website presentable. 

## Results: 

### UFO Sighting welcome page: 

**Heading and Main Article:**

On opening the url, we land on the welcome page with the title - UFO Sightings. It will have a heading – “The Truth is Out There” with an interesting article on UFOs.

![image](https://user-images.githubusercontent.com/108366412/190507380-09b5e79f-ddfa-435e-bda0-6b630dba84e9.png)
 
**Base Table without application of filter criteria:**

The page will further have a table which will show all the UFO sightings included in the data. Note that we have set filter criteria – Date, City, State, Country, and Shape beside the table to filter the data as desired. 
![image](https://user-images.githubusercontent.com/108366412/190507430-4ea21c68-b1ed-4ca5-9f83-208bc2c93e51.png)
 
**Table upon application of filter criteria:**

Upon applying shape filter with “circle” value, we can filter the data with entries only showing UFOs with a circle shape. We are down to just 4 results from a table huge. 

This happens when we type value (“circle” in our case) in the shape placeholder field. The value which we put in, should match the case of the entries in the table. In our table, data is in lower case, hence make sure to put in the search criteria in lower case and press enter. To get the default table back, refresh the page or click the “UFO Sightings” located at the top left corner which also acts as a refresh button. 
![image](https://user-images.githubusercontent.com/108366412/190507508-2461d4a7-6756-4b46-857c-6de3287a1e9d.png)

On applying a second criterion – this time setting city to Benton, we get only one search result. It means there is only one UFO sighting in the city of Benton which was circle in shape. 
![image](https://user-images.githubusercontent.com/108366412/190507542-813cc3f1-0d20-4230-b868-bd7e2fba7c71.png)
 
## Summary:
In a summary statement, describe one drawback of this new design and two recommendations for further development.
At first sight the table does look appealing with great filter options however it does have few drawbacks and can be made more efficient by adding more features to the filter.

### Drawback
For filtering, we must know the entries included in the data in their required case. Some of the shape names included are fireball, formation, light, chevron and unknown. It may not occur to us to search for a such a specific shape. There is no drop-down list of all the possible shapes included in the table. A drop-down list for all search criteria will surely help improve user experience. 
![image](https://user-images.githubusercontent.com/108366412/190508962-121e5e44-64d5-4ad4-88fa-85f6cae0cbdc.png)


### Recommendation

1. We must know the case the entry is in. Upon first look it seems all data is in lower case but if a value is in uppercase, it may not show up with other lower-case values. In filter search, we must also put in the exact value in exact case without any extra spaces in the beginning or end to get the search result. Below is an example where in instead of putting "us" in lowercase, we have "US" which is uppercase.
![image](https://user-images.githubusercontent.com/108366412/190508982-14ce2a2a-62aa-478e-b260-93337ba60582.png)
By including “ignoreCase: false” argument, we can overcome the case sensitivity. We can use “entry => entry.trim()” to ignore any extra spaces before or after the entry. 
 
2. A count of number entries after filtering can also be added to give the user an instant figure of the entries for a specific search criterion. A small icon showing data is filtered can be also be added beside filter search to give the user idea whether data is already filtered or not without checking in each criterion if value is entered in placeholder or not.
