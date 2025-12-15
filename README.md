this is a simple implimentaion of a elt pipeline for nyc taxi data. 

the vision right now has it as such:

1. i will manually load a .parquet file to a bucket in gcs
2. i will have a dagster sensor that will poll my buckets ever minute or so to see if it can detect a new upload
3. when a new file is detected, that will trigger a series of events to load the .parquet into big query
4. then, a few transformations will occur leading to analytics ready data



i will have a dagster instance running on my server that will be orchestrating this work flow



#### future plans

- ideally i would have all of this in a serverless cloud native architecture but this is project is just to practive working with dagster and big query
- additionally, i will use this project to work on my infrastrucurre skills and understanding cloud architecture