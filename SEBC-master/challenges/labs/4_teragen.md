$time hadoop jar /opt/cloudera/parcels/CDH-5.9.0-1.cdh5.9.0.p0.23/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -Ddfs.block.size=33554432 -Dmapreduce.map.log.level=INFO -Dmapreduce.reduce.log.level=INFO -Dyarn.app.mapreduce.am.log.level=INFO -Dmapreduce.map.memory.mb=1024 -Dmapred.map.tasks=12 65536000 /user/saturn/tgen


17/06/23 04:50:32 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-36-93.eu-west-1.compute.internal/172.31.36.93:8032
17/06/23 04:50:32 INFO terasort.TeraSort: Generating 65536000 using 12
17/06/23 04:50:32 INFO mapreduce.JobSubmitter: number of splits:12
17/06/23 04:50:32 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
17/06/23 04:50:32 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/06/23 04:50:33 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1498205579892_0001
17/06/23 04:50:33 INFO impl.YarnClientImpl: Submitted application application_1498205579892_0001
17/06/23 04:50:33 INFO mapreduce.Job: The url to track the job: http://ip-172-31-36-93.eu-west-1.compute.internal:8088/proxy/application_1498205579892_0001/
17/06/23 04:50:33 INFO mapreduce.Job: Running job: job_1498205579892_0001
17/06/23 04:50:39 INFO mapreduce.Job: Job job_1498205579892_0001 running in uber mode : false
17/06/23 04:50:39 INFO mapreduce.Job:  map 0% reduce 0%
17/06/23 04:50:52 INFO mapreduce.Job:  map 4% reduce 0%
17/06/23 04:50:55 INFO mapreduce.Job:  map 17% reduce 0%
17/06/23 04:50:57 INFO mapreduce.Job:  map 20% reduce 0%
17/06/23 04:50:58 INFO mapreduce.Job:  map 24% reduce 0%
17/06/23 04:51:00 INFO mapreduce.Job:  map 25% reduce 0%
17/06/23 04:51:01 INFO mapreduce.Job:  map 28% reduce 0%
17/06/23 04:51:03 INFO mapreduce.Job:  map 30% reduce 0%
17/06/23 04:51:04 INFO mapreduce.Job:  map 33% reduce 0%
17/06/23 04:51:06 INFO mapreduce.Job:  map 35% reduce 0%
17/06/23 04:51:07 INFO mapreduce.Job:  map 37% reduce 0%
17/06/23 04:51:09 INFO mapreduce.Job:  map 38% reduce 0%
17/06/23 04:51:10 INFO mapreduce.Job:  map 39% reduce 0%
17/06/23 04:51:15 INFO mapreduce.Job:  map 40% reduce 0%
17/06/23 04:51:16 INFO mapreduce.Job:  map 43% reduce 0%
17/06/23 04:51:17 INFO mapreduce.Job:  map 44% reduce 0%
17/06/23 04:51:18 INFO mapreduce.Job:  map 47% reduce 0%
17/06/23 04:51:19 INFO mapreduce.Job:  map 51% reduce 0%
17/06/23 04:51:22 INFO mapreduce.Job:  map 53% reduce 0%
17/06/23 04:51:23 INFO mapreduce.Job:  map 55% reduce 0%
17/06/23 04:51:25 INFO mapreduce.Job:  map 58% reduce 0%
17/06/23 04:51:26 INFO mapreduce.Job:  map 59% reduce 0%
17/06/23 04:51:28 INFO mapreduce.Job:  map 63% reduce 0%
17/06/23 04:51:31 INFO mapreduce.Job:  map 67% reduce 0%
17/06/23 04:51:34 INFO mapreduce.Job:  map 70% reduce 0%
17/06/23 04:51:37 INFO mapreduce.Job:  map 72% reduce 0%
17/06/23 04:51:40 INFO mapreduce.Job:  map 77% reduce 0%
17/06/23 04:51:43 INFO mapreduce.Job:  map 80% reduce 0%
17/06/23 04:51:45 INFO mapreduce.Job:  map 81% reduce 0%
17/06/23 04:51:46 INFO mapreduce.Job:  map 84% reduce 0%
17/06/23 04:51:48 INFO mapreduce.Job:  map 85% reduce 0%
17/06/23 04:51:49 INFO mapreduce.Job:  map 88% reduce 0%
17/06/23 04:51:51 INFO mapreduce.Job:  map 89% reduce 0%
17/06/23 04:51:52 INFO mapreduce.Job:  map 93% reduce 0%
17/06/23 04:51:54 INFO mapreduce.Job:  map 94% reduce 0%
17/06/23 04:51:55 INFO mapreduce.Job:  map 96% reduce 0%
17/06/23 04:52:00 INFO mapreduce.Job:  map 97% reduce 0%
17/06/23 04:52:01 INFO mapreduce.Job:  map 98% reduce 0%
17/06/23 04:52:03 INFO mapreduce.Job:  map 100% reduce 0%
17/06/23 04:52:03 INFO mapreduce.Job: Job job_1498205579892_0001 completed successfully
17/06/23 04:52:03 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=1474778
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=1025
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=48
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=24
        Job Counters
                Launched map tasks=12
                Other local map tasks=12
                Total time spent by all maps in occupied slots (ms)=870386
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=870386
                Total vcore-seconds taken by all map tasks=870386
                Total megabyte-seconds taken by all map tasks=891275264
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=1025
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=2817
                CPU time spent (ms)=155250
                Physical memory (bytes) snapshot=4340305920
                Virtual memory (bytes) snapshot=19081736192
                Total committed heap usage (bytes)=4591714304
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000

real    1m34.240s
user    0m6.033s
sys     0m0.274s




$ hdfs dfs -ls /user/saturn/tgen

Found 13 items
-rw-r--r--   3 saturn supergroup          0 2017-06-23 04:52 /user/saturn/tgen/_SUCCESS
-rw-r--r--   3 saturn supergroup  546133400 2017-06-23 04:52 /user/saturn/tgen/part-m-00000
-rw-r--r--   3 saturn supergroup  546133300 2017-06-23 04:52 /user/saturn/tgen/part-m-00001
-rw-r--r--   3 saturn supergroup  546133300 2017-06-23 04:51 /user/saturn/tgen/part-m-00002
-rw-r--r--   3 saturn supergroup  546133400 2017-06-23 04:51 /user/saturn/tgen/part-m-00003
-rw-r--r--   3 saturn supergroup  546133300 2017-06-23 04:51 /user/saturn/tgen/part-m-00004
-rw-r--r--   3 saturn supergroup  546133300 2017-06-23 04:51 /user/saturn/tgen/part-m-00005
-rw-r--r--   3 saturn supergroup  546133400 2017-06-23 04:51 /user/saturn/tgen/part-m-00006
-rw-r--r--   3 saturn supergroup  546133300 2017-06-23 04:51 /user/saturn/tgen/part-m-00007
-rw-r--r--   3 saturn supergroup  546133300 2017-06-23 04:51 /user/saturn/tgen/part-m-00008
-rw-r--r--   3 saturn supergroup  546133400 2017-06-23 04:51 /user/saturn/tgen/part-m-00009
-rw-r--r--   3 saturn supergroup  546133300 2017-06-23 04:51 /user/saturn/tgen/part-m-00010
-rw-r--r--   3 saturn supergroup  546133300 2017-06-23 04:52 /user/saturn/tgen/part-m-00011
[saturn@ip-172-31-38-33 lib]$ ^C
