# YSI Batch Prediction
The objective of this project is to use SMILES/Name/CAS to fetch measured YSI and predicted YSI of orangic compounds via **an API of YSI Estimator (https://ysi.ml.nrel.gov/docs)**. Two CAS/name-to-SMILES converters are available, one is **cactus_conversions.py** made by me based on **cactus API (https://cactus.nci.nih.gov/chemical/structure)** and the other is **chemical_conversions.py** made by Dr. Peter St. John (https://github.com/pstjohn) based on **PubChem API (https://pubchempy.readthedocs.io/en/latest/api.html)**. Users should refer to these links in case of any change of the API URLs.

Users can choose one of the three chemical identifiers (SMILES/Name/CAS) as the input by adding it to the corresponding column in compounds.xlsx. The identifier will eventually be converted to SMILES. The output is another excel called YSI results.xlsx.

### Objective
fetch measured and predicted YSIs with identifiers as inputs

### Method
identifiers→ SMILES (via PubChem) → API (Application programming interface) → YSIs;

### Input
an excel sheet with SMILES or Name or CAS; 
### Output
another excel sheet with measured and predicted YSI;

### Pros
only need one identifier, fast (100 compounds/mins), filter out outliers;
### Cons
bizarre names and CAS cannot transfer to SMILES.
