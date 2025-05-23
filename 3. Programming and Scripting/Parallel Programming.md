 Purpose & Outcomes
Understand concurrency, parallelism, and distributed computing

Apply these concepts in Python and Apache Spark

Assess performance implications and select the right approach

🧾 Key Definitions
Term	Definition
Concurrency	Tasks making progress at the same time (even on a single core)
Parallelism	Tasks executed simultaneously, often across multiple cores or machines
Multiprocessing	Uses multiple processes; good for CPU-bound tasks
Multithreading	Uses multiple threads in the same process; good for I/O-bound tasks
Distributed computing	Executes tasks across multiple physical machines

🔄 Concurrency vs Parallelism
Concurrency: Multiple tasks run independently, but not always at the same time.

Parallelism: Tasks run at the same time to complete faster.

🧠 Concurrency ≠ Parallelism

🖥️ Multiprocessing vs Multithreading
Aspect	Multiprocessing	Multithreading
Use case	CPU-bound	I/O-bound
Memory	Separate	Shared
Speed	Higher overhead	Faster creation
Achieves	True parallelism	Concurrency

🐍 Parallel Programming in Python
Threading module uses OS-level threads but limited by Global Interpreter Lock (GIL).

Multiprocessing module allows real parallelism (not limited by GIL).

python
Copy
Edit
from multiprocessing import Process
def task(): ...
p = Process(target=task)
p.start()
🧩 Fork-Join Model
Used for divide-and-conquer algorithms.

Fork: Parent creates a child process/thread.

Join: Parent waits for child to finish before continuing.

🧠 Task vs Data Parallelism
Type	Description
Task Parallelism	Different tasks on the same/different data
Data Parallelism	Same operation on different chunks of data

Example: Spark uses data parallelism extensively.

⚡ Apache Spark
💡 Key Points:
Distributed cluster computing framework

APIs in Python, Scala, Java, R

Core abstraction: RDDs (Resilient Distributed Datasets)

🔁 RDD Operations
Transformations: map(), filter(), flatMap()

Actions: collect(), count(), reduce(), saveAsTextFile()

Key-Value: reduceByKey(), groupByKey(), sortByKey()

python
Copy
Edit
lines = sc.textFile("file.txt")
counts = lines.flatMap(lambda l: l.split(" ")) \
              .map(lambda word: (word, 1)) \
              .reduceByKey(lambda x, y: x + y)
🧪 Practical Application
Use Azure Databricks to run Spark jobs

Notebook tasks include:

Creating RDDs

Performing transformations and actions

Parsing CSV and performing basic analytics

🔗 Tutorial Briefing PDF
[L5DE M3T7 V1.pdf](https://github.com/user-attachments/files/20408875/L5DE.M3T7.V1.pdf)
