<!-- CSS work goes here for the time being -->
<!-- set a:link text-decoration to none -->
<!-- set a:hover text-decoration to underline -->
<!-- http://forums.markdownpad.com/discussion/143/include-pdf-pagebreak-instructions-in-markdown/p1 -->

---
<div style="page-break-after: always;"></div>

# <center> Challenges - June 23, 2017 - Retake edition

* Overview
  * Build a CM-managed CDH cluster and secure it
* Place your work in the `challenges/labs` folder
  * All text files require  Markdown (`.md`) extension and formatting
  * All screenshots must be in PNG format
  * You will create the files needed for each submission
* You can consult with each other and research online
  * Submit only your own work!
* Update your GitHub repo often -- don't wait until the end!
* If you break your cluster, or your cluster breaks you:
  * Tell an instructor (`mfernest`)
  * Review the work you have pushed to GitHub
  * Create a new Issue to describe what you think happened

---
<div style="page-break-after: always;"></div>

## <center> Challenge Setup

* Create the Issue `Challenges Setup`
* Make sure `mfernest` is a Collaborator
* Assign the Issue to yourself and label it `started`
* In the file `challenges/labs/0_setup.md`:
  * List the cloud provider you are using (AWS, GCE, Azure, other)
  * List your instances by their IP address and DNS name
  * List the Linux release you are using 
  * List the file system capacity for the first node 
  * List the command and output for `yum repolist enabled` 
* Add the following Linux accounts to all nodes
  * User `saturn` with a UID of `2800`
  * User `haley` with a UID of `2900`
  * Create the group `comets` and add `haley` to it
  * Create the group `planets` and add `saturn` to it
* List the `/etc/passwd` entries for `saturn` and `haley` 
  * Not the entire file!
* List the `/etc/group` entries for `comets` and `planets` 
  * Not the entire file!
* Push these updates to your GitHub repo
* Label your Issue `review` 
* Assign the Issue to the instructor

---
<div style="page-break-after: always;"></div>

## <center> Challenge 1: Install a MySQL server

* Create the Issue `Install MySQL` if you are using RHEL/Centos 6.x
  * Name the Issue `Install MariaDB` for RHEL/CentOS 7.x
* Assign the Issue to yourself and label it `started`
* Install a MySQL 5.6 or MariaDB 5.5 server on the first node listed in `0_setup.md`
  * You must a YUM repository to install the package
  * Copy the repo configuration you use to `challenges/labs/1_my-database-server.repo.md`
* On all cluster nodes
  * Install the appropriate client package and JDBC connector jar
* Start the database service and create these databases
  * `scm`
  * `rman`
  * `hive`
  * `oozie`
  * `hue`
  * `sentry`
* Record the following data in `challenges/labs/1_db-server.md`
  * The command and output to show the hostname for your database server 
  * The command and output to report the database server version
  * The command and output to list the databases in the server
* Push this work to your GitHub repo
* Label the Issue `review` and assign it to the instructor

---
<div style="page-break-after: always;"></div>

## <center> Challenge 2: Install Cloudera Manager 5.10

* Create the Issue `Install CM`
* Assign yourself to the Issue and label it `started`
* Install Cloudera Manager on the second node listed in `0_setup.md`
* List the command and output for `ls /etc/yum.repos.d` in `challenges/labs/2_cm.md`
  * Copy `cloudera-manager.repo` to `challenges/labs/2_cloudera-manager.repo.md`
* Connect Cloudera Manager Server to its database
  * Use the `scm_prepare_database.sh` script to create the `db.properties` file 
    * List the full command and result in `2_cm.md`
* Start the Cloudera Manager server. In `challenges/labs/2_db.properties.md` add:
  * The first line of the server log
  * The line(s) that contain the phrase "Started Jetty server"
  * The content of the `db.properties` file 
* Push these changes to your GitHub repo and label the Issue 'review`
* Assign the issue to the instructor

---
<div style="page-break-after: always;"></div>

## <center> Challenge 3 - Install CDH 5.9

* Create the Issue `Install CDH`
* Assign the issue to yourself and label it `started`
* Deploy Coreset services + Spark 1.6
  * Rename your cluster after your GitHub handle
* Create user directories in HDFS for `saturn` and `haley`
* Add the following to `3_cm.md`:
    * The command and output for `hdfs dfs -ls /user`
    * The command and output from the CM API call `../api/v14/hosts` 
    * The command and output from the CM API call `../api/v6/clusters/<githubName>/services`
* Login to Hue and install the sample data for Hive
    * Copy a HUE screen that lists the Hive tables to `challenges/labs/3_hue_hive.png`
* Push this work to your GitHub repo and label the Issue `review`
* Assign the issue to the instructor

---
<div style="page-break-after: always;"></div>

## <center> Challenge 4 - HDFS Testing

* Create the Issue `Test HDFS`
* Assign the issue to yourself and label it `started`
* As user `saturn`, use `teragen` to generate a 65,536,000-record dataset
  * Write the output to 12 files 
  * Set the block size for this file to 32 MB
  * Set the mapper container size to 1 GiB
  * Name the target directory `tgen`
  * Use the `time` command to capture job duration
* Put the following in `challenges/labs/4_teragen.md`
  * The full `teragen` command and output 
  * The result of the `time` command
  * The command and output of `hdfs dfs -ls /user/saturn/tgen`
* Push this work to your GitHub repo and label the Issue `review`
* Assign the issue to the instructor

---
<div style="page-break-after: always;"></div>

## <center> Challenge 5 - Kerberize the cluster

* Create the Issue `Kerberize cluster`
* Assign the issue to yourself and label it `started`
* Install an MIT KDC on the second node in your cluster
  * Name your realm after your GitHub handle
  * Use `PA` as a suffix
  * For example: `RSTOKES.PA`
* Create Kerberos principals for `saturn`, `haley`, and `cloudera-scm`
  * Grant `cloudera-scm` the privileges needed to create principals and generate keytabs
* Enable Kerberos for the cluster
* Run the `terasort` program as `saturn` using the output target `/user/saturn/tsort`
  * Copy the command and full output to `challenges/labs/5_terasort.md`
* Run the Hadoop `pi` program as the user `haley`
  * Copy the command and full output to `challenges/labs/5_pi.md`
*  Copy the configuration files in `/var/kerberos/krb5kdc/` to your repo:
    * Add the prefix `5_` and the suffix `.md` to the original file name
    * Example: `5_kdc.conf.md`
* Push this work to your GitHub repo and label the Issue `review`
* Assign the issue to the instructor

---
<div style="page-break-after: always;"></div>

## <center> Challenge 6 - Upgrade CDH 

* Create the Issue `Upgrade CDH`
  * Label it `started`
* Follow Cloudera's docs for upgrading CDH to the latest release you can
* Capture the CM view of the cluster showing the CDH version in `challenges/labs/6_upgrade.png`
* Label the issue `review`
* Assign the issue to the instructor
* Push all work to your GitHub repo

---
<div style="page-break-after: always;"></div>

## <center> If you finish early, or once time is called:

* Commit any outstanding changes from your repo to GitHub
* Email `mfe@cloudera.com` that you have stopped pushing to your repo
  * You can continue working, if you wish, after sending this note
* Anything else you'd like to say about the class?

---
<div style="page-break-after: always;"></div>
