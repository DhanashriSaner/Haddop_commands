# Hadoop_commands
<h3>ls command</h3>
The ls command in Hadoop shows the list of files/contents in a specified directory, i.e., path<br>

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




