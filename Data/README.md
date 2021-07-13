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
