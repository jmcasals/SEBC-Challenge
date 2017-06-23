$ hdfs dfs -ls /user
Found 9 items
drwxr-xr-x   - admin  admin               0 2017-06-23 04:23 /user/admin
drwxr-xr-x   - saturn supergroup          0 2017-06-23 04:35 /user/haley
drwxr-xr-x   - hdfs   supergroup          0 2017-06-23 04:23 /user/hdfs
drwxrwxrwx   - mapred hadoop              0 2017-06-23 04:13 /user/history
drwxrwxr-t   - hive   hive                0 2017-06-23 04:14 /user/hive
drwxrwxr-x   - hue    hue                 0 2017-06-23 04:14 /user/hue
drwxrwxr-x   - oozie  oozie               0 2017-06-23 04:14 /user/oozie
drwxr-xr-x   - saturn supergroup          0 2017-06-23 04:32 /user/saturn
drwxr-x--x   - spark  spark               0 2017-06-23 04:13 /user/spark

$curl  -X GET -u admin:admin \http://localhost:7180/api/v14/hosts

{
  "items" : [ {
    "hostId" : "3b5cc641-25f6-47f3-b6ba-825b51b1c0b4",
    "ipAddress" : "172.31.36.93",
    "hostname" : "ip-172-31-36-93.eu-west-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-38-33.eu-west-1.compute.internal:7180/cmf/hostRedirect/3b5cc641-25f6-47f3-b6ba-825b51b1c0b4",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331913728
  }, {
    "hostId" : "f54d35c9-586b-43d1-89cb-ab50ce1e3f4a",
    "ipAddress" : "172.31.38.33",
    "hostname" : "ip-172-31-38-33.eu-west-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-38-33.eu-west-1.compute.internal:7180/cmf/hostRedirect/f54d35c9-586b-43d1-89cb-ab50ce1e3f4a",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331913728
  }, {
    "hostId" : "cac06cbe-4629-4d29-8381-f551fde2f124",
    "ipAddress" : "172.31.39.89",
    "hostname" : "ip-172-31-39-89.eu-west-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-38-33.eu-west-1.compute.internal:7180/cmf/hostRedirect/cac06cbe-4629-4d29-8381-f551fde2f124",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331913728
  }, {
    "hostId" : "8ce3e98c-7d9f-4397-ad3b-356924530b6b",
    "ipAddress" : "172.31.43.159",
    "hostname" : "ip-172-31-43-159.eu-west-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-38-33.eu-west-1.compute.internal:7180/cmf/hostRedirect/8ce3e98c-7d9f-4397-ad3b-356924530b6b",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331913728
  }, {
    "hostId" : "c8f20b40-0d6c-48fe-8296-5c716b10623b",
    "ipAddress" : "172.31.45.115",
    "hostname" : "ip-172-31-45-115.eu-west-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-38-33.eu-west-1.compute.internal:7180/cmf/hostRedirect/c8f20b40-0d6c-48fe-8296-5c716b10623b",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15331913728
  } ]



$curl  -X GET -u admin:admin \http://localhost:7180/api/v6/clusters/jmcasals/services

{
  "items" : [ {
    "name" : "hive",
    "type" : "HIVE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-33.eu-west-1.compute.internal:7180/cmf/serviceRedirect/hive",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HIVE_HIVEMETASTORES_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HIVE_HIVESERVER2S_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hive"
  }, {
    "name" : "zookeeper",
    "type" : "ZOOKEEPER",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-33.eu-west-1.compute.internal:7180/cmf/serviceRedirect/zookeeper",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "ZOOKEEPER_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "ZooKeeper"
  }, {
    "name" : "hue",
    "type" : "HUE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-33.eu-west-1.compute.internal:7180/cmf/serviceRedirect/hue",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HUE_HUE_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hue"
  }, {
    "name" : "oozie",
    "type" : "OOZIE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-33.eu-west-1.compute.internal:7180/cmf/serviceRedirect/oozie",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Oozie"
  }, {
    "name" : "yarn",
    "type" : "YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-33.eu-west-1.compute.internal:7180/cmf/serviceRedirect/yarn",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "YARN_JOBHISTORY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_NODE_MANAGERS_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_RESOURCEMANAGERS_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_USAGE_AGGREGATION_HEALTH",
      "summary" : "DISABLED"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "YARN (MR2 Included)"
  }, {
    "name" : "spark_on_yarn",
    "type" : "SPARK_ON_YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-33.eu-west-1.compute.internal:7180/cmf/serviceRedirect/spark_on_yarn",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Spark"
  }, {
    "name" : "hdfs",
    "type" : "HDFS",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-38-33.eu-west-1.compute.internal:7180/cmf/serviceRedirect/hdfs",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_DATA_NODES_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_FREE_SPACE_REMAINING",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_HA_NAMENODE_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_MISSING_BLOCKS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HDFS"
  } ]
}
