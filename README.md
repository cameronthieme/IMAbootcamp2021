# Predicting Hydroelectricity generation in Brazil
## [IMA Bootcamp 2021](https://www.ima.umn.edu/boot-camp): project suggested by Cargill

### Team Members:
-  Ana Chavez Caliz (PSU)
- Jürgen Kritschgau (ISU)
- Francisco Martinez (OSU)
-  Avishek Mukherjee (UDel)
-  Smita Praharaj (UMC) 
-  Cameron Thieme (UMN)
-  Jennifer Zhu (TAMU)

## The Project
Taking into account the energy needed by Cargill to operate in Brazil, we investigate the effective-ness of the option for Cargill to buy energy from hydroelectric power grids vs producing its ownpower sources.  We choose hydroelectricity since it accounts for more than 45 percent of the totalenergy generated in Brazil.  To make our model simple, we eliminated the pricing of electricity sincethe pricing depends on various government regulations and policies.  Instead, we focus on forecast-ing the amount of electricity that will be generated in the future, taking into account variables likerain, maximum demand and so on.We start off by investigating a single reservoir at Barra Bonita for its simplicity.  After a prelimi-nary data exploration, given the weak correlation between energy generated at Barra Bonita againstother variables of interest and lack of seasonality, we realize that moving to a subsystem level or acollection of high energy-generating power plants on a monthly timescale will be beneficial for theanalysis.

## The Data
We use publicly available data from many Brazilian entities:

- Dam and power grid data obtained from the [ONS](http://www.ons.org.br/paginas/resultados-da-operacao/historico-da-operacao)

  - Daily, weekly, monthly scale depending on variable 
  - Generally complete, with few missing entries 

- Weather data from mixed sources ( [INMET](https://portal.inmet.gov.br/dadoshistoricos) and [CPTEC](https://bacias.cptec.inpe.br/) )

  - aggregated to basin, state, or region 
  - Daily, weekly, monthly scale 
  - Averaged by dropping “NA”s 

## Our Results
The following Google Slide contains our results. 
