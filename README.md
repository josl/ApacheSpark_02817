# WEEK 08: Apache Spark

Exercise 8 of 02807 Computational Tools for Big Data at DTU

## Content:

This week will be an introduction to Apache Spark and the Python library pyspark.

Watch my lecture here: https://www.youtube.com/watch?v=KCoLQ7BZosA

## Learning objectives:

After this week, you are supposed to know:

- What Apache Spark is
- How to write a Spark program
- How to implement and run a pyspark script locally

## Resources:

Spark programming guide: http://spark.apache.org/docs/latest/programming-guide.html

Documentation for pyspark: http://spark.apache.org/docs/latest/api/python/


## Exercises:

### Exercise 7.0: (don’t include in assignment):

You should install Spark and pyspark. Follow the following steps:

- Download and install Vagrant from here: https://www.vagrantup.com/
- Download the following Vagrant-file: https://www.dropbox.com/s/q8yj7qd5hifkhfj/Vagrantfile?dl=0
- Go to the folder of the Vagrantfile
- Run “vagrant up” to boot the virtual machine (this will probably take some time)
- Access the Jupyter web UI for running IPython notebooks by navigating your web browser to “http://localhost:8001” (or “http://127.0.0.1:8001/“)
- Download the following iPython notebook with some examples: https://www.dropbox.com/s/hbz98qnhbspc1mf/Spark%20test.ipynb?dl=0
- Upload the notebook using the Upload-button in the ipython notebook in the browser. Note: The upload button in iPython is also a good way to copy the data files to the Vagrant virtual machine.
- Open the notebook in the browser and run the code!


### Exercise 7.1:

Write a Spark job to count the occurrences of each word in a text file. Document that it works with a small example.

### Exercise 7.2:

Write a Spark job that determines if a graph has an Euler tour (all vertices have even degree) where you can assume that the graph you get is connected. This file https://www.dropbox.com/s/usdi0wpsqm3jb7f/eulerGraphs.txt?dl=0 has 5 graphs – for each graph, the first line tells the number of nodes N and the number of edges E. The next E lines tells which two nodes are connected by an edge. Two nodes can be connected by multiple edges.

It is fine if you split the file into 5 different files. You do not need to keep the node and edge counts in the top of the file.

Document that it works using a small example.
### Exercise 7.3:

You are given a couple of hours of raw WiFi data from my phone: https://www.dropbox.com/s/964gq5o5bkzg7q3/wifi.data?dl=0

Compute the following things using Spark:

1. What are the 10 networks I observed the most, and how many times were they observed? Note: the bssid is unique for every network, the name (ssid) of the network is not necessarily unique.
2. What are the 10 most common wifi names? (ssid)
3. What are the 10 longest wifi names? (again, ssid)

## First steps

- make vagrant # Boots Vagrant based on the Vagrantfile (very slow...)
- Open http://127.0.0.1:8001/tree#notebooks and start a Terminal
- run: apt-get update ; apt-get install git-all
- git clone https://github.com/josl/ApacheSpark_02817

## General Comands

It's recommended to create a virtual environment (conda env preffered)

General commands:
* "make list" to list all available targets;
* "make setup" to install all dependencies (do not forget to create a virtualenv first);
* "make test" to test your application (tests in the tests/ directory);
* "make tox" to run tests against all supported python versions.


## License
MIT © [Jose Luis Bellod Cisneros](http://josl.github.i- o)
