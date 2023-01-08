# Data Description

Select query lists copied from the data_description file:

### Table **flights**

```sql
SELECT
    fl_date
  , mkt_unique_carrier
  , branded_code_share
  , mkt_carrier
  , mkt_carrier_fl_num
  , op_unique_carrier
  , tail_num
  , op_carrier_fl_num
  , origin_airport_id
  , origin
  , origin_city_name
  , dest_airport_id
  , dest
  , dest_city_name
  , crs_dep_time
  , dep_time
  , dep_delay
  , taxi_out
  , wheels_off
  , wheels_on
  , taxi_in
  , crs_arr_time
  , arr_time
  , arr_delay
  , cancelled
  , cancellation_code
  , diverted
  , dup
  , crs_elapsed_time
  , actual_elapsed_time
  , air_time
  , flights
  , distance
  , carrier_delay
  , weather_delay
  , nas_delay
  , security_delay
  , late_aircraft_delay
  , first_dep_time
  , total_add_gtime
  , longest_add_gtime
FROM flights;
```

### Table **passengers**

```sql
SELECT
    departures_scheduled
  , departures_performed
  , payload
  , seats
  , passengers
  , freight
  , mail
  , distance
  , ramp_to_ramp
  , air_time
  , unique_carrier
  , airline_id
  , unique_carrier_name
  , region
  , carrier
  , carrier_name
  , carrier_group
  , carrier_group_new
  , origin_airport_id
  , origin_city_market_id
  , origin
  , origin_city_name
  , origin_country
  , origin_country_name
  , dest_airport_id
  , dest_city_market_id
  , dest
  , dest_city_name
  , dest_country
  , dest_country_name
  , aircraft_group
  , aircraft_type
  , aircraft_config
  , month
  , year
  , distance_group
  , class
FROM passengers;
```

### Table **fuel_comsumption**

```sql
SELECT
    month
  , airline_id
  , unique_carrier
  , carrier
  , carrier_name
  , carrier_group_new
  , sdomt_gallons
  , satl_gallons
  , spac_gallons
  , slat_gallons
  , sint_gallons
  , ts_gallons
  , tdomt_gallons
  , tint_gallons
  , total_gallons
  , sdomt_cost
  , satl_cost
  , spac_cost
  , slat_cost
  , sint_cost
  , ts_cost
  , tdomt_cost
  , tint_cost
  , total_cost
  , year
FROM fuel_comsumption;
```

### Table **flights_test**

This table consists of subset of columns from table flights. It represents flights from January 2020 which will be used for evaluation. Therefore, we are missing some features that we are not suppossed to know before the flight lands.

```SQL
SELECT
    fl_date
  , mkt_unique_carrier
  , branded_code_share
  , mkt_carrier
  , mkt_carrier_fl_num
  , op_unique_carrier
  , tail_num
  , op_carrier_fl_num
  , origin_airport_id
  , origin
  , origin_city_name
  , dest_airport_id
  , dest
  , dest_city_name
  , crs_dep_time
  , crs_arr_time
  , dup
  , crs_elapsed_time
  , flights
  , distance
FROM flights_test;
```
