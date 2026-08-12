The `scientificNameID` field contains a taxonomic identifier (lsid) from World Register of Marine Species (WoRMS).
The values in `scientificName` can be compared with the WoRMS database to automatically identify each lsid, but some values may need manual alignment.

* install RStudio
* install packages ([obistools](https://github.com/iobis/obistools))
* load your occurrence dataframe, match taxa, and update the column.

```R
# Read in occurrence table
occur <- read.csv("occurence_table.csv")

# Conduct taxon matching on only the unique instances of each taxa's name
worms <- obistools::match_taxa(unique(occur$scientificName), ask=T)

# Merge the matched names back with occurrence data
occur_match <- merge(occur, worms, by="scientificName", all= T)
```

* [OBIS manual on taxa matching](https://manual.obis.org/name_matching.html).
