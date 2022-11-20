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
screen1

* 2nd step :

Extract the tar file in the currently directory.

```bash
tar -xvf hadoop-3.2.3.tar.gz
```

screen2

3rd Step: 

Navigate to the hadoop-3.2.3 directory.

```bash
cd hadoop-3.2.3
```

screen3

4th Step: 

Check the hadoop command to see if it is setup. This will display the usage documentation for the hadoop script.

```bash
bin/hadoop
```

screen4

5th Step:

Download data.txt to your current directory.

```bash
curl https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-BD0225EN-SkillsNetwork/labs/data/data.txt --output data.txt
```

screen5
