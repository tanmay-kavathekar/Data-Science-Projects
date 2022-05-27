README
------

This folder contains domestic flight data from 2015. This data has NOT been cleaned.

You'll find four files alongside this README:

* flights.csv
* sample-flights.csv
* airports.csv
* airlines.csv


flights.csv
---------------

The file contains the following columns:

YEAR				Year of the Flight Trip
MONTH				Month of the Flight Trip
DAY				Day of the Flight Trip
DAY_OF_WEEK			Day of week of the Flight Trip
AIRLINE				Airline Identifier
FLIGHT_NUMBER			Flight Identifier
TAIL_NUMBER			Aircraft Identifier
ORIGIN_AIRPORT			Starting Airport
DESTINATION_AIRPORT		Destination Airport
SCHEDULED_DEPARTURE		Planned Departure Time
DEPARTURE_TIME	 		WHEEL_OFF - TAXI_OUT
DEPARTURE_DELAY			Total Delay on Departure 
TAXI_OUT	 		The time duration elapsed between departure from the origin airport gate and wheels off
WHEELS_OFF			The time point that the aircraft's wheels leave the ground
SCHEDULED_TIME			Planned time amount needed for the flight trip
ELAPSED_TIME			AIR_TIME+TAXI_IN+TAXI_OUT
AIR_TIME			The time duration between wheels_off and wheels_on time
DISTANCE	 		Distance between two airports
WHEELS_ON	 		The time point that the aircraft's wheels touch on the ground
TAXI_IN	 			The time duration elapsed between wheels-on and gate arrival at the destination airport
SCHEDULED_ARRIVAL	 	Planned arrival time
ARRIVAL_TIME	 		WHEELS_ON+TAXI_IN
ARRIVAL_DELAY	 		ARRIVAL_TIME-SCHEDULED_ARRIVAL
DIVERTED	 		Aircraft landed on airport that out of schedule
CANCELLED	 		Flight Cancelled (1 = cancelled)
CANCELLATION_REASON	 	Reason for Cancellation of flight: A - Airline/Carrier; B - Weather; C - National Air System; D - Security
AIR_SYSTEM_DELAY	 	Delay caused by air system
SECURITY_DELAY	 		Delay caused by security
AIRLINE_DELAY	 		Delay caused by the airline
LATE_AIRCRAFT_DELAY	 	Delay caused by aircraft
WEATHER_DELAY	 		Delay caused by weather

About some of the time values:

* All time values are shown as integers
* Some times represent a specific time. For example, in the SCHEDULED_DEPARTURE column 55 represents 00:55 (or 12:55 AM), 1345 represents 13:45 (or 1:45 PM) and both 61 or 2401 would be invalid
* Other time values represent a delay in minutes. For example, in the DEPARTURE_DELAY column, 0 means the flight left on time, 61 would mean the flight was 61 minutes late departing and -34 means the flight left 34 minutes early.

sample-flights.csv
------------------

This contains a random sample of 6000 flights from the full flights.csv file.

Columns will be the same as flights.csv.

airlines.csv
-------------

This file contain the IATA airline codes and airline names

airports.csv
------------

This file contains the IATA airport codes, airport name assorted location data (including city, state, latitude and longitude)
