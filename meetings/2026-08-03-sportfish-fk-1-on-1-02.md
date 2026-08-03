Brittany Troast & Tylar Murray

* Flow chart was helpful for understanding occurrence core vs event core
* Sportfish data naturally maps to event core
* modify instructions : can re-use unique identifer instead of create new?
* set up to use Location table
  * we are reformating to use Event table only
* verbatimLat & lon are identical
  * can leave off optional verbatim columns
* count may be complicated because tot_count has count per trawl
  * for sportfish we can use 1 for all rows
  * some stations have additional collected occurrences in another file
    * we will focus on the sportfish first then add on the others
  * parentEventID does not apply here
  * keyfield has date+time+station
* dwc quick reference can be confusing for OBIS usage
  * example: doesn't include scientificName on the occurrence
* 
