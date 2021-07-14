# Data

Data downloaded from the ONS (Operador Nacional do Sistema Elétrico) [webpage](http://www.ons.org.br/paginas/resultados-da-operacao/historico-da-operacao).
All data is daily (except where otherwise noted), and goes from January 1, 2016 to December 31, 2020. 
All data is at the closest level to Barra Bonita, Tiete, Sao Paulo in the Sudeste/Centro-Oeste subsystem. 

## Constants

The installed generation capacity for Barra Bonita: 140 MW.

## The csv files

### monthly_df.csv
All of the variables that we had on a monthly scale
- **Date**: Month and Year
- **Capacity**: Substation Transformation Capacity (MVA).  Data from Southwest/Central Region.  Units and meaning are unclear at this time
- **Length**: Total length of transmission lines in Brazil.  Units: km
- **marginal_cost_monthly_mean**: Contains the monthly mean of the marginal cost of operation in the Sudeste/Centro-Oeste subsystem.
The marginal cost refers to the cost of producing an extra KWh of energy. Date averaged from weekly means, where binning is by the month that the last day of the week falls into.  Last entry of weekly info dropped (falls into 2021)


-----------------------#daily data-------------------------------------

### aggragate_daily_data.csv
Combines all daily data we have collected into one csv organzied by date. Note that after reading the csv, the date information needs to be set as dates using as.Date(). Furthermore, the space variable is implicit to the column name since each date as data for Barra Bonita and other locations.

Space Scale: ill-defined 

Time Scale: daily

### Variables 

-***date***: YYYY-MM-DD

-***affluent_natural_energy_southeast***: affluent natural energy for Southeast/Central-west region in MWmed

-***effluent_flow***: effluent flow in m^3/s

-***influent_flow***: influent flow in m^3

-***volume_used***: percent volume used

-***poured_flow***: poured flow in m^3/s

-***turbine_flow***: turbine flow in m^3/s

-***water_level***: water level in meters

-***energy_generated***: energy generated in GWh

-***energy_stored***: energy stored in GWH throughout the Southeast/Central-west region

-***physical_energy_exchange***: physical energy exchanged at boundry lines of Southeast/Central-west region in GWh

-***liquid_energy_exchange***: liquid energy exchanged at boundry lines of Southeast/Central-west region in GWh

-***affluent_natural_energy_tiete_basin***: affluent natural energy for the tiete basin region in MWmed

-***maximum_demand***: maximum demand in Southeast/Centra-west region in MW

-***energy_charge***: energy charge in GWh



-----------------------#Barra Bonita-----------------------------------
### Influent_Flow.csv
Average(?) rate of flow into the reservoir per day

Space Scale: Barra Bonita

Time scale: daily

#### Variables
- **Date**: Day.
- **Influent_Flow**: Average(?) rate of flow into the reservoir per day in *m^3/s*.

### Poured_Flow.csv
Average(?) rate of flow released by reservoir through surface spillways and/or bottom spillways.

Space Scale: Barra Bonita

Time scale: daily

#### Variables
- **Date**: Day.
- **Effluent_Flow**: Average(?) rate of flow released by reservoir per day in *m^3/s*.

### Turbine_Flow.csv
Average(?) rate of flow that passes through the turbines of a hydroelectric plant.

Space Scale: Barra Bonita

Time scale: daily

#### Variables
- **Date**: Day.
- **Effluent_Flow**: Average(?) rate of flow that passes through the turbines per day in *m^3/s*.

### Effluent_Flow.csv
Average(?) rate of flow leaving hydroelectric plant.

Space Scale: Barra Bonita

Time scale: daily

#### Variables
- **Date**: Day.
- **Effluent_Flow**: Average(?) rate of flow leaving hydroelectric plant per day in $m^3/2$.

### Percent_Vol_Used.csv
Percentage of useful(?) volume. (Translation needed; what does "Volume Útil" mean?)

Space Scale: Barra Bonita

Time scale: daily

#### Variables
- **Date**: Day.
- **Percent_Vol_Used**: meaning tbd.

### group_waterlevel_data.csv

Daily water level measurements at Barra Bonita

Space Scale: Barra Bonita

Time Scale: Daily 

- **date**: YYYY-MM-DD
- **waterlevel**: meters (probably height from sealevel)


### nrg_generated.csv
Amount of energy generated (GWh), measured daily at Barra Bonita, 1/1/16 to 12/31/20

Space Scale: Barra Bonita

Time scale: Daily

- **Date**: Date and time of measurement
- **Energy Generated (GWh)**: Amount of energy generated (GWh)



-----------------------#Souteast/Central-West--------------------------

### Marginal_Cost_Weekly_Mean.csv
Contains the weekly mean of the marginal cost of operation in the Sudeste/Centro-Oeste subsystem.
The marginal cost refers to the cost of producing an extra KWh of energy. 

Space Scale: Southwest/CentralWest Region

Time scale: weekly

#### Variables
- **Start_of_week**: Date of the start of the week. 
- **Date**: Last day of the corresponding week. 
- **Marginal_cost_mean_week**: Weekly mean marginal cost, in Brazilian Reals per MWh. 

### Stored_Energy.csv
Contains the energy in storage at the Sudeste/Centro-Oeste subsystem each day.

Space Scale: Southwest/CentralWest Region

Time scale: daily

#### Variables
- **Date**: Day.
- **Stored_energy**: energy in storage at the given day, in GWh. 

(**Note:** to compute the energy produced on day *x* that was stored that day, we would need to compute the difference between the values of *Stored_enegy* at days *x* and *x-1*.)  


### group_energy_exchange_data.csv

Daily energy exchange measurments at boundry lines of the southeast/central energy region.

Space Scale: Southeast/central

Time Scale: Daily



- **date**: YYYY-MM-DD
- **physical_energy_exchange**: physical energy exchange measured at boundery lines of southeast district (GWh)
- **liquid_energy_exchange**: liquid energy exchange measured at boundery lines of southeast district (GWh)



### nrg_capacity.csv
Subsytem energy capacity for Southwest/Central Region, 1/1/16 to 12/31/20

Space Scale: Southwest/Central Region

Time scale: monthly

Units and meaning are unclear for Capacity
- **Date**: Date and time of measurement (Month and Year)
- **Capacity**: Substation Transformation Capacity (MVA)


### Affluent_Natural_Energy_SE:MidW.csv

Space: Southeast/MidWest

Time:Daily

Units: MWmed

### Maximum_Demand.csv

Space: Southeast/MidWest

Time: Daily

Units: MW

### energy_charge.csv

Space: Southeast/central west
Time: Daily, 1/1/2016-12/31/2020

day to day energy charge (units: GWh)

### hourly_load.csv

space: Southeast/central west
Time: Daily and hourly, 1/1/2016-12/31/2020

day-to-day hourly_load (units: MWh/h)

------------------------------#Misc------------------------

### Affluent_Natural_Energy_TieteBasin.csv

Space: Tiete Basin

Time: Daily

Units: MWmed



### TransmissionLines_Length.csv

Space: Brazil

Time: Monthly

Units: km


