time hadoop jar /opt/cloudera/parcels/CDH-5.9.0-1.cdh5.9.0.p0.23/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/saturn/tgen /user/saturn/tsort

17/06/23 07:29:35 INFO terasort.TeraSort: starting
17/06/23 07:29:36 INFO hdfs.DFSClient: Created token for saturn: HDFS_DELEGATION_TOKEN owner=saturn@JMCASALS.PA, renewer=yarn, realUser=, issueDate=1498217376720, maxDate=1498822176720, sequenceNumber=6, masterKeyId=6 on 172.31.38.33:8020
17/06/23 07:29:36 INFO security.TokenCache: Got dt for hdfs://ip-172-31-18-168.eu-west-1.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.38.33:8020, Ident: (token for saturn: HDFS_DELEGATION_TOKEN owner=saturn@JMCASALS.PA, renewer=yarn, realUser=, issueDate=1498217376720, maxDate=1498822176720, sequenceNumber=6, masterKeyId=6)
17/06/23 07:29:36 INFO input.FileInputFormat: Total input paths to process : 12
Spent 310ms computing base-splits.
Spent 5ms computing TeraScheduler splits.
Computing input splits took 315ms
Sampling 10 splits of 204
Making 8 from 100000 sampled records
Computing parititions took 656ms
Spent 974ms computing partitions.
17/06/23 07:29:37 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-38-33.eu-west-1.compute.internal/172.31.38.33:8032
17/06/23 07:29:37 INFO mapreduce.JobSubmitter: number of splits:204
17/06/23 07:29:38 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1498212369276_0003
17/06/23 07:29:38 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.38.33:8020, Ident: (token for saturn: HDFS_DELEGATION_TOKEN owner=saturn@JMCASALS.PA, renewer=yarn, realUser=, issueDate=1498217376720, maxDate=1498822176720, sequenceNumber=6, masterKeyId=6)
17/06/23 07:29:38 INFO impl.YarnClientImpl: Submitted application application_1498212369276_0003
17/06/23 07:29:38 INFO mapreduce.Job: The url to track the job: http://ip-172-31-18-168.eu-west-1.compute.internal:8088/proxy/application_1498212369276_0003/
17/06/23 07:29:38 INFO mapreduce.Job: Running job: job_1498212369276_0003
17/06/23 07:29:47 INFO mapreduce.Job: Job job_1498212369276_0003 running in uber mode : false
17/06/23 07:29:47 INFO mapreduce.Job:  map 0% reduce 0%
17/06/23 07:29:58 INFO mapreduce.Job:  map 1% reduce 0%
17/06/23 07:30:06 INFO mapreduce.Job:  map 6% reduce 0%
17/06/23 07:30:07 INFO mapreduce.Job:  map 8% reduce 0%
17/06/23 07:30:08 INFO mapreduce.Job:  map 9% reduce 0%
17/06/23 07:30:18 INFO mapreduce.Job:  map 10% reduce 0%
17/06/23 07:30:19 INFO mapreduce.Job:  map 12% reduce 0%
17/06/23 07:30:20 INFO mapreduce.Job:  map 16% reduce 0%
17/06/23 07:30:28 INFO mapreduce.Job:  map 17% reduce 0%
17/06/23 07:30:29 INFO mapreduce.Job:  map 18% reduce 0%
17/06/23 07:30:31 INFO mapreduce.Job:  map 20% reduce 0%
17/06/23 07:30:32 INFO mapreduce.Job:  map 23% reduce 0%
17/06/23 07:30:33 INFO mapreduce.Job:  map 24% reduce 0%
17/06/23 07:30:38 INFO mapreduce.Job:  map 25% reduce 0%
17/06/23 07:30:43 INFO mapreduce.Job:  map 26% reduce 0%
17/06/23 07:30:44 INFO mapreduce.Job:  map 27% reduce 0%
17/06/23 07:30:45 INFO mapreduce.Job:  map 30% reduce 0%
17/06/23 07:30:46 INFO mapreduce.Job:  map 31% reduce 0%
17/06/23 07:30:49 INFO mapreduce.Job:  map 32% reduce 0%
17/06/23 07:30:54 INFO mapreduce.Job:  map 33% reduce 0%
17/06/23 07:30:55 INFO mapreduce.Job:  map 34% reduce 0%
17/06/23 07:30:56 INFO mapreduce.Job:  map 35% reduce 0%
17/06/23 07:30:57 INFO mapreduce.Job:  map 38% reduce 0%
17/06/23 07:30:58 INFO mapreduce.Job:  map 40% reduce 0%
17/06/23 07:31:06 INFO mapreduce.Job:  map 41% reduce 0%
17/06/23 07:31:07 INFO mapreduce.Job:  map 42% reduce 0%
17/06/23 07:31:08 INFO mapreduce.Job:  map 44% reduce 0%
17/06/23 07:31:09 INFO mapreduce.Job:  map 46% reduce 0%
17/06/23 07:31:10 INFO mapreduce.Job:  map 47% reduce 0%
17/06/23 07:31:15 INFO mapreduce.Job:  map 48% reduce 0%
17/06/23 07:31:17 INFO mapreduce.Job:  map 49% reduce 0%
17/06/23 07:31:18 INFO mapreduce.Job:  map 50% reduce 0%
17/06/23 07:31:20 INFO mapreduce.Job:  map 51% reduce 0%
17/06/23 07:31:21 INFO mapreduce.Job:  map 53% reduce 0%
17/06/23 07:31:22 INFO mapreduce.Job:  map 54% reduce 0%
17/06/23 07:31:24 INFO mapreduce.Job:  map 55% reduce 0%
17/06/23 07:31:26 INFO mapreduce.Job:  map 56% reduce 0%
17/06/23 07:31:31 INFO mapreduce.Job:  map 57% reduce 0%
17/06/23 07:31:32 INFO mapreduce.Job:  map 58% reduce 0%
17/06/23 07:31:33 INFO mapreduce.Job:  map 60% reduce 0%
17/06/23 07:31:34 INFO mapreduce.Job:  map 62% reduce 0%
17/06/23 07:31:35 INFO mapreduce.Job:  map 63% reduce 0%
17/06/23 07:31:41 INFO mapreduce.Job:  map 64% reduce 0%
17/06/23 07:31:43 INFO mapreduce.Job:  map 65% reduce 0%
17/06/23 07:31:44 INFO mapreduce.Job:  map 68% reduce 0%
17/06/23 07:31:45 INFO mapreduce.Job:  map 69% reduce 0%
17/06/23 07:31:46 INFO mapreduce.Job:  map 70% reduce 0%
17/06/23 07:31:47 INFO mapreduce.Job:  map 71% reduce 0%
17/06/23 07:31:52 INFO mapreduce.Job:  map 72% reduce 0%
17/06/23 07:31:54 INFO mapreduce.Job:  map 73% reduce 0%
17/06/23 07:31:55 INFO mapreduce.Job:  map 74% reduce 0%
17/06/23 07:31:56 INFO mapreduce.Job:  map 75% reduce 0%
17/06/23 07:31:58 INFO mapreduce.Job:  map 77% reduce 0%
17/06/23 07:32:00 INFO mapreduce.Job:  map 78% reduce 0%
17/06/23 07:32:04 INFO mapreduce.Job:  map 80% reduce 0%
17/06/23 07:32:08 INFO mapreduce.Job:  map 82% reduce 0%
17/06/23 07:32:09 INFO mapreduce.Job:  map 84% reduce 0%
17/06/23 07:32:11 INFO mapreduce.Job:  map 85% reduce 0%
17/06/23 07:32:13 INFO mapreduce.Job:  map 86% reduce 0%
17/06/23 07:32:14 INFO mapreduce.Job:  map 87% reduce 0%
17/06/23 07:32:20 INFO mapreduce.Job:  map 89% reduce 0%
17/06/23 07:32:24 INFO mapreduce.Job:  map 91% reduce 0%
17/06/23 07:32:29 INFO mapreduce.Job:  map 91% reduce 4%
17/06/23 07:32:30 INFO mapreduce.Job:  map 91% reduce 11%
17/06/23 07:32:31 INFO mapreduce.Job:  map 92% reduce 23%
17/06/23 07:32:32 INFO mapreduce.Job:  map 93% reduce 27%
17/06/23 07:32:33 INFO mapreduce.Job:  map 94% reduce 27%
17/06/23 07:32:34 INFO mapreduce.Job:  map 95% reduce 27%
17/06/23 07:32:38 INFO mapreduce.Job:  map 96% reduce 28%
17/06/23 07:32:39 INFO mapreduce.Job:  map 97% reduce 28%
17/06/23 07:32:41 INFO mapreduce.Job:  map 98% reduce 28%
17/06/23 07:32:42 INFO mapreduce.Job:  map 99% reduce 28%
17/06/23 07:32:43 INFO mapreduce.Job:  map 100% reduce 28%
17/06/23 07:32:44 INFO mapreduce.Job:  map 100% reduce 29%
17/06/23 07:32:47 INFO mapreduce.Job:  map 100% reduce 33%
17/06/23 07:32:48 INFO mapreduce.Job:  map 100% reduce 42%
17/06/23 07:32:50 INFO mapreduce.Job:  map 100% reduce 54%
17/06/23 07:32:51 INFO mapreduce.Job:  map 100% reduce 59%
17/06/23 07:32:53 INFO mapreduce.Job:  map 100% reduce 61%
17/06/23 07:32:54 INFO mapreduce.Job:  map 100% reduce 65%
17/06/23 07:32:56 INFO mapreduce.Job:  map 100% reduce 71%
17/06/23 07:32:58 INFO mapreduce.Job:  map 100% reduce 77%
17/06/23 07:32:59 INFO mapreduce.Job:  map 100% reduce 79%
17/06/23 07:33:00 INFO mapreduce.Job:  map 100% reduce 81%
17/06/23 07:33:02 INFO mapreduce.Job:  map 100% reduce 87%
17/06/23 07:33:04 INFO mapreduce.Job:  map 100% reduce 92%
17/06/23 07:33:06 INFO mapreduce.Job:  map 100% reduce 93%
17/06/23 07:33:08 INFO mapreduce.Job:  map 100% reduce 96%
17/06/23 07:33:09 INFO mapreduce.Job:  map 100% reduce 97%
17/06/23 07:33:10 INFO mapreduce.Job:  map 100% reduce 99%
17/06/23 07:33:12 INFO mapreduce.Job:  map 100% reduce 100%
17/06/23 07:33:13 INFO mapreduce.Job: Job job_1498212369276_0003 completed successfully
17/06/23 07:33:13 INFO mapreduce.Job: Counters: 53
        File System Counters
                FILE: Number of bytes read=2911712891
                FILE: Number of bytes written=5785394065
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=6553633048
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=636
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=204
                Launched reduce tasks=8
                Data-local map tasks=204
                Total time spent by all maps in occupied slots (ms)=2141342
                Total time spent by all reduces in occupied slots (ms)=404808
                Total time spent by all map tasks (ms)=2141342
                Total time spent by all reduce tasks (ms)=404808
                Total vcore-milliseconds taken by all map tasks=2141342
                Total vcore-milliseconds taken by all reduce tasks=404808
                Total megabyte-milliseconds taken by all map tasks=2192734208
                Total megabyte-milliseconds taken by all reduce tasks=414523392
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Map output bytes=6684672000
                Map output materialized bytes=2846142396
                Input split bytes=33048
                Combine input records=0
                Combine output records=0
                Reduce input groups=65536000
                Reduce shuffle bytes=2846142396
                Reduce input records=65536000
                Reduce output records=65536000
                Spilled Records=131072000
                Shuffled Maps =1632
                Failed Shuffles=0
                Merged Map outputs=1632
                GC time elapsed (ms)=35360
                CPU time spent (ms)=1040140
                Physical memory (bytes) snapshot=109119488000
                Virtual memory (bytes) snapshot=334989172736
                Total committed heap usage (bytes)=120312561664
                Peak Map Physical memory (bytes)=525205504
                Peak Map Virtual memory (bytes)=1599369216
                Peak Reduce Physical memory (bytes)=948789248
                Peak Reduce Virtual memory (bytes)=1610989568
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=6553600000
        File Output Format Counters
                Bytes Written=6553600000
17/06/23 07:33:13 INFO terasort.TeraSort: done
