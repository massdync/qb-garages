# qb-garages

This is a modified version of qb-garages with support of storing vehicles' properties

A new column named `properties` is added into the table

When a player stores their vehicle, the script will call `QBCore.Functions.GetVehicleProperties()` and store the result as json encoded string into the database

When a player take their vehicle out from the garage, the script will fetch the json encoded string from the database then decode it into table, and eventually apply it to the vehicle with `QBCore.Functions.SetVehicleProperties()` 

<hr>

**Public Garages**
* Park owned cars in public garages.
* You can only parks vehicles that you own in public garages. 

![image](https://github.com/qbcore-framework/qb-garages/assets/57848836/b56344ea-a902-4c07-9ae6-4984486648d2)

**House Garages**
* Park owned cars in house garages. To add a house garage, you must have the realestate job and do /addgarage.
* You can only parks vehicles from persons that have the key in a house garage. 
* You can take every vehicle from the house garages to which you have the key. 
* You can only parks ground vehicles in house garages. 

**Gang Garages**
* Allows for gangs to have their own garages.
* You can parks every vehicle that is owned by gang members in gang garages. 
* You can take every vehicle from the gang garages. 

**Job Garages**
* Allows jobs to have garage specific.
* You can parks every vehicle that is owned by someone in job garages. 
* You can take every vehicle from the job garages. 

**Depot Garages**
* Allows depot cars to be retreived from here. Cops can do /depot [price] to send a car to the depot.

**Auto Respawn Config**
* If set to true, cars that are currently outside will be placed in the last garage used.
* If set to false, cars that are currently outside will be placed in the depot.

**Shared garages Config**
* If set to true, Gang and job garages are shared.
* If set to false, Gang and Job garages are personal.

**Configurations**
* You can only parks ground vehicles in garages of type "car" in config. 
* You can only parks water vehicles in garages of type "sea" in config. 
* You can only parks air vehicles in garages of type "air" in config. 
* Vehicle types and jobs or gang can be mixed in config.

**Blips and names**
* Blips and names are modifiable for each garage. 


# License

    QBCore Framework
    Copyright (C) 2021 Joshua Eger

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <https://www.gnu.org/licenses/>

