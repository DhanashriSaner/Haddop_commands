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
OR <br>
```
hadoop fs -ls /
```
<br>
<h3> if we want to create file named as 'test' with extension '.txt' inside cloudera, we will use following command </h3>

```
vi test.txt
```
<br>
<h3> copy the file 'test.txt' from local and then use it in hdfs user directory</h3>

```
hadoop fs -copyFromLocal test.txt /user
```



