time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -Ddfs.block.size=33554432 -Dmapreduce.job.maps=12 -Dmapreduce.map.memory.mb=1024 65536000 /user/reilly/tgen

[reilly@ip-172-31-45-9 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -Ddfs.block.size=33554432 -Dmapreduce.job.maps=12 -Dmapreduce.map.memory.mb=1024 65536000 /user/reilly/tgen
17/11/03 06:33:16 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-42-252.eu-central-1.compute.internal/172.31.42.252:8032
17/11/03 06:33:16 INFO terasort.TeraSort: Generating 65536000 using 12
17/11/03 06:33:16 INFO mapreduce.JobSubmitter: number of splits:12
17/11/03 06:33:16 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/11/03 06:33:17 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1509703778642_0001
17/11/03 06:33:17 INFO impl.YarnClientImpl: Submitted application application_1509703778642_0001
17/11/03 06:33:17 INFO mapreduce.Job: The url to track the job: http://ip-172-31-42-252.eu-central-1.compute.internal:8088/proxy/application_1509703778642_0001/
17/11/03 06:33:17 INFO mapreduce.Job: Running job: job_1509703778642_0001
17/11/03 06:33:24 INFO mapreduce.Job: Job job_1509703778642_0001 running in uber mode : false
17/11/03 06:33:24 INFO mapreduce.Job:  map 0% reduce 0%
17/11/03 06:33:36 INFO mapreduce.Job:  map 4% reduce 0%
17/11/03 06:33:37 INFO mapreduce.Job:  map 18% reduce 0%
17/11/03 06:33:39 INFO mapreduce.Job:  map 21% reduce 0%
17/11/03 06:33:40 INFO mapreduce.Job:  map 27% reduce 0%
17/11/03 06:33:43 INFO mapreduce.Job:  map 28% reduce 0%
17/11/03 06:33:46 INFO mapreduce.Job:  map 30% reduce 0%
17/11/03 06:33:48 INFO mapreduce.Job:  map 31% reduce 0%
17/11/03 06:33:49 INFO mapreduce.Job:  map 32% reduce 0%
17/11/03 06:33:54 INFO mapreduce.Job:  map 33% reduce 0%
17/11/03 06:33:57 INFO mapreduce.Job:  map 35% reduce 0%
17/11/03 06:33:58 INFO mapreduce.Job:  map 37% reduce 0%
17/11/03 06:34:00 INFO mapreduce.Job:  map 38% reduce 0%
17/11/03 06:34:01 INFO mapreduce.Job:  map 43% reduce 0%
17/11/03 06:34:03 INFO mapreduce.Job:  map 45% reduce 0%
17/11/03 06:34:04 INFO mapreduce.Job:  map 54% reduce 0%
17/11/03 06:34:06 INFO mapreduce.Job:  map 55% reduce 0%
17/11/03 06:34:07 INFO mapreduce.Job:  map 58% reduce 0%
17/11/03 06:34:10 INFO mapreduce.Job:  map 59% reduce 0%
17/11/03 06:34:15 INFO mapreduce.Job:  map 60% reduce 0%
17/11/03 06:34:21 INFO mapreduce.Job:  map 62% reduce 0%
17/11/03 06:34:24 INFO mapreduce.Job:  map 63% reduce 0%
17/11/03 06:34:27 INFO mapreduce.Job:  map 65% reduce 0%
17/11/03 06:34:28 INFO mapreduce.Job:  map 66% reduce 0%
17/11/03 06:34:33 INFO mapreduce.Job:  map 68% reduce 0%
17/11/03 06:34:34 INFO mapreduce.Job:  map 69% reduce 0%
17/11/03 06:34:36 INFO mapreduce.Job:  map 71% reduce 0%
17/11/03 06:34:40 INFO mapreduce.Job:  map 72% reduce 0%
17/11/03 06:34:42 INFO mapreduce.Job:  map 76% reduce 0%
17/11/03 06:34:44 INFO mapreduce.Job:  map 78% reduce 0%
17/11/03 06:34:45 INFO mapreduce.Job:  map 80% reduce 0%
17/11/03 06:34:51 INFO mapreduce.Job:  map 83% reduce 0%
17/11/03 06:34:53 INFO mapreduce.Job:  map 84% reduce 0%
17/11/03 06:35:02 INFO mapreduce.Job:  map 85% reduce 0%
17/11/03 06:35:03 INFO mapreduce.Job:  map 86% reduce 0%
17/11/03 06:35:08 INFO mapreduce.Job:  map 88% reduce 0%
17/11/03 06:35:09 INFO mapreduce.Job:  map 95% reduce 0%
17/11/03 06:35:12 INFO mapreduce.Job:  map 96% reduce 0%
17/11/03 06:35:14 INFO mapreduce.Job:  map 98% reduce 0%
17/11/03 06:35:15 INFO mapreduce.Job:  map 99% reduce 0%
17/11/03 06:35:18 INFO mapreduce.Job:  map 100% reduce 0%
17/11/03 06:35:19 INFO mapreduce.Job: Job job_1509703778642_0001 completed successfully
17/11/03 06:35:19 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=1469846
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
                Total time spent by all maps in occupied slots (ms)=700034
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=700034
                Total vcore-seconds taken by all map tasks=700034
                Total megabyte-seconds taken by all map tasks=716834816
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=1025
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=1738
                CPU time spent (ms)=143460
                Physical memory (bytes) snapshot=4169809920
                Virtual memory (bytes) snapshot=18963656704
                Total committed heap usage (bytes)=4411883520
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000

real    2m5.988s
user    0m5.808s
sys     0m0.261s



[reilly@ip-172-31-45-9 ~]$ hdfs dfs -ls /user/reilly/tgen
Found 13 items
-rw-r--r--   3 reilly reilly          0 2017-11-03 06:35 /user/reilly/tgen/_SUCCESS
-rw-r--r--   3 reilly reilly  546133400 2017-11-03 06:34 /user/reilly/tgen/part-m-00000
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:34 /user/reilly/tgen/part-m-00001
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:34 /user/reilly/tgen/part-m-00002
-rw-r--r--   3 reilly reilly  546133400 2017-11-03 06:34 /user/reilly/tgen/part-m-00003
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:34 /user/reilly/tgen/part-m-00004
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:34 /user/reilly/tgen/part-m-00005
-rw-r--r--   3 reilly reilly  546133400 2017-11-03 06:34 /user/reilly/tgen/part-m-00006
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:34 /user/reilly/tgen/part-m-00007
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:35 /user/reilly/tgen/part-m-00008
-rw-r--r--   3 reilly reilly  546133400 2017-11-03 06:35 /user/reilly/tgen/part-m-00009
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:35 /user/reilly/tgen/part-m-00010
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:35 /user/reilly/tgen/part-m-00011

[reilly@ip-172-31-45-9 ~]$ hadoop fsck -blocks /user/reilly/tgen
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.

Connecting to namenode via http://ip-172-31-35-238.eu-central-1.compute.internal:50070
FSCK started by reilly (auth:SIMPLE) from /172.31.45.9 for path /user/reilly/tgen at Fri Nov 03 06:37:27 EDT 2017
.............Status: HEALTHY
 Total size:    6553600000 B
 Total dirs:    1
 Total files:   13
 Total symlinks:                0
 Total blocks (validated):      204 (avg. block size 32125490 B)
 Minimally replicated blocks:   204 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          5
 Number of racks:               1
FSCK ended at Fri Nov 03 06:37:27 EDT 2017 in 10 milliseconds


The filesystem under path '/user/reilly/tgen' is HEALTHY

