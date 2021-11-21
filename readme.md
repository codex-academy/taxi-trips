# Taxi trips

A local study is looking into the national mini taxi industry in South Africa and they need help analyzing some data.

Taxi's from different regions are doing various trips. Each trip has a cost and a taxi can do a trip more than once.

* Routes got a name and a fare,
* A taxi: 
	* got a reg number, 
	* can do many trips on a given route.
* Each taxi belongs to a Region - there are three regions currently Gauteng, Cape Town & Durban.

Note: tables are linked with foreign keys.

Create 4 tables: a Route, Taxi, Trip & Region table. 
The trip table brings routes and taxi’s together.
Each taxi is linked to 1 region. Many taxis can be linked to the same region.

Create a Factory Function called `TaxiTrips` with the following methods:

Function name            | Description   
------------------------ | ---------------
`totalTripCount` 		 | return the total number of trips made in total               
`findAllRegions` 		     |  find all the regions              
`findTaxisForRegion` 	     |  find all the taxis for a given regions
`findTripsByRegNumber` 	 |  Find all the trips made by a given taxi - use reg number as look up
`findTripsByRegion` 	     |  Find all the trips made for a given region
`findIncomeByRegNumber`    |  List the income for each taxi - use reg number in this query
`findTotalIncomePerTaxi`   |  find the total income per taxi.
`findTotalIncome` 		 | Find the total amount received in income for all the taxis
	
The methods should use SQL to do the calculations.

We made a start for you by creating the `taxi-trips.js` file with some tests in `taxi-trips.test.js`.

Make all the tests pass in `taxi-trips.test.js` select the appropriate parameters and return data.

## Database setup

In the `sql` folder create two files.

* Create the tables using a sql script file called `sql/tables.sql`,
* Add data to the files using a file called `sql/data.sql`.

Ensure each region have 3 taxi's and that each taxi have made between 3 to 5 trips.

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

## Travis

Ensure to deploy to Travis. Add a travis badge to the readme file.

Fork and clone this repository.

# Please

* Do your own work - we will see if you are copying code,
* ask mentors if you need clarification - email them `mentors@projectcodex.co`,
* enjoy it.

