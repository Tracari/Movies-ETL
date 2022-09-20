# Movies-ETL
## Overview: 
This project is an introduction to a core concept of data engineering, the data pipeline process: ETL
- Extract 
- Transform
- Load. 
In this skill a clean dataset needs to prepared for a hackathon for an online streaming platform's contest. The scraped raw data will be extracted from 3 sources, transformed into 1 set, and loaded in to SQL database. The database can then be provided to the “hackers” to develop an algorithm to predict popularity probability among a dataset.

### Data Environment:
Python
Pandas
PostgreSQL
JSON
NumPy
SqlAlchemy

## Results: 1-2 major points
### Extract: 

To create the movies dataset with ratings information, a function was defined to take in 3 arguments that read in the extracted .csv data from 2 websites and JSON data from 1 website into respective Pandas DataFrames. 

<img width="775" alt="Screen Shot 2022-09-19 at 10 00 31 PM" src="https://user-images.githubusercontent.com/105556091/191157886-9ed64c55-9997-43c6-98fa-dcdf6be72671.png">



### Transform:
Before the datasets can be joined and loaded into PostgreSQL for the hackers access, the individual datasets need to be inspected to ensure the data is valuable, formatting is consistent, and the provided information is prioritized.
- Transforming data is achieved through a constant iteration process to identify and classify: 
   - necessary data vs nonessential data and 
   - properly formatted data vs data the needs corrective formatting.
   - frequency of null values

ETL_CLEAN_WIKI_MOVIES.IPYNB
<img width="771" alt="Screen Shot 2022-09-19 at 10 19 18 PM" src="https://user-images.githubusercontent.com/105556091/191160161-f2308f6c-f4d4-4f49-9456-e0b4d70b2cf8.png">

<img width="766" alt="Screen Shot 2022-09-19 at 10 19 33 PM" src="https://user-images.githubusercontent.com/105556091/191160417-9fd41974-dcd0-4f18-bc57-87c225ad1656.png">

<img width="603" alt="Screen Shot 2022-09-19 at 10 20 13 PM" src="https://user-images.githubusercontent.com/105556091/191160445-0f29653c-d8e9-437d-b8b8-4e5657c7f727.png">


### Load: 

Once the individual datasets have been cleaned and transformed, Using Python the movies datasets can be merged into one Pandas DataFrame and with the use of SqlAlchemy can Loaded into PostgreSQL for publishing and public access

<img width="853" alt="Screen Shot 2022-09-19 at 10 05 31 PM" src="https://user-images.githubusercontent.com/105556091/191158427-805720e9-61c5-449a-a1de-cfe52c690d05.png">

<img width="745" alt="Screen Shot 2022-09-19 at 10 07 30 PM" src="https://user-images.githubusercontent.com/105556091/191158626-da29afe3-7c25-4188-bf32-d42fc8aa9249.png">

<img width="757" alt="Screen Shot 2022-09-19 at 10 03 34 PM" src="https://user-images.githubusercontent.com/105556091/191158161-ed794152-b256-4185-831d-0d6d6a15e3f2.png">



#### Summary: 
The ETL pipeline, a core concept of data engineering, moves information from source systems to its destination. The process reconstructs and cleans raw data in preparation for analytical and operational uses, Like a hack-a-thon!
In this exercise, a valuable dataset was engineered by extracting raw data from several systems then transforming the information through an iterative process of revealing and detailing appropriate and effective data. The dataset was then republished and stored in a public database purposed for community access. Extract. Transform. Load.

