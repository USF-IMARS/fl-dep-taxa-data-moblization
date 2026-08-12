Create a script to complete [QC checks with obistools R package):

```R
occurrences <- read.csv("occurence.csv")
obistools::check_fields(occurrences)

obistools::plot_map(occurrences)

obistools::check_onland(occurrences)

obistools::check_depth(occurrences)

obistools::check_eventdate(occurrences)
```

* [OBIS Manual on QC checks with obistools](https://manual.obis.org/data_qc.html#conducting-qc-with-obistools)


## Event Core
* [additional check if using event core](https://github.com/iobis/obistools#check-eventid-in-an-extension)
