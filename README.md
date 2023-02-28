# Hadoop_commands
<h3>ls command</h3>
The ls command listing contents inside a directory<br>

```
ls
```
<br>

hadoop fs ls command <br>
```
hdfs dfs -ls /
```
**OR** <br>
```
hadoop fs -ls /
```
<br>
<h3> If we want to create file named as 'test' with extension '.txt' inside cloudera, we will use following command </h3>

```
vi test.txt
```
<br>
<h3> Copy the file 'test.txt' from local and then use it in hdfs user directory</h3>

```
hadoop fs -copyFromLocal test.txt /user
```
<h3> Delete file</h3>

```
rm test.txt
```
<br>
<h3> Check the present working directory </h3>

```
pwd
```
<h3> Command to check the Deamon is up or not </h3>

```
jps
```
<h3> Command to check the version of hadoop </h3>

```
hadoop version
```
<h3> Command to create new directory named 'xyz' in Local </h3>

```
mkdir xyz
```
<h3> Command to create new directory named 'abc' in hadoop </h3>

```
hadoop fs -mkdir /abc
```
<br>
<br>

<h1> Hadoop wordcount program </h1>

<img align="center" alt="Hadoop_wordcount_program" width = 300 src="https://user-images.githubusercontent.com/88526990/221773883-dd6e1b53-28e0-43dc-b482-d6e1961cf226.jpg"><br>

we want to perform wordcount on the above given words
<br>
<h4> Make the Directory named as 'wordcount' in HDFS </h4>

```
hadoop fs -mkdir wordcount/
```

<h4> Make the Sub-Directory namely 'input' and 'output inside the 'wordcount' Directory in HDFS </h4>

```
hadoop fs -mkdir wordcount/input
```
<h4>Output sub-directory</h4>

```
hadoop fs -mkdir wordcount/output
```

<h4> Make the words.txt file in local system </h4>

```
vi words.txt
```
<br>

<h4> Place the file 'words.txt' from local system into HDFS input sub-directory using following put command </h4>

```
hadoop fs -put words.txt /wordcount/input 
```

