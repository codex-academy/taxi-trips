# Taxi trips

A local study is looking into the national minibus taxi industry in South Africa and they need help analyzing some data.

Taxi's from different regions are doing various trips. Each trip has a cost and a taxi can do a trip more than once.

* Routes got a name and a fare,
* A taxi: 
	* got a reg number, 
	* can do many trips on a given route.
* Each taxi belongs to a Region - there are three regions currently Gauteng, Cape Town & Durban.

**Note:** tables are linked with foreign keys.

Create 4 tables: 

* a Route, 
* Taxi, 
* Trip 
* & Region table. 

The trip table brings routes and taxi’s together.
Each taxi is linked to 1 region. Many taxis can be linked to the same region.

## Factory Function

Create a Factory Function called `TaxiTrips` with the following methods:

Function name            | Description   
------------------------ | ---------------
`totalTripCount` 		 | return the total number of trips made               
`findAllRegions` 		     |  find all the regions              
`findTaxisForRegion` 	     |  find all the taxis for a given region - use region name as look up
`findTripsByRegNumber` 	 |  Find all the trips made by a given taxi - use reg number as look up
`findTripsByRegion` 	     |  Find all the trips made for a given region - use the region name as lookup
`findIncomeByRegNumber`    |   The total income for a taxi - use reg number in this query
`findTotalIncomePerTaxi`   |  find the total income for each of the taxis (a total for each taxi)
`findTotalIncome` 		 | Find the total amount received in income from all the taxis (one amount)
`findTotalIncomeByRegion`  | Find the total amount income for each of the regions
	
The methods should use SQL to do the calculations.

We made a start for you by creating the `taxi-trips.js` file with some tests in `taxi-trips.test.js`.

Make all the tests pass with, your data in the database, in `taxi-trips.test.js` use the appropriate parameters and return data. The tests are not setup using specific data. You need to make sure each test tests the appropriate things.

## Database setup

In the `sql` folder create two files.

* Create the tables using a sql script file called `tables.sql`,
* Add data to the tables using a file called `data.sql`.

Ensure each region have 3 taxi's and that each taxi have made between 3 to 5 trips.

Ensure that the taxi registration numbers are appropriate for the region they are operating in.

Here are some example routes:

### Cape Town

* Cape Town - Bellville
* Cape Town - Gugulethu
* Cape Town - Langa

### Gauteng

* Sandton - Randburg
* Alexandra - Sandton
* Sandton - Midrand

### Durban

* Umlazi - Durban Central
* Durban Central - Umhlanga Rocks
* Durban Central - Umbilo

You can find more information on Taxi routes at [taximap](http://taximap.co.za/).

## Planning

* Do planning in Kanbanflow for 30 minutes - share your Kanbanflow link to us.
* Do a Problem Solving Template (PST) and share it.

Send an email with a subject of `My planning` to `mentors@projectcodex.co` this should includes link to your planning on your KanbanFlow board and your PST.


## Travis

Ensure to deploy to Travis. Add a travis badge to the readme file.

Fork and clone this repository.

# Please

* Do your own work - we will see if you are copying code.
* Ask mentors if you need clarification - email them `mentors@projectcodex.co`.
* Enjoy it!

