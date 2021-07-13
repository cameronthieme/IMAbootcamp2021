# Data

Data downloaded from the ONS (Operador Nacional do Sistema Elétrico) [webpage](http://www.ons.org.br/paginas/resultados-da-operacao/historico-da-operacao).
All data is daily (except where otherwise noted), and goes from January 1, 2015 to December 31, 2020. 
All data is at the closest level to Barra Bonita, Tiete, Sao Paulo in the Sudeste/Centro-Oeste subsystem. 

## The csv files

### Marginal_Cost_Weekly_Mean.csv
Contains the weekly mean of the marginal cost of operation in the Sudeste/Centro-Oeste subsystem.
The marginal cost refers to the cost of producing an extra KWh of energy. 

#### Variables
- **Start_of_week**: Date of the start of the week. 
- **Date**: Last day of the corresponding week. 
- **Marginal_cost_mean_week**: Weekly mean marginal cost, in Brazilian Reals per MWh. 

### Stored_Energy.csv
Contains the energy in storage at the Sudeste/Centro-Oeste subsystem each day.

#### Variables
- **Date**: Day.
- **Stored_energy**: energy in storage at the given day, in GWh. 

(**Note:** to compute the energy produced on day *x* that was stored that day, we would need to compute the difference between the values of *Stored_enegy* at days *x* and *x-1*.)  

### Influent_Flow.csv
Average(?) rate of flow into the reservoir per day

#### Variables
- **Date**: Day.
- **Effluent_Flow**: Average(?) rate of flow into the reservoir per day in *m^3/s*.

### Poured_Flow.csv
Average(?) rate of flow released by reservoir through surface spillways and/or bottom spillways.

#### Variables
- **Date**: Day.
- **Effluent_Flow**: Average(?) rate of flow released by reservoir per day in *m^3/s*.

### Turbine_Flow.csv
Average(?) rate of flow that passes through the turbines of a hydroelectric plant.

#### Variables
- **Date**: Day.
- **Effluent_Flow**: Average(?) rate of flow that passes through the turbines per day in *m^3/s*.

### Effluent_Flow.csv
Average(?) rate of flow leaving hydroelectric plant.

#### Variables
- **Date**: Day.
- **Effluent_Flow**: Average(?) rate of flow leaving hydroelectric plant per day in $m^3/2$.

### Percent_Vol_Used.csv
Percentage of useful(?) volume. (Translation needed; what does "Volume Útil" mean?)

#### Variables
- **Date**: Day.
- **Percent_Vol_Used**: meaning tbd.

### group_waterlevel_data.csv
Region: Barra Bonita
Granularity: Daily 

Daily water level measurements at Barra Bonita

- **date**: YYYY-MM-DD
- **waterlevel**: meters (probably height from sealevel)

### group_energy_exchange_data.csv
Region: Southeast/central
Granularity: Daily

Daily energy exchange measurments at boundry lines of the southeast/central energy region.

- **date**: YYYY-MM-DD
- **physical_energy_exchange**: physical energy exchange measured at boundery lines of southeast district (GWh)
- **liquid_energy_exchange**: liquid energy exchange measured at boundery lines of southeast district (GWh)

### New_Dataset.csv
Small description
- **var1**


### nrg_generated.csv
Amount of energy generated (GWh), measured daily at Barra Bonita, 1/1/16 to 12/31/20

Space Scale: Barra Bonita

Time scale: Daily

- **Date**: Date and time of measurement
- **Energy Generated (GWh)**: Amount of energy generated (GWh)

### nrg_capacity.csv
Subsytem energy capacity for Southwest/Central Region, 1/1/16 to 12/31/20

Space Scale: Southwest/Central Region

Time scale: monthly

Units and meaning are unclear for Capacity
- **Date**: Date and time of measurement (Month and Year)
- **Capacity**: Substation Transformation Capacity (MVA)
