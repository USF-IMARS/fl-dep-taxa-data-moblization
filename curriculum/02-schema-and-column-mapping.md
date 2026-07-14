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

occurrenceID | scientificName | basisOfRecord | occurrenceStatus | decimalLatitude | decimalLongitude | eventDate
-------------|----------------|---------------|------------------|-----------------|------------------|----------


-------------------------------------------------------------




-------------------------------------------------------------

To put your data into OBIS, you must construct an occurrence table.

Some of your data may not fit into the Occurrence table. 
For this data you can use other tables, like the Event and MeasurementOrFact tables.

-------------------------------------------------------------

Homework map columns to occurrence table.


Minimum Occurrence columns:

TODO

-------------------------------------------------------------

Mapping example:

TODO


Links

* [schema diagram](https://ipt.gbif.org/manual/en/ipt/latest/dwca-guide)
  * start with occurrence, Event, & MoF
* [DwC Quick reference](https://dwc.tdwg.org/terms/#measurementorfact)

-------------------------------------------------------------
