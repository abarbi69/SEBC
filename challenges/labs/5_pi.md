```
[frankola@ip-172-31-44-217 ~]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar pi 50 100
Number of Maps  = 50
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
Wrote input for Map #10
Wrote input for Map #11
Wrote input for Map #12
Wrote input for Map #13
Wrote input for Map #14
Wrote input for Map #15
Wrote input for Map #16
Wrote input for Map #17
Wrote input for Map #18
Wrote input for Map #19
Wrote input for Map #20
Wrote input for Map #21
Wrote input for Map #22
Wrote input for Map #23
Wrote input for Map #24
Wrote input for Map #25
Wrote input for Map #26
Wrote input for Map #27
Wrote input for Map #28
Wrote input for Map #29
Wrote input for Map #30
Wrote input for Map #31
Wrote input for Map #32
Wrote input for Map #33
Wrote input for Map #34
Wrote input for Map #35
Wrote input for Map #36
Wrote input for Map #37
Wrote input for Map #38
Wrote input for Map #39
Wrote input for Map #40
Wrote input for Map #41
Wrote input for Map #42
Wrote input for Map #43
Wrote input for Map #44
Wrote input for Map #45
Wrote input for Map #46
Wrote input for Map #47
Wrote input for Map #48
Wrote input for Map #49
Starting Job
17/11/03 07:44:47 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-42-252.eu-central-1.compute.internal/172.31.42.252:8032
17/11/03 07:44:47 INFO hdfs.DFSClient: Created token for frankola: HDFS_DELEGATION_TOKEN owner=frankola@ABARBI69.FNG, renewer=yarn, realUser=, issueDate=1509709487534, maxDate=1510314287534, sequenceNumber=2, masterKeyId=2 on 172.31.35.238:8020
17/11/03 07:44:47 INFO security.TokenCache: Got dt for hdfs://ip-172-31-35-238.eu-central-1.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.35.238:8020, Ident: (token for frankola: HDFS_DELEGATION_TOKEN owner=frankola@ABARBI69.FNG, renewer=yarn, realUser=, issueDate=1509709487534, maxDate=1510314287534, sequenceNumber=2, masterKeyId=2)
17/11/03 07:44:47 INFO input.FileInputFormat: Total input paths to process : 50
17/11/03 07:44:47 INFO mapreduce.JobSubmitter: number of splits:50
17/11/03 07:44:47 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1509708469036_0002
17/11/03 07:44:47 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.35.238:8020, Ident: (token for frankola: HDFS_DELEGATION_TOKEN owner=frankola@ABARBI69.FNG, renewer=yarn, realUser=, issueDate=1509709487534, maxDate=1510314287534, sequenceNumber=2, masterKeyId=2)
17/11/03 07:44:48 INFO impl.YarnClientImpl: Submitted application application_1509708469036_0002
17/11/03 07:44:48 INFO mapreduce.Job: The url to track the job: http://ip-172-31-42-252.eu-central-1.compute.internal:8088/proxy/application_1509708469036_0002/
17/11/03 07:44:48 INFO mapreduce.Job: Running job: job_1509708469036_0002
17/11/03 07:44:56 INFO mapreduce.Job: Job job_1509708469036_0002 running in uber mode : false
17/11/03 07:44:56 INFO mapreduce.Job:  map 0% reduce 0%
17/11/03 07:45:03 INFO mapreduce.Job:  map 4% reduce 0%
17/11/03 07:45:07 INFO mapreduce.Job:  map 8% reduce 0%
17/11/03 07:45:08 INFO mapreduce.Job:  map 20% reduce 0%
17/11/03 07:45:12 INFO mapreduce.Job:  map 24% reduce 0%
17/11/03 07:45:16 INFO mapreduce.Job:  map 40% reduce 0%
17/11/03 07:45:20 INFO mapreduce.Job:  map 44% reduce 0%
17/11/03 07:45:22 INFO mapreduce.Job:  map 46% reduce 0%
17/11/03 07:45:23 INFO mapreduce.Job:  map 56% reduce 0%
17/11/03 07:45:24 INFO mapreduce.Job:  map 60% reduce 0%
17/11/03 07:45:28 INFO mapreduce.Job:  map 64% reduce 0%
17/11/03 07:45:29 INFO mapreduce.Job:  map 68% reduce 0%
17/11/03 07:45:30 INFO mapreduce.Job:  map 76% reduce 0%
17/11/03 07:45:32 INFO mapreduce.Job:  map 80% reduce 0%
17/11/03 07:45:35 INFO mapreduce.Job:  map 86% reduce 0%
17/11/03 07:45:36 INFO mapreduce.Job:  map 90% reduce 0%
17/11/03 07:45:37 INFO mapreduce.Job:  map 96% reduce 0%
17/11/03 07:45:39 INFO mapreduce.Job:  map 98% reduce 0%
17/11/03 07:45:40 INFO mapreduce.Job:  map 100% reduce 100%
17/11/03 07:45:41 INFO mapreduce.Job: Job job_1509708469036_0002 completed successfully
17/11/03 07:45:42 INFO mapreduce.Job: Counters: 50
        File System Counters
                FILE: Number of bytes read=257
                FILE: Number of bytes written=6323749
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=15240
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=203
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=50
                Launched reduce tasks=1
                Data-local map tasks=49
                Rack-local map tasks=1
                Total time spent by all maps in occupied slots (ms)=271993
                Total time spent by all reduces in occupied slots (ms)=4128
                Total time spent by all map tasks (ms)=271993
                Total time spent by all reduce tasks (ms)=4128
                Total vcore-seconds taken by all map tasks=271993
                Total vcore-seconds taken by all reduce tasks=4128
                Total megabyte-seconds taken by all map tasks=278520832
                Total megabyte-seconds taken by all reduce tasks=4227072
        Map-Reduce Framework
                Map input records=50
                Map output records=100
                Map output bytes=900
                Map output materialized bytes=1700
                Input split bytes=9340
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=1700
                Reduce input records=100
                Reduce output records=0
                Spilled Records=200
                Shuffled Maps =50
                Failed Shuffles=0
                Merged Map outputs=50
                GC time elapsed (ms)=1725
                CPU time spent (ms)=26790
                Physical memory (bytes) snapshot=23183851520
                Virtual memory (bytes) snapshot=80644251648
                Total committed heap usage (bytes)=26474971136
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=5900
        File Output Format Counters
                Bytes Written=97
Job Finished in 54.734 seconds
Estimated value of Pi is 3.14160000000000000000
```
