## Hive Notes

1. HDFS Command
---

Command|Comments|
 ----------- | ----------- |
`hadoop fs –mkdir /user/lab `| create a directory on hdfs|
`hadoop fs –ls /user/lab `| list the files in the directory
`hadoop fs –put myFile.txt /user/lab `| move a file from local fs to hdfs|
<code> hadoop fs –cat /user/lab/myFile.txt &#124; head </code>| display the content of a file|
`hadoop fs –get /user/lab/myFile.txt `| move a file from hdfs to local fs|
`hadoop fs –rmdir /user/lab ``| remove a directory on hdfs|

2. Hive
- create tab-delimited table
<code>
create table full_text (
  id string,
  ts string,
  lat_lon string,
  lat string,
  lon string,
  tweet string)
  row format delimited
  fields terminated by '\t' ; </code>
