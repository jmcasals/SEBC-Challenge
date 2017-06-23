
time hadoop jar /opt/cloudera/parcels/CDH-5.9.0-1.cdh5.9.0.p0.23/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar  pi 10 100
Number of Maps  = 10
Samples per Map = 100
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Wrote input for Map #5
Wrote input for Map #6
Wrote input for Map #7
Wrote input for Map #8
Wrote input for Map #9
Starting Job
17/06/23 07:05:31 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-18-33.eu-west-1.compute.internal/172.31.18.33:8032
17/06/23 07:05:31 INFO hdfs.DFSClient: Created token for haley: HDFS_DELEGATION_TOKEN owner=haley@JMCASALS.PA, renewer=yarn, realUser=, issueDate=1498215931757, maxDate=1498820731757, sequenceNumber=3, masterKeyId=6 on 172.31.18.33:8020
17/06/23 07:05:31 INFO security.TokenCache: Got dt for hdfs://ip-172-31-18-33.eu-west-1.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.18.33:8020, Ident: (token for haley: HDFS_DELEGATION_TOKEN owner=haley@JMCASALS.PA, renewer=yarn, realUser=, issueDate=1498215931757, maxDate=1498820731757, sequenceNumber=3, masterKeyId=6)
17/06/23 07:05:31 INFO input.FileInputFormat: Total input paths to process : 10
17/06/23 07:05:31 INFO mapreduce.JobSubmitter: number of splits:10
17/06/23 07:05:32 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1498212369276_0001
17/06/23 07:05:32 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.18.33:8020, Ident: (token for haley: HDFS_DELEGATION_TOKEN owner=haley@JMCASALS.PA, renewer=yarn, realUser=, issueDate=1498215931757, maxDate=1498820731757, sequenceNumber=3, masterKeyId=6)
17/06/23 07:05:33 INFO impl.YarnClientImpl: Submitted application application_1498212369276_0001
17/06/23 07:05:33 INFO mapreduce.Job: The url to track the job: http://ip-172-31-18-33.eu-west-1.compute.internal:8088/proxy/application_1498212369276_0001/
17/06/23 07:05:33 INFO mapreduce.Job: Running job: job_1498212369276_0001
17/06/23 07:05:42 INFO mapreduce.Job: Job job_1498212369276_0001 running in uber mode : false
17/06/23 07:05:42 INFO mapreduce.Job:  map 0% reduce 0%
17/06/23 07:05:47 INFO mapreduce.Job:  map 10% reduce 0%
17/06/23 07:05:56 INFO mapreduce.Job:  map 100% reduce 0%
17/06/23 07:06:03 INFO mapreduce.Job:  map 100% reduce 100%
17/06/23 07:06:03 INFO mapreduce.Job: Job job_1498212369276_0001 completed successfully
17/06/23 07:06:03 INFO mapreduce.Job: Counters: 53
        File System Counters
                FILE: Number of bytes read=94
                FILE: Number of bytes written=1420237
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=2990
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=43
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=10
                Launched reduce tasks=1
                Data-local map tasks=10
                Total time spent by all maps in occupied slots (ms)=109531
                Total time spent by all reduces in occupied slots (ms)=3402
                Total time spent by all map tasks (ms)=109531
                Total time spent by all reduce tasks (ms)=3402
                Total vcore-milliseconds taken by all map tasks=109531
                Total vcore-milliseconds taken by all reduce tasks=3402
                Total megabyte-milliseconds taken by all map tasks=112159744
                Total megabyte-milliseconds taken by all reduce tasks=3483648
        Map-Reduce Framework
                Map input records=10
                Map output records=20
                Map output bytes=180
                Map output materialized bytes=340
                Input split bytes=1810
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=340
                Reduce input records=20
                Reduce output records=0
                Spilled Records=40
                Shuffled Maps =10
                Failed Shuffles=0
                Merged Map outputs=10
                GC time elapsed (ms)=780
                CPU time spent (ms)=8310
                Physical memory (bytes) snapshot=4957507584
                Virtual memory (bytes) snapshot=17396092928
                Total committed heap usage (bytes)=5697961984
                Peak Map Physical memory (bytes)=508751872
                Peak Map Virtual memory (bytes)=1598341120
                Peak Reduce Physical memory (bytes)=195518464
                Peak Reduce Virtual memory (bytes)=1597779968
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=1180
        File Output Format Counters
                Bytes Written=97
Job Finished in 31.606 seconds
Estimated value of Pi is 3.14800000000000000000
 
real    0m34.802s
user    0m5.884s
sys     0m0.365s
