Open_Data
=========

Python interactions with Open Data repositories

### chigago_datasets.py

Socrata Open Data datasets can be selected, cached locally, and printed out.
Datasets published by City of Chicago @ http://data.cityofchicago.org
 
Read in description data on all datasets (currently 294)

```
loop: Allow the user to select one
    Write a json version of the dataset to a local file
    From the dataset metadata, create a namedtuple for the column names
    Dump all dataset rows as namedtuples
    Go to loop
    
```

Notes:
    Not all datasets have json representations --> script fails
    Avoid monstrous datasets such as All Crimes from 2001 to Present (5m records)
