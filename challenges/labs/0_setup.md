

cloud provider AWS
RHEL-7.2_HVM-20161025-x86_64-1-Hourly2-GP2 - ami-7def1712
50 GB storage each

ec2-18-195-23-240.eu-central-1.compute.amazonaws.com  18.195.23.240;
ec2-52-59-2-173.eu-central-1.compute.amazonaws.com    52.59.2.173;
ec2-18-195-24-160.eu-central-1.compute.amazonaws.com  18.195.24.160;
ec2-35-158-179-163.eu-central-1.compute.amazonaws.com 35.158.179.163;
ec2-18-194-116-159.eu-central-1.compute.amazonaws.com 18.194.116.159;

[root@ip-172-31-42-252 ec2-user]# yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
repo id                                          repo name           status
rhui-REGION-client-config-server-7/x86_64        Red Hat Update Infr      5
rhui-REGION-rhel-server-releases/7Server/x86_64  Red Hat Enterprise  17,471
rhui-REGION-rhel-server-rh-common/7Server/x86_64 Red Hat Enterprise     228
repolist: 17,704


[root@ip-172-31-35-238 ec2-user]# df -k
Filesystem     1K-blocks    Used Available Use% Mounted on
/dev/xvda2      52416492 1227568  51188924   3% /
devtmpfs         7599292       0   7599292   0% /dev
tmpfs            7486480       0   7486480   0% /dev/shm
tmpfs            7486480   16628   7469852   1% /run
tmpfs            7486480       0   7486480   0% /sys/fs/cgroup
tmpfs            1497296       0   1497296   0% /run/user/1000
