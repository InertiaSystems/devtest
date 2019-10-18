# Inertia Systems Code Sample
This is a Code Sample project for your Inertia Systems job application!
This sample should take approximately **1 hour** to complete. 

Your code will be analyzed on a variety of factors, including:

    - Readability
    - Functionality
    - Accuracy

Submit your code as a `.zip` file to your hiring contact.

-------------

You will be creating a simple JSON API with a HTML/Javascript front-end.

Using the included `sampledata.json` file as a data source we will have to answer a few questions.  Here is some information about the sample data:

```
{
    "equipment": { 
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
**equipment** - A JSON object that contains all of the current inventory results.

**date** - The DATE that this inventory was recorded.

**items** - The LIST of inventory items.

**name** - The NAME of the inventory item.

**need** - The count of this item that is needed for one day of work.

**newlife** - The number of days a NEW item of this type will be useful.

**replacement_cost** - The COST of a NEW item of this type.

**inventory_life** - This is an ARRAY of current inventory items available.  Each number represents the remaining life of that item.  When an ITEM reaches 0, it can no longer be used.

-------

Your task is to create an API that answers the following questions with JSON responses to a basic front end display.

1. How much is our inventory worth, using straight-line depreciation of each asset.  
>For example: If an item has 10 days of life when new, and costs 100.  It will be worth 30 when there is 3 days left of life, as each day costs 10.  (`100/10 = 10`)

2.  Daily cost of operations.  How much, using the depreciation of each asset, does each day cost us to operate.

3.  How many items need to be replaced in `X` days.  Given an integer for the number of days after the inventory date report, how many items will need to be replaced and the total costs of the order to replace them.
>For Example:  If I give you `5` days as a parameter, it will remove `5` days of life from each item needed per day until they reach `0` and the report will tell me how many new items are needed to order to return to the needed inventory, and the cost of them all. 

----
Your front end may be as simple or as complex as you want so long as it addresses the 3 questions asked above.  Use this as a chance to demonstrate your front-end skills.  You may use any framework or library you want, however, your project should utilize the built in php web-server for execution. https://www.php.net/manual/en/features.commandline.webserver.php

```
cd public
php -S localhost:8000
````

Thank you for applying!  
