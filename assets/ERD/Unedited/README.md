All files for company and year were in the following table format:

| Column Name                 | Type        | Description |
|-----------------------------|------------| --------------|
| net_manager             | text           | Code of the regional network manager |
| purchase_area           | text           | Code of the area where the energy is purchased |
| street                  | text            | Name of the street |
| zipcode_from / zipcode_to | text       | Range of zip codes covered (4 numbers and 2 letters) |
| city                    | text            |Name of the city |
| num_connections         | whole number            |Number of connections in the zip code range |
| delivery_perc           | decimal number         |Percentage of net consumption of electricity or gas. Lower values indicate more energy returned to the grid (e.g., from solar panels) |
| perc_of_active_connections | decimal number         |Percentage of active connections in the zip code range |
| type_of_connection      | text             |Principal type of connection in the zip code range. For electricity: `# fuses X # ampère`. For gas: `G4, G6, G10, G16, G25` |
| type_conn_perc          | decimal number            |Percentage of presence of the principal type of connection in the zip code range |
| annual_consume          | whole number            |Annual consumption (`kWh` for electricity, `m³` for gas) |
| annual_consume_lowtarif_perc | decimal number       |Percentage of consumption during low tariff hours (10 p.m. - 7 a.m. and weekends) |
| smartmeter_perc        | decimal number              |Percentage of smart meters in the zip code range |
