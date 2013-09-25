filecrusher
===========
This is a fork of the original filecrusher found here:
http://www.jointhegrid.com/hadoop_filecrush/

This was built using Cloudera Hadoop (CDH 4.3.1) libraries.

In order to build you will need to clone the repository and run the following:

mvn package

This should give you a nice jar that you can than use to combine your small files into larger files.

hadoop jar /root/filecrush-2.0-SNAPSHOT.jar crush.Crush --help

hadoop jar /root/filecrush-2.0-SNAPSHOT.jar crush.Crush --verbose /tmp/crushNew/user/flume/SmallFiles/08/28/13/ /tmp/crush2

