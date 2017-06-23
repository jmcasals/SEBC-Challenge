Cloud Provider is: AWS (AWS m3xlarge instances)

Instances are:

Name			Public IP	Public DNS		

ClouderaCasals1		52.212.49.52	ec2-52-212-49-52.eu-west-1.compute.amazonaws.com
ClouderaCasals2		52.49.182.75	ec2-52-49-182-75.eu-west-1.compute.amazonaws.com
ClouderaCasals3		52.51.237.231	ec2-52-51-237-231.eu-west-1.compute.amazonaws.com
ClouderaCasals4		54.72.197.46	ec2-54-72-197-46.eu-west-1.compute.amazonaws.com
ClouderaCasals5		54.76.154.127	ec2-54-76-154-127.eu-west-1.compute.amazonaws.com

$cat /proc/version

Linux version 3.10.0-514.21.2.el7.x86_64 (mockbuild@x86-037.build.eng.bos.redhat.com) (gcc version 4.8.5 20150623 (Red Hat 4.8.5-11) (GCC) ) #1 SMP Sun May 28 17:08:21 EDT 2017

$uname -a

Linux ip-172-31-39-89.eu-west-1.compute.internal 3.10.0-514.21.2.el7.x86_64 #1 SMP Sun May 28 17:08:21 EDT 2017 x86_64 x86_64 x86_64 GNU/Linux

$df -h

Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2      1.0T 1001M  1.0T   1% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   17M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000
tmpfs           1.5G     0  1.5G   0% /run/user/0


$yum repolist enabled

Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
rhui-REGION-client-config-server-7                                                                                                            | 2.9 kB  00:00:00
rhui-REGION-rhel-server-releases                                                                                                              | 3.5 kB  00:00:00
rhui-REGION-rhel-server-rh-common                                                                                                             | 3.8 kB  00:00:00
(1/7): rhui-REGION-rhel-server-releases/7Server/x86_64/group                                                                                  | 701 kB  00:00:00
(2/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/group                                                                                 |  104 B  00:00:00
(3/7): rhui-REGION-client-config-server-7/x86_64/primary_db                                                                                   | 5.5 kB  00:00:00
(4/7): rhui-REGION-rhel-server-releases/7Server/x86_64/updateinfo                                                                             | 1.9 MB  00:00:00
(5/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/primary_db                                                                            | 118 kB  00:00:00
(6/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/updateinfo                                                                            |  33 kB  00:00:00
(7/7): rhui-REGION-rhel-server-releases/7Server/x86_64/primary_db                                                                             |  37 MB  00:00:00
repo id                                                                 repo name                                                                              status
rhui-REGION-client-config-server-7/x86_64                               Red Hat Update Infrastructure 2.0 Client Configuration Server 7                             6
rhui-REGION-rhel-server-releases/7Server/x86_64                         Red Hat Enterprise Linux Server 7 (RPMs)                                               14,473
rhui-REGION-rhel-server-rh-common/7Server/x86_64                        Red Hat Enterprise Linux Server 7 RH Common (RPMs)                                        228
repolist: 14,707

$useradd -u 2800 saturn
$useradd -u 2900 haley;

$groupadd comets
$groupadd planets 

$usermod -a -G comets haley 
$usermod -a -G planets saturn					

/etc/passwd -->

saturn:x:2800:2800::/home/saturn:/bin/bash
haley:x:2900:2900::/home/haley:/bin/bash

/etc/group -->

comets:x:2901:haley
planets:x:2902:saturn


