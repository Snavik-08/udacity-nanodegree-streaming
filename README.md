
## Data Streaming Nanodegree
### SF Crime Statistics with Spark Streaming

** 1. How did changing values on the SparkSession property parameters affect the throughput and latency of the data?

It will either decrease or increase the processed rows per second

** 2. What were the 2-3 most efficient SparkSession property key/value pairs? Through testing multiple variations on values, how can you tell these were the most optimal? The goal on here is to maximize the processedRowsPerSecond in long run. So, I choose:


Comparing the spark.sql.shuffle.partitions with 2 compared to 20, it was clear that the processedRowsPerSecond was  better for 2 partitions

Comparing spark.default.parallelism of 100 with 10000, it seems that e processedRowsPerSecond were better for the value 100 
