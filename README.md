# Inertia Systems PHP Code Sample
This is a Code Sample project for your Inertia Systems job application!
This sample should take approximately **1-2 hours** to complete. 

### **Submit your code as a `.zip` file to your hiring contact.**

Your code will be analyzed on a variety of factors, including:

    - Readability
    - Functionality
    - Accuracy

-------------
Using the included `sampledata.json` file as a data source we will have to answer a few questions.  Here is some information about the sample data:

```
{
    "inventory": { 
        "date":"2019-10-10", 
        "items":[            
            {
                "name": "shovel",  
                "need": 4,         
                "newlife": 10,     
                "replacement_cost": 14,   
                "inventory_life": [9, 5, 3, 0, 0]                         
            },
            .
            .
            .
    }
}
```
**inventory** - A JSON object that contains all of the current inventory results.

**date** - The DATE that this inventory was recorded.

**items** - The LIST of inventory items.

**name** - The NAME of the inventory item.

**need** - The amount needed of this item for one day of work.

**newlife** - The number of days a NEW item of this type will be useful.

**replacement_cost** - The COST of a NEW item of this type.

**inventory_life** - This is an ARRAY of current inventory items available.  Each number represents the remaining life of that item.  When an ITEM reaches 0, it can no longer be used.

-------

You will be creating a web app that uses PHP Scripts that accept HTTP Requests with an HTML and Javascript front-end.  It should communicate using AJAX to the PHP script back-end. Front end code will retrieve JSON responses with the information for display. You may create as many files as you need to accomplish the task in an organized manner.  Provide the ability to request and display the answer to these three questions along with any necessary inputs: 

**1. How much is our inventory worth, using straight-line depreciation of each asset.**
>For example: If an item has 10 days of life when new, and costs 100.  When there is 3 days of life left it will be worth 30, because each day costs 10.  (`100/10 = 10`)  You may round to 2 decimal places.

**2.  Daily cost of operations.  How much, using the depreciation of each asset, does each day cost us to operate.  Display daily cost per item type, and total overall cost of all the types.**

**3.  How many items need to be replaced in `X` days.  Given an integer for the number of days after the inventory date report, how many items will need to be replaced and the total costs of the order to replace them.**
>For Example:  If I give you `5` days as a parameter, it will remove `5` days of life from each item needed per day until they reach `0` and the report will tell me how many new items are required to fufill the needed inventory, and the total cost of them all.  

It is OKAY for a day to go by with not enough working items in inventory for the sake of this exercise, we simply want to reduce their remaining life to 0 and then stop counting them in the available inventory.

----
Your front end may be as simple or as complex as you want so long as it addresses the 3 questions asked above.  Use this as a chance to demonstrate your code organization skills.  You may use any framework or library you want (jQuery..etc.), however, your project should utilize the built in php web-server for execution. https://www.php.net/manual/en/features.commandline.webserver.php

**You will not be ranked on the _prettyness_ of the UI just its _functionality_**

These commands should run your project from the repository directory.
```
cd public
php -S localhost:8000
````

Thank you for applying!  

