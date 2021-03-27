DropWizard and MongoDB example
==============================

Import provided xml with coffee shops in MongoDB
------------------------------------------------
`gradle populateMongo`

Run the server
--------------
`gradle run`

Test the app
------------
[http://localhost:8080/coffee.html](http://localhost:8080/coffee.html)


----------------------------

How to obtain OpenStreetMap testing data
----------------------------------------

- search the POI using [openstreetmap](https://www.openstreetmap.org)
- use [overpass-turbo](https://overpass-turbo.eu/) to extract information from the OSM database

```
/*
This is an example Overpass query.
Try it out by pressing the Run button above!
You can find more examples with the Load tool.
*/
area[name="Municipiul București"];
nwr[amenity=cafe](area);
out center;
```
- use Export capabilities to save data


More info:
----------

- [https://wiki.openstreetmap.org/wiki/Overpass_turbo/Wizard](https://wiki.openstreetmap.org/wiki/Overpass_turbo/Wizard)
- [https://wiki.openstreetmap.org/wiki/Key:amenity](https://wiki.openstreetmap.org/wiki/Key:amenity)
- [https://dev.overpass-api.de/overpass-doc/en/criteria/per_tag.html#local](https://dev.overpass-api.de/overpass-doc/en/criteria/per_tag.html#local)