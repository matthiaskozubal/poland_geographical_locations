Returns geographical coordinates of a given voivodeship, district of Warsaw, or city in Poland.
==============

Locations are obtained from wikidata.org using a SPARQL query language.
* Use: ```return_coordinates(place)``` where ```place``` is either voivodeship, district of Warsaw, or city in Poland, written in polish. 
* Output: [latitude, longitude].


Examples:
--------
1. 
    * ```In:   return_coordinates('województwo podlaskie')```
    * ```Out: [53.267219444444, 22.931938888889]```
   
2.
    * ```In:   return_coordinates('podlaskie')```
    * ```Out: [53.267219444444, 22.931938888889]```
3.
    * ```In:   return_coordinates('PODLASKIE')```
    * ```Out: [53.267219444444, 22.931938888889]```
4.
    * ```In:   return_coordinates('Ursus')```
    * ```Out: [52.19517, 20.88419]```
5.
    * ```In:  return_coordinates('Dobra')```
    * ```Out: [53.583333333333, 15.308333333333]```
6.
    * ```In:   return_coordinates('żyrardów')```
    * ```Out: [52.05, 20.433333333333]```    
    
    
Alternatively, following functions can also be used:
* ```get_voivodeships()``` - returns a dataframe with all voivodeships in Poland,
* ```get_warsaw_districts()``` - returns a dataframe with all districts of Warsaw (Poland),
* ```get_cities()``` - returns a dataframe with all cities in Poland.
