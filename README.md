# Simple use and setup of Hadoop
Setup
----
- [Single machine and Pseudo-distributed Settings](http://www.powerxing.com/install-hadoop.html)
- [Distributed Settings](http://www.powerxing.com/install-hadoop-cluster/)

Use of commands
----
- Adding the directory of `bin` to environmental variable `PATH`, then you can use any command inside `bin`. For example, you can 
  directly use `hdfs dfs -ls` while you are at `~` directory.
- Have been in Hadoop directory, we can use `bin/hdfs` to look up all the commands.
- Using `bin/hdfs dfs -ls` to skim all directories in HDFS.

JAVA_HOME not found problem
----
- Occurring `JAVA_HOME not found` problem when doing `./bin/hdfs/ namenode -format` or `./sbin/start-dfs.sh`. First to check whether
`java -version` is successful or `JAVA_HOME` in `etc/profile` is correct, then add `JAVA_HOME` to `~/.bashrc`. If it still doesn't
work, then modify `JAVA_HOME` of `hadoop-env.sh` in `hadoop/etc/hadoop`.
