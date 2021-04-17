(Q1) What do you think the line job.setJarByClass(Filter.class); does? <br />
I think by using this setJarByClass method we tell Hadoop to find out the relevant jar by finding out that the class specified as it's parameter to be present as part of that jar. 
Here we help Hadoop to find out that which jar it should send to nodes to perform Map and Reduce tasks.<br />
(Q2) What is the effect of the line job.setNumReduceTasks(0);? <br />
It means we don't have any reducer job here.<br />
(Q3) Where does the main function run? (Driver node, Master node, or an execturo node).<br />
I think it runs on the driver node since the driver node creates new configuration, sets the path and filesystem.<br />
(Q4) How many lines do you see in the output?<br />
Map output records=27972<br />
(Q5) Local file system: How many files are produced in the output?<br />
4 files <br />
![alt text](https://github.com/ClaireDong0403/CS167/blob/main/lab3/Q5.png)<br />
(Q6) Explain this number based on the input file size and default block size.<br />
Bytes Read=2339220 = 2.33 MB which should be smaller than the default block size. So there is only one block created. Therefore we have one output file: part-m-00000.<br />
(Q7) HDFS: How many files are produced in the output?
2 files: '_SUCCESS' and 'part-m-00000'
