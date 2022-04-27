# Simple Data Definition
The goal for this project is to create a data/object storing file format with very minimal boiler plate around the actual data. SDD stores data similarly to YAML, but with even less syntax.
```
EXAMPLE SDD FILE
---------------------------
dates:                                                          // lines that end with ':' start an object declaration
 y2k:                                                           // spaces (one space per level) are used to assign heirarchy
  month = 1                                                     // data values are assigned using the equals sign
  day = 1
  year = 2000
 independenceDay:
  month = 7
  day = 4
  year = 1776
  description = "The day America got the dub"                   // strings are surrounded by double quotes
  securedRights = ["Life", "Liberty", "Pursuit of Hapiness"]    // lists are surrounded by square brackets, with values 
                                                                // separated by commas. All elements in a list should be the same type
```
