# bivariate-maps-qgis-recreate-sf
The idea of this work was based on the excellent work of Timo Grossenbacher, https://timogrossenbacher.ch/2019/04/bivariate-maps-with-ggplot2-and-sf/ which has initially created these maps with R. I played and tested a lot of time with these R code and was amazed about it. 

Some weeks ago I showed these maps to a friend of me which work in the GIS area. We played in the past a lot with gis systems, he with his ESRI Arcgis and I with QGIS. He had the opinion that this would be easy possible with a GIS system as well. I was in the following strong motivated to figure out if this is possible. Yes it is and I am very lucky that it is possible as well!

i don't like to repeat all about licences of the date. For this issue I point to the documentation of Timo Grossenbacher for the inital R version which you can find, https://timogrossenbacher.ch/2019/04/bivariate-maps-with-ggplot2-and-sf/.

QGIS version used and extensions
- QGIS LTS Version 3.4
- Plugin "Mask"

How to:
1. Start a new project in QGIS
2. Drag and drop the Shapefiles (*.shp) into the QGIS
3. In our case we use the file "data.csv" for the data. When you inport a ".csv-File into QGIS, QGIS has problems to define the right type for the data. To define the types you can create a file with the extension *.csvt which describes the types of the date, e.E. "String","Integer","Real","Real" in one single line in a file data.csvt. if this file is available then you can just drag and drop the data.csv file and the attributes have the desired types. 

GDAL.org describibes how you can define to types for the data, https://gdal.org/drivers/vector/csv.html
Limited type recognition can be done for Integer, Real, String, Date (YYYY-MM-DD), Time (HH:MM:SS+nn), DateTime (YYYY-MM-DD HH:MM:SS+nn) columns through a descriptive file with the same name as the CSV file, but a .csvt extension. In a single line the types for each column have to be listed with double quotes and be comma separated (e.g., “Integer”,”String”). It is also possible to specify explicitly the width and precision of each column, e.g. “Integer(5)”,”Real(10.7)”,”String(15)”. The driver will then use these types as specified for the csv columns.

has a very nice feature to create 

Peter Berger

