# ysi_batch_prediction
The objective of this project is to use SMILES/Name/CAS to fetch measured YSI and predicted YSI via an API of YSI Estimator (https://ysi.ml.nrel.gov/) and a SMILES/Name/CAS converter (chemical_conversions.py) made by Dr. Peter St. John at NREL (https://github.com/pstjohn).
Users can choose one of the three chemical identifiers (SMILES/Name/CAS) as the input by adding it to the corresponding column in compounds.xlsx. The identifier will eventually be converted to SMILES. The output is another excel called YSI results.xlsx.
