# Working with data bigger than RAM

## Abstract
I will compile here all the interesting solutions/tools to work with data bigger than RAM. This won't be necessary in general, as cloud servers (AWS EC2) are cheap and huge, and in 99% of the projects we can perfectly work with summarized data. But it is sometimes useful to be able to handle large amounts of data to perform simple queries for posterior analysis,or to create that summaries without the need of more complex or expensive tools.

## MonetDBLite
Very fast [R package](https://github.com/hannesmuehleisen/MonetDBLite-R) (based on the [MonetDB](https://www.monetdb.org/Home) data base) to perform SQL queries over files in your HDD. The data needs to be initially transformed to a specific format (the package has tools to perform this transformation). After that transformation, SQL queries can be performed over the data set in a VERY FAST way (almost as fast as data.table operations!). *dplyr* can also be used through the *dbplyr* package. A use example can be found [here]().

## MLDB
https://github.com/mldbai/mldb

## dbplot
TODO: https://db.rstudio.com/dbplot

