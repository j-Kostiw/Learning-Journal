 Why Spark?
Fast: In-memory processing

Scalable: Works across many machines

Easy to Use: High-level APIs in Python, Scala, Java, R

Real-world case: Alibaba used Spark to process huge volumes of data efficiently.

🔧 RDD (Resilient Distributed Dataset) Basics
Create RDDs
python
Copy
Edit
sc.parallelize([1, 2, 3])
sc.textFile("file.txt")
Transformations
map(): Apply a function to each element

filter(): Keep elements that match a condition

flatMap(): Flatten lists of results

Actions
collect(): Bring all data to the driver

take(n): Return first n elements

count(): Count items

reduce(): Combine with a function (e.g., sum)

saveAsTextFile(): Save results

Key-Value RDDs
python
Copy
Edit
rdd = sc.parallelize([("cat", 1), ("cat", 2)])
rdd.reduceByKey(lambda x, y: x + y)
🧱 Pair RDD Operations
Function	Description
countByKey()	Counts how many times each key appears
groupByKey()	Groups values by key
sortByKey()	Sorts by key
join()	Combines two RDDs by key

Example: Word Count
python
Copy
Edit
lines = sc.textFile("hamlet.txt")
counts = lines.flatMap(lambda l: l.split(" ")) \
              .map(lambda w: (w, 1)) \
              .reduceByKey(lambda x, y: x + y)
⚡ Pipelining
Spark optimizes chained transformations to avoid unnecessary intermediate storage.

🔗 Joins & Practical Example
Join web logs to knowledge base articles:

Map logs: (docid, userid)

Map index: (docid, title)

Join on docid

Output: (userid, title)

📡 Broadcast Variables
Avoid repetitive network transfers:

python
Copy
Edit
lookup = sc.broadcast(my_lookup_data)
rdd.map(lambda x: do_something_with(lookup.value))
Useful for reference data (e.g., postcode directory)

🧾 SparkSQL
Use SQL-like queries on distributed data

Uses DataFrames, not traditional databases

Can be faster to develop with and more readable

Pros vs MySQL:
Spark can use all CPU cores in a cluster

No need to import data into a database

Spark scales better for big data

SQL Query Example
python
Copy
Edit
df.select("country", "city").show()
spark.sql("SELECT country, city FROM ZIPCODES").show()
🧪 DataFrames vs Pandas
Feature	Spark DataFrame	Pandas DataFrame
Mutability	Immutable	Mutable
Execution	Distributed	Local
Use case	Big data, clusters	Small-to-medium data

🏗️ Creating DataFrames
From CSV:

python
Copy
Edit
from pyspark.sql import SparkSession

spark = SparkSession.builder.appName("MyApp").getOrCreate()
df = spark.read.csv("data.csv", header=True)
🔄 SQLContext vs SparkSession
Feature	SQLContext	SparkSession
Introduced	Spark v1.x	Spark v2.x onwards
Status	Deprecated	Preferred

SparkSession is a unified entry point for using SQL, RDDs, Hive, etc.

🔍 Inspecting & Querying DataFrames
Function	Purpose
.show()	View records
.where()	Filter rows
.orderBy()	Sort
.groupBy().count()	Aggregation

🔗 Join Types in PySpark
python
Copy
Edit
df1.join(df2, on="id", how="inner")
Type	Description
inner	Matching rows only
left	All from left, match from right
right	All from right, match from left
outer	All from both sides

🧠 Knowledge Check Reminders
sc.parallelize([1,2,3]) creates RDD from a list ✅

Spark uses pipelining to avoid storing data between steps ✅

Pair RDDs support advanced operations like join, groupByKey ✅

🧪 Practical Exercise
Join logs with knowledge base articles using RDDs or DataFrames. Explore the walkthrough here:
🔗 Code Walkthrough

✅ Takeaways 
RDDs: Foundation for distributed processing

Transformations: Build up logic without execution

Actions: Trigger computation

DataFrames & SparkSQL: Powerful, user-friendly data querying

Broadcast variables: Efficient reuse of reference data

Pipelining: Key Spark performance booster
[L5DE M3T8 V1.pdf](https://github.com/user-attachments/files/20408962/L5DE.M3T8.V1.pdf)

