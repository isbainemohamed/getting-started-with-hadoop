# getting-started-with-hadoop
This repository contains necessary materials to set up a single node hadoop cluster.
## 1. Objectives

- Run a single-node Hadoop instance
- Perform a word count using Hadoop Map Reduce.

## 2. Set up Single-Node Hadoop:

The steps outlined in the next sections use the single-node Hadoop Version 3.2.3. Hadoop is most useful when deployed in a fully distributed mode on a large cluster of networked servers sharing a large volume of data. However, for basic understanding, we will configure Hadoop on a single node.

In this guide, we will run the WordCount example with an input text and see how the content of the input file is processed by WordCount.

* 1st Step:

Download hadoop-3.2.3.tar.gz to your theia environment by running the following command.

```bash
curl https://dlcdn.apache.org/hadoop/common/hadoop-3.2.3/hadoop-3.2.3.tar.gz --output hadoop-3.2.3.tar.gz
```
![download](https://github.com/isbainemohamed/getting-started-with-hadoop/blob/9c92d432ad7627750c771808fb6ac9cc4dc13a65/screens/screen1.png)

* 2nd step :

Extract the tar file in the currently directory.

```bash
tar -xvf hadoop-3.2.3.tar.gz
```

![download](https://github.com/isbainemohamed/getting-started-with-hadoop/blob/9c92d432ad7627750c771808fb6ac9cc4dc13a65/screens/screen2.png)

3rd Step: 

Navigate to the hadoop-3.2.3 directory.

```bash
cd hadoop-3.2.3
```

![download](https://github.com/isbainemohamed/getting-started-with-hadoop/blob/9c92d432ad7627750c771808fb6ac9cc4dc13a65/screens/screen3.png)

4th Step: 

Check the hadoop command to see if it is setup. This will display the usage documentation for the hadoop script.

```bash
bin/hadoop
```

![download](https://github.com/isbainemohamed/getting-started-with-hadoop/blob/9c92d432ad7627750c771808fb6ac9cc4dc13a65/screens/screen4.png)

5th Step:

Download data.txt to your current directory and explore the data in our file

```bash
curl https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-BD0225EN-SkillsNetwork/labs/data/data.txt --output data.txt
cat data.txt
```

![download](https://github.com/isbainemohamed/getting-started-with-hadoop/blob/9c92d432ad7627750c771808fb6ac9cc4dc13a65/screens/screen5.png)

![download](https://github.com/isbainemohamed/getting-started-with-hadoop/blob/9c92d432ad7627750c771808fb6ac9cc4dc13a65/screens/screen6.png)

6th Step:

Run the Map reduce application for wordcount on data.txt and store the output in /user/root/output

```bash
bin/hadoop jar share/hadoop/mapreduce/hadoop-mapreduce-examples-3.2.3.jar wordcount data.txt output
```

![download](https://github.com/isbainemohamed/getting-started-with-hadoop/blob/9c92d432ad7627750c771808fb6ac9cc4dc13a65/screens/screen7.png) 

7th Step:

Once the word count runs successfully, we can run the following command to see the output file it has generated.

```bash
ls output
```

![download](https://github.com/isbainemohamed/getting-started-with-hadoop/blob/9c92d432ad7627750c771808fb6ac9cc4dc13a65/screens/screen8.png)

part-r-00000 with _SUCCESS is indicating that the wordcount has been done.


show the output of our wordcount

```bash
cat output/part-r-00000
```

![download](https://github.com/isbainemohamed/getting-started-with-hadoop/blob/9c92d432ad7627750c771808fb6ac9cc4dc13a65/screens/screen9.png)

------------------------------------------------

![download](https://github.com/isbainemohamed/getting-started-with-hadoop/blob/9c92d432ad7627750c771808fb6ac9cc4dc13a65/screens/aknowledegement.png)
