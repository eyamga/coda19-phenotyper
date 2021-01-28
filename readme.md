# CODA19 phenotyper project
 
## Files organization of the project


### Custom SQL scripts
- files located in py_eyamga/sql
SQL lite scripts extracting all meaningful categories from the 

### Python scripts
- dataparser
* queries all SQL file appropriately and exports them as CSV in local directory
- RxCUI class
* maps drug names to MESH drug class categories

### R script

In order :
### 1. Dataparser
similar to the python script
runs sql scripts and exports appropriate csv files in the local /csv dir

### 2. EDA
- load datawrangled csv files
- transforms the data from narrow to wide 
- exports a final csv file that is ready for analysis
Other features
- MICE imputation
- Exports EDA pdfs
- 3 differents format : data at 24h, 48h and 72h

### 3. Feature engineering
- Runs PCA/MCA/FAMD  

### 4. Cluster Analysis
- As described

### 5. Markdown folder
- Runs entire project and modified script and outputs sharable html fule
