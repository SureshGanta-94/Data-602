# NYPD Arrest Data

### About the Dataset:
- This is a breakdown of every arrest effected in NYC by the NYPD during the current year.
- This data is manually extracted every quarter and reviewed by the Office of Management Analysis and Planning.
- Each record represents an arrest effected in NYC by the NYPD and includes information about the type of crime, the location and time of enforcement.
- In addition, information related to suspect demographics is also included.
- This data can be used by the public to explore the nature of police enforcement activity.

### Dataset Description
The dataset retrieved from 'NYC OpenData'. This has information about number of arrests made in the current fiscal year(2021). This dataset is update frequncy is every quarter.

#### Dataset Source: https://data.cityofnewyork.us/Public-Safety/NYPD-Arrest-Data-Year-to-Date-/uip8-fykc/data 

### Columns in the Dataset

- ARREST_KEY: Randomly generated persistent ID for each arrest
- ARREST_DATE: Exact date of arrest for the reported event
- PD_CD: Three digit internal classification code (more granular than Key Code)
- PD_DESC: Description of internal classification corresponding with PD code (more granular than Offense Description)
- KY_CD: Three digit internal classification code (more general category than PD code)
- OFNS_DESC: Description of internal classification corresponding with KY code (more general category than PD description)
- LAW_CODE: Law code charges corresponding to the NYS Penal Law, VTL and other various local laws
- LAW_CAT_CD: Level of offense: felony, misdemeanor, violation
- ARREST_BORO<: Borough of arrest. B(Bronx), S(Staten Island), K(Brooklyn), M(Manhattan), Q(Queens)
- ARREST_PRECINCT: Precinct where the arrest occurred
- JURISDICTION_CODE: Jurisdiction responsible for arrest. Jurisdiction codes 0(Patrol), 1(Transit) and 2(Housing) represent NYPD whilst codes 3 and more represent non NYPD jurisdictions
- AGE_GROUP: Perpetrator’s age within a category
- PERP_SEX: Perpetrator’s sex description
- PERP_RACE: Perpetrator’s race description
- X_COORD_CD: Midblock X-coordinate for New York State Plane Coordinate System, Long Island Zone, NAD 83, units feet (FIPS 3104)
- Y_COORD_CD: Midblock Y-coordinate for New York State Plane Coordinate System, Long Island Zone, NAD 83, units feet (FIPS 3104)
- Latitude: Latitude coordinate for Global Coordinate System, WGS 1984, decimal degrees (EPSG 4326)
- Longitude: Longitude coordinate for Global Coordinate System, WGS 1984, decimal degrees (EPSG 4326)
- New Georeferenced Column: pinpoints geocode of the location

### Operations Performed
- Exploring dataset
- Data Inconsistencies
- Data Cleaning
- Sanity checks to identify duplicates
- Distribution plots

### EDA Outcomes and Important Observations
- The top three offenses are 'ASSAULT 3 & RELATED OFFENSES,' 'FELONY ASSAULT,' and 'PETIT LARCENY.'
- The highest level of offenses are'misdemeanor' and 'felony.'
- Males are more likely to commit crimes than females.
- The 'black' and 'white hispanic' races are more likely to commit crimes according to data.
- 'April' is the month with the fewest arrests, while 'october' has the most.
- Up to the 21st of the month, the number of arrests is rather equally distributed.
- There is a significant decline in arrests from the 21st of the month to the end of the month.
- People of the 'Black' race are more likely to be detained in both genders.
- The age group '25-44' is involved in criminal activity in both male and female genders.
- 'Black' race individuals commit more crimes than those of other races at every age.
