```
su - reilly
Last failed login: Fri Nov  3 07:32:07 EDT 2017 on pts/0
There was 1 failed login attempt since the last successful login.
[reilly@ip-172-31-44-217 ~]$
[reilly@ip-172-31-44-217 ~]$
[reilly@ip-172-31-44-217 ~]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/reilly/tgen /user/reilly/tsort
17/11/03 07:32:32 INFO terasort.TeraSort: starting
17/11/03 07:32:33 WARN security.UserGroupInformation: PriviledgedActionException as:reilly (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Failed to find any Kerberos tgt)]
17/11/03 07:32:33 WARN ipc.Client: Exception encountered while connecting to the server : javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Failed to find any Kerberos tgt)]
17/11/03 07:32:33 WARN security.UserGroupInformation: PriviledgedActionException as:reilly (auth:KERBEROS) cause:java.io.IOException: javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Failed to find any Kerberos tgt)]
17/11/03 07:32:33 ERROR terasort.TeraSort: Failed on local exception: java.io.IOException: javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Failed to find any Kerberos tgt)]; Host Details : local host is: "ip-172-31-44-217.eu-central-1.compute.internal/172.31.44.217"; destination host is: "ip-172-31-35-238.eu-central-1.compute.internal":8020;
[reilly@ip-172-31-44-217 ~]$ kinit reilly@ABARBI69.FNG
Password for reilly@ABARBI69.FNG:
[reilly@ip-172-31-44-217 ~]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/reilly/tgen /user/reilly/tsort
17/11/03 07:32:56 INFO terasort.TeraSort: starting
17/11/03 07:32:57 INFO hdfs.DFSClient: Created token for reilly: HDFS_DELEGATION_TOKEN owner=reilly@ABARBI69.FNG, renewer=yarn, realUser=, issueDate=1509708777838, maxDate=1510313577838, sequenceNumber=1, masterKeyId=2 on 172.31.35.238:8020
17/11/03 07:32:57 INFO security.TokenCache: Got dt for hdfs://ip-172-31-35-238.eu-central-1.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.35.238:8020, Ident: (token for reilly: HDFS_DELEGATION_TOKEN owner=reilly@ABARBI69.FNG, renewer=yarn, realUser=, issueDate=1509708777838, maxDate=1510313577838, sequenceNumber=1, masterKeyId=2)
17/11/03 07:32:58 INFO input.FileInputFormat: Total input paths to process : 12
Spent 347ms computing base-splits.
Spent 5ms computing TeraScheduler splits.
Computing input splits took 353ms
Sampling 10 splits of 204
Making 10 from 100000 sampled records
Computing parititions took 865ms
Spent 1221ms computing partitions.
17/11/03 07:32:58 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-42-252.eu-central-1.compute.internal/172.31.42.252:8032
17/11/03 07:32:59 INFO mapreduce.JobSubmitter: number of splits:204
17/11/03 07:32:59 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1509708469036_0001
17/11/03 07:32:59 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.35.238:8020, Ident: (token for reilly: HDFS_DELEGATION_TOKEN owner=reilly@ABARBI69.FNG, renewer=yarn, realUser=, issueDate=1509708777838, maxDate=1510313577838, sequenceNumber=1, masterKeyId=2)
17/11/03 07:33:00 INFO impl.YarnClientImpl: Submitted application application_1509708469036_0001
17/11/03 07:33:00 INFO mapreduce.Job: The url to track the job: http://ip-172-31-42-252.eu-central-1.compute.internal:8088/proxy/application_1509708469036_0001/
17/11/03 07:33:00 INFO mapreduce.Job: Running job: job_1509708469036_0001
17/11/03 07:33:09 INFO mapreduce.Job: Job job_1509708469036_0001 running in uber mode : false
17/11/03 07:33:09 INFO mapreduce.Job:  map 0% reduce 0%
17/11/03 07:33:19 INFO mapreduce.Job:  map 1% reduce 0%
17/11/03 07:33:25 INFO mapreduce.Job:  map 4% reduce 0%
17/11/03 07:33:26 INFO mapreduce.Job:  map 5% reduce 0%
17/11/03 07:33:31 INFO mapreduce.Job:  map 6% reduce 0%
17/11/03 07:33:35 INFO mapreduce.Job:  map 9% reduce 0%
17/11/03 07:33:37 INFO mapreduce.Job:  map 10% reduce 0%
17/11/03 07:33:43 INFO mapreduce.Job:  map 11% reduce 0%
17/11/03 07:33:44 INFO mapreduce.Job:  map 13% reduce 0%
17/11/03 07:33:45 INFO mapreduce.Job:  map 14% reduce 0%
17/11/03 07:33:49 INFO mapreduce.Job:  map 15% reduce 0%
17/11/03 07:33:53 INFO mapreduce.Job:  map 16% reduce 0%
17/11/03 07:33:54 INFO mapreduce.Job:  map 17% reduce 0%
17/11/03 07:33:55 INFO mapreduce.Job:  map 19% reduce 0%
17/11/03 07:34:01 INFO mapreduce.Job:  map 20% reduce 0%
17/11/03 07:34:02 INFO mapreduce.Job:  map 21% reduce 0%
17/11/03 07:34:03 INFO mapreduce.Job:  map 22% reduce 0%
17/11/03 07:34:04 INFO mapreduce.Job:  map 23% reduce 0%
17/11/03 07:34:07 INFO mapreduce.Job:  map 24% reduce 0%
17/11/03 07:34:11 INFO mapreduce.Job:  map 26% reduce 0%
17/11/03 07:34:13 INFO mapreduce.Job:  map 27% reduce 0%
17/11/03 07:34:15 INFO mapreduce.Job:  map 28% reduce 0%
17/11/03 07:34:19 INFO mapreduce.Job:  map 29% reduce 0%
17/11/03 07:34:20 INFO mapreduce.Job:  map 30% reduce 0%
17/11/03 07:34:21 INFO mapreduce.Job:  map 32% reduce 0%
17/11/03 07:34:27 INFO mapreduce.Job:  map 33% reduce 0%
17/11/03 07:34:29 INFO mapreduce.Job:  map 34% reduce 0%
17/11/03 07:34:30 INFO mapreduce.Job:  map 35% reduce 0%
17/11/03 07:34:32 INFO mapreduce.Job:  map 37% reduce 0%
17/11/03 07:34:37 INFO mapreduce.Job:  map 38% reduce 0%
17/11/03 07:34:38 INFO mapreduce.Job:  map 39% reduce 0%
17/11/03 07:34:39 INFO mapreduce.Job:  map 40% reduce 0%
17/11/03 07:34:41 INFO mapreduce.Job:  map 41% reduce 0%
17/11/03 07:34:42 INFO mapreduce.Job:  map 42% reduce 0%
17/11/03 07:34:46 INFO mapreduce.Job:  map 43% reduce 0%
17/11/03 07:34:47 INFO mapreduce.Job:  map 44% reduce 0%
17/11/03 07:34:48 INFO mapreduce.Job:  map 45% reduce 0%
17/11/03 07:34:49 INFO mapreduce.Job:  map 46% reduce 0%
17/11/03 07:34:54 INFO mapreduce.Job:  map 47% reduce 0%
17/11/03 07:34:55 INFO mapreduce.Job:  map 48% reduce 0%
17/11/03 07:34:56 INFO mapreduce.Job:  map 49% reduce 0%
17/11/03 07:34:57 INFO mapreduce.Job:  map 50% reduce 0%
17/11/03 07:35:03 INFO mapreduce.Job:  map 51% reduce 0%
17/11/03 07:35:05 INFO mapreduce.Job:  map 52% reduce 0%
17/11/03 07:35:06 INFO mapreduce.Job:  map 54% reduce 0%
17/11/03 07:35:08 INFO mapreduce.Job:  map 55% reduce 0%
17/11/03 07:35:12 INFO mapreduce.Job:  map 56% reduce 0%
17/11/03 07:35:14 INFO mapreduce.Job:  map 57% reduce 0%
17/11/03 07:35:15 INFO mapreduce.Job:  map 58% reduce 0%
17/11/03 07:35:16 INFO mapreduce.Job:  map 59% reduce 0%
17/11/03 07:35:19 INFO mapreduce.Job:  map 60% reduce 0%
17/11/03 07:35:22 INFO mapreduce.Job:  map 61% reduce 0%
17/11/03 07:35:23 INFO mapreduce.Job:  map 62% reduce 0%
17/11/03 07:35:24 INFO mapreduce.Job:  map 63% reduce 0%
17/11/03 07:35:25 INFO mapreduce.Job:  map 64% reduce 0%
17/11/03 07:35:29 INFO mapreduce.Job:  map 65% reduce 0%
17/11/03 07:35:31 INFO mapreduce.Job:  map 66% reduce 0%
17/11/03 07:35:32 INFO mapreduce.Job:  map 67% reduce 0%
17/11/03 07:35:34 INFO mapreduce.Job:  map 68% reduce 0%
17/11/03 07:35:36 INFO mapreduce.Job:  map 69% reduce 0%
17/11/03 07:35:40 INFO mapreduce.Job:  map 70% reduce 0%
17/11/03 07:35:41 INFO mapreduce.Job:  map 71% reduce 0%
17/11/03 07:35:42 INFO mapreduce.Job:  map 72% reduce 0%
17/11/03 07:35:43 INFO mapreduce.Job:  map 73% reduce 0%
17/11/03 07:35:46 INFO mapreduce.Job:  map 74% reduce 0%
17/11/03 07:35:49 INFO mapreduce.Job:  map 75% reduce 0%
17/11/03 07:35:51 INFO mapreduce.Job:  map 77% reduce 0%
17/11/03 07:35:54 INFO mapreduce.Job:  map 78% reduce 0%
17/11/03 07:35:58 INFO mapreduce.Job:  map 79% reduce 0%
17/11/03 07:35:59 INFO mapreduce.Job:  map 80% reduce 0%
17/11/03 07:36:00 INFO mapreduce.Job:  map 81% reduce 0%
17/11/03 07:36:02 INFO mapreduce.Job:  map 82% reduce 0%
17/11/03 07:36:05 INFO mapreduce.Job:  map 83% reduce 0%
17/11/03 07:36:08 INFO mapreduce.Job:  map 84% reduce 0%
17/11/03 07:36:09 INFO mapreduce.Job:  map 86% reduce 0%
17/11/03 07:36:15 INFO mapreduce.Job:  map 86% reduce 2%
17/11/03 07:36:16 INFO mapreduce.Job:  map 86% reduce 5%
17/11/03 07:36:17 INFO mapreduce.Job:  map 86% reduce 8%
17/11/03 07:36:19 INFO mapreduce.Job:  map 87% reduce 8%
17/11/03 07:36:20 INFO mapreduce.Job:  map 87% reduce 9%
17/11/03 07:36:21 INFO mapreduce.Job:  map 87% reduce 14%
17/11/03 07:36:24 INFO mapreduce.Job:  map 87% reduce 15%
17/11/03 07:36:27 INFO mapreduce.Job:  map 88% reduce 15%
17/11/03 07:36:28 INFO mapreduce.Job:  map 89% reduce 15%
17/11/03 07:36:37 INFO mapreduce.Job:  map 90% reduce 15%
17/11/03 07:36:44 INFO mapreduce.Job:  map 91% reduce 15%
17/11/03 07:36:46 INFO mapreduce.Job:  map 92% reduce 15%
17/11/03 07:36:53 INFO mapreduce.Job:  map 93% reduce 15%
17/11/03 07:36:57 INFO mapreduce.Job:  map 93% reduce 16%
17/11/03 07:37:01 INFO mapreduce.Job:  map 94% reduce 16%
17/11/03 07:37:02 INFO mapreduce.Job:  map 95% reduce 16%
17/11/03 07:37:11 INFO mapreduce.Job:  map 96% reduce 16%
17/11/03 07:37:17 INFO mapreduce.Job:  map 97% reduce 16%
17/11/03 07:37:20 INFO mapreduce.Job:  map 98% reduce 16%
17/11/03 07:37:28 INFO mapreduce.Job:  map 99% reduce 16%
17/11/03 07:37:31 INFO mapreduce.Job:  map 99% reduce 17%
17/11/03 07:37:35 INFO mapreduce.Job:  map 100% reduce 17%
17/11/03 07:37:39 INFO mapreduce.Job:  map 100% reduce 19%
17/11/03 07:37:40 INFO mapreduce.Job:  map 100% reduce 24%
17/11/03 07:37:41 INFO mapreduce.Job:  map 100% reduce 27%
17/11/03 07:37:42 INFO mapreduce.Job:  map 100% reduce 34%
17/11/03 07:37:43 INFO mapreduce.Job:  map 100% reduce 37%
17/11/03 07:37:44 INFO mapreduce.Job:  map 100% reduce 38%
17/11/03 07:37:45 INFO mapreduce.Job:  map 100% reduce 39%
17/11/03 07:37:46 INFO mapreduce.Job:  map 100% reduce 42%
17/11/03 07:37:47 INFO mapreduce.Job:  map 100% reduce 46%
17/11/03 07:37:48 INFO mapreduce.Job:  map 100% reduce 52%
17/11/03 07:37:49 INFO mapreduce.Job:  map 100% reduce 55%
17/11/03 07:37:50 INFO mapreduce.Job:  map 100% reduce 57%
17/11/03 07:37:51 INFO mapreduce.Job:  map 100% reduce 61%
17/11/03 07:37:52 INFO mapreduce.Job:  map 100% reduce 63%
17/11/03 07:37:53 INFO mapreduce.Job:  map 100% reduce 65%
17/11/03 07:37:54 INFO mapreduce.Job:  map 100% reduce 68%
17/11/03 07:37:55 INFO mapreduce.Job:  map 100% reduce 70%
17/11/03 07:37:57 INFO mapreduce.Job:  map 100% reduce 78%
17/11/03 07:37:58 INFO mapreduce.Job:  map 100% reduce 79%
17/11/03 07:37:59 INFO mapreduce.Job:  map 100% reduce 80%
17/11/03 07:38:00 INFO mapreduce.Job:  map 100% reduce 86%
17/11/03 07:38:02 INFO mapreduce.Job:  map 100% reduce 87%
17/11/03 07:38:03 INFO mapreduce.Job:  map 100% reduce 91%
17/11/03 07:38:06 INFO mapreduce.Job:  map 100% reduce 92%
17/11/03 07:38:07 INFO mapreduce.Job:  map 100% reduce 96%
17/11/03 07:38:08 INFO mapreduce.Job:  map 100% reduce 97%
17/11/03 07:38:09 INFO mapreduce.Job:  map 100% reduce 98%
17/11/03 07:38:10 INFO mapreduce.Job:  map 100% reduce 99%
17/11/03 07:38:11 INFO mapreduce.Job:  map 100% reduce 100%
17/11/03 07:38:12 INFO mapreduce.Job: Job job_1509708469036_0001 completed successfully
17/11/03 07:38:12 INFO mapreduce.Job: Counters: 50
        File System Counters
                FILE: Number of bytes read=2910678527
                FILE: Number of bytes written=5783588111
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=6553631212
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=642
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=20
        Job Counters
                Launched map tasks=204
                Launched reduce tasks=10
                Data-local map tasks=194
                Rack-local map tasks=10
                Total time spent by all maps in occupied slots (ms)=1435040
                Total time spent by all reduces in occupied slots (ms)=673132
                Total time spent by all map tasks (ms)=1435040
                Total time spent by all reduce tasks (ms)=673132
                Total vcore-seconds taken by all map tasks=1435040
                Total vcore-seconds taken by all reduce tasks=673132
                Total megabyte-seconds taken by all map tasks=1469480960
                Total megabyte-seconds taken by all reduce tasks=689287168
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Map output bytes=6684672000
                Map output materialized bytes=2846208942
                Input split bytes=31212
                Combine input records=0
                Combine output records=0
                Reduce input groups=65536000
                Reduce shuffle bytes=2846208942
                Reduce input records=65536000
                Reduce output records=65536000
                Spilled Records=131072000
                Shuffled Maps =2040
                Failed Shuffles=0
                Merged Map outputs=2040
                GC time elapsed (ms)=20822
                CPU time spent (ms)=910810
                Physical memory (bytes) snapshot=107325628416
                Virtual memory (bytes) snapshot=338197057536
                Total committed heap usage (bytes)=121025069056
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
17/11/03 07:38:12 INFO terasort.TeraSort: done
```
