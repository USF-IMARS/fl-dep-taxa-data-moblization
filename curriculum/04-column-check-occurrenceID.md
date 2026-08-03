`occurrenceID` must be unique.
We recommend creating a "natural key" occurrence id to help heuristically identify the record.
The format of the occurrenceID might be something like `exampleDataset-{eventDate}-{sequential number}`.
Using this example format you might have the following rows:

occurrenceID                  | scientificName | basisOfRecord    | occurrenceStatus | decimalLatitude | decimalLongitude | eventDate
------------------------------|----------------|------------------|------------------|-----------------|------------------|-----------
exampleDataset-2020-02-02-001 | B. musculus    | HumanObservation | present          | 30.170303300254 | -67.457828248219 | 2020-02-02
exampleDataset-2020-02-02-002 | B. musculus    | HumanObservation | present          | 33.289573300123 | -66.247199027405 | 2021-02-02
exampleDataset-1999-10-11-001 | B. musculus    | HumanObservation | present          | 36.136760302944 | -60.821994505693 | 1999-10-11

