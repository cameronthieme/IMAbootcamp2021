### aggragate_daily_data.csv
Combines all daily data we have collected into one csv organzied by date. Note that after reading the csv, the date information needs to be set as dates using as.Date(). Furthermore, the space variable is implicit to the column name since each date as data for Barra Bonita and other locations.

Space Scale: ill-defined 

Time Scale: daily

### Variables 

-***date***: YYYY-MM-DD

-***effluent_flow***: effluent flow in m^3/s

-***influent_flow***: influent flow in m^3

-***volume_used***: percent volume used

-***poured_flow***: poured flow in m^3/s

-***turbine_flow***: turbine flow in m^3/s

-***water_level***: water level in meters

-***energy_generated***: energy generated in GWh

-***energy_stored***: energy stored in GWH throughout the Southeast/Central-west region

-***maximum_demand***: maximum demand in Southeast/Centra-west region in MW

-***energy_charge***: energy charge in GWh



------------------BARRA_BONITA-----------------------------------

### Influent_Flow.csv

- **Unit** : m^3/s
- **TimeScale** : daily
- **Duration** : 1/1/1999-7/13/2021

### Effluent_Flow.csv

- **Unit** : m^3/s
- **TimeScale** : daily
- **Duration** : 1/1/1999-7/13/2021

### Turbine_Flow.csv

- **Unit** : m^3/s
- **TimeScale** : daily
- **Duration** : 1/1/1999-7/13/2021


### Poured_Flow.csv

- **Unit** : m^3/s
- **TimeScale** : daily
- **Duration** : 1/1/1999-7/13/2021

### Percent_Vol_Used.csv

- **Unit** : %
- **TimeScale** : daily
- **Duration** : 1/1/1999-7/13/2021

### group_waterlevel_data.csv

- **Unit** : m
- **TimeScale** : daily
- **Duration** : 1/1/1999-7/13/2021

### nrg_generated.csv

- **Unit** : GWh
- **TimeScale** : hourly
- **Duration** : 1/1/1999-7/13/2021



--------------------SOUTHEAST_CENTRALWEST_SUBSYSTEM-------------

### energy_charge.csv

- **Unit** : GWh
- **TimeScale** : daily
- **Duration** : 1/1/1999-7/13/2021

### Maximum_Demand.csv

- **Unit** : MW
- **TimeScale** : daily
- **Duration** : 1/1/1999-7/13/2021

### hourly_load.csv

- **Unit** : MWh/h
- **TimeScale** : hourly
- **Duration** : 1/1/1999-7/13/2021

### Stored_Energy.csv

- **Unit** : GWh
- **TimeScale** : Daily
- **Duration** : 1/1/2000-7/13/2021


