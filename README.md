# WordCountMapReduceJava
Word Count Example using Map Reduce and Java 

First Install Hadoop. If you haven't check CodeWithArjun For installation. 

Then, create /test/data.text file with some text. For Example 

HDFS is a storage unit of Hadoop
MapReduce is a processing tool of Hadoop


Then Write Java program from this repository. 

Then create Jar using command 
mvn clean install

Then use this command for the jar file created in your location: 

hadoop jar /Users/arjuncodes/Documents/MapReduceExample/target/MapReduceExample-1.0-SNAPSHOT.jar demo.WC_Runner /test/data.txt /r_output

Then will create output inside r_output file. The run this command to find the number of words. 

hadoop fs -cat /r_output/part-00000

The output would look like this : 

HDFS	1
Hadoop	2
MapReduce	1
a	2
is	2
of	2
processing	1
storage	1
tool	1
unit	1
