In this meeting we will discuss how to plan your data schema.


-------------------------------------------------------------


Darwin Core Archives are made up entirely of 
* tables
* relationships between tables

This is called a relational database schema. 


-------------------------------------------------------------


In Darwin Core a table is a collection of rows and a header row at the top.

An essential table is the **occurrence** table.

The occurrence table is the table of what was seen where+when.
Here is a partial Darwin Core Occurrence Table:

occurrenceID | scientificName | basisOfRecord    | occurrenceStatus | decimalLatitude | decimalLongitude | eventDate
-------------|----------------|------------------|------------------|-----------------|------------------|-----------
my-occur-123 | B. musculus    | HumanObservation | present          | 30.170303300254 | -67.457828248219 | 2020-02-02
my-occur-124 | B. musculus    | HumanObservation | present          | 33.289573300123 | -66.247199027405 | 2021-02-02
my-occur-125 | B. musculus    | HumanObservation | present          | 36.136760302944 | -60.821994505693 | 2023-02-02


-------------------------------------------------------------


To put your data into OBIS, you must construct an occurrence table.

Some of your data may not fit into the Occurrence table. 
For this data you can use other tables, like the Event and MeasurementOrFact tables.
First we will create the occurrence table, then we can work on other tables.


-------------------------------------------------------------


Your task is to create a "mapping" of columns to explain where the required Darwin Core Occurrence column data is in your existing dataset.
Below is an example mapping:

DwC Column Name    | Where it is in your data.
-------------------|--------------------------------
* occurrenceID     | New column will be created with format `exampleDataset-{eventDate}-{sequential number}`.
* occurrenceStatus | `present` for all records.
* basisOfRecord    | `HumanObservation` for all records.
* scientificName   | Column "species name" from observations.xslx.
* scientificNameID | NOTE: leave this blank for now.
* eventDate        | Column "date" from observations.xlsx.
* decimalLatitude  | Column "lat" from observations.xlsx.
* decimalLongitude | Column "lon" from observations.xlsx.


-------------------------------------------------------------


Homework: map your columns to occurrence table columns.

The Minimum Occurrence columns are:

DwC Column Name    | Where it is in your data.
-------------------|--------------------------------
* occurrenceID     | 
* occurrenceStatus | 
* basisOfRecord    | `.
* scientificName   | .
* scientificNameID | .
* eventDate        | .
* decimalLatitude  | .
* decimalLongitude | .


-------------------------------------------------------------


Additional Guidance:
* [DwC Manual : How to Format the Occurrence Table](https://manual.obis.org/format_occurrence.html)

Reference Materials:
* [DwC schema diagram](https://ipt.gbif.org/manual/en/ipt/latest/dwca-guide)
* [DwC Quick reference](https://dwc.tdwg.org/terms/#measurementorfact)


