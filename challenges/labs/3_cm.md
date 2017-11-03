[root@ip-172-31-45-9 ec2-user]# hdfs dfs -ls /user
Found 9 items
drwxr-xr-x   - admin    admin               0 2017-11-03 06:14 /user/admin
drwxr-xr-x   - frankola frankola            0 2017-11-03 06:15 /user/frankola
drwxr-xr-x   - hdfs     supergroup          0 2017-11-03 06:14 /user/hdfs
drwxrwxrwx   - mapred   hadoop              0 2017-11-03 06:09 /user/history
drwxrwxr-t   - hive     hive                0 2017-11-03 06:11 /user/hive
drwxrwxr-x   - hue      hue                 0 2017-11-03 06:11 /user/hue
drwxrwxr-x   - oozie    oozie               0 2017-11-03 06:11 /user/oozie
drwxr-xr-x   - reilly   reilly              0 2017-11-03 06:15 /user/reilly
drwxr-x--x   - spark    spark               0 2017-11-03 06:10 /user/spark

[root@ip-172-31-45-9 ec2-user]# curl -u admin:admin 'http://52.59.2.173:7180/api/v14/hosts'
{
  "items" : [ {
    "hostId" : "97becf4b-d771-4a73-9c9e-a74eadce920a",
    "ipAddress" : "172.31.35.238",
    "hostname" : "ip-172-31-35-238.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/hostRedirect/97becf4b-d771-4a73-9c9e-a74eadce920a",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332311040
  }, {
    "hostId" : "615bdc90-8ccf-4a0f-a8e9-ac5caacf23ba",
    "ipAddress" : "172.31.42.252",
    "hostname" : "ip-172-31-42-252.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/hostRedirect/615bdc90-8ccf-4a0f-a8e9-ac5caacf23ba",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332311040
  }, {
    "hostId" : "1decd012-f3d6-4eb3-b02e-1af0ddcf3e69",
    "ipAddress" : "172.31.44.217",
    "hostname" : "ip-172-31-44-217.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/hostRedirect/1decd012-f3d6-4eb3-b02e-1af0ddcf3e69",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332311040
  }, {
    "hostId" : "e1923cf5-a4c2-4f0a-908c-5c35a11a5649",
    "ipAddress" : "172.31.45.9",
    "hostname" : "ip-172-31-45-9.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/hostRedirect/e1923cf5-a4c2-4f0a-908c-5c35a11a5649",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332311040
  }, {
    "hostId" : "181db817-4fbd-4889-acf8-264a227f5cbc",
    "ipAddress" : "172.31.46.99",
    "hostname" : "ip-172-31-46-99.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/hostRedirect/181db817-4fbd-4889-acf8-264a227f5cbc",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332311040
  } ]

[root@ip-172-31-45-9 ec2-user]# curl -u admin:admin 'http://52.59.2.173:7180/api/v11/clusters/abarbi69/services'
{
  "items" : [ {
    "name" : "hive",
    "type" : "HIVE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hive",
    "roleInstancesUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hive/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HIVE_HIVEMETASTORES_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HIVE_HIVESERVER2S_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hive",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "zookeeper",
    "type" : "ZOOKEEPER",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/zookeeper",
    "roleInstancesUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/zookeeper/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "ZOOKEEPER_CANARY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "ZooKeeper",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hue",
    "type" : "HUE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hue",
    "roleInstancesUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hue/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HUE_HUE_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hue",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "oozie",
    "type" : "OOZIE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/oozie",
    "roleInstancesUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/oozie/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Oozie",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "yarn",
    "type" : "YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/yarn",
    "roleInstancesUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/yarn/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "YARN_JOBHISTORY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "YARN_NODE_MANAGERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "YARN_RESOURCEMANAGERS_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "YARN_USAGE_AGGREGATION_HEALTH",
      "summary" : "DISABLED",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "YARN (MR2 Included)",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "spark_on_yarn",
    "type" : "SPARK_ON_YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/spark_on_yarn",
    "roleInstancesUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/spark_on_yarn/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Spark",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hdfs",
    "type" : "HDFS",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hdfs",
    "roleInstancesUrl" : "http://ip-172-31-45-9.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hdfs/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_CANARY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_DATA_NODES_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_FREE_SPACE_REMAINING",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_HA_NAMENODE_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_MISSING_BLOCKS",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HDFS",
    "entityStatus" : "GOOD_HEALTH"
  } ]

[root@ip-172-31-45-9 ec2-user]# curl -u admin:admin "http://52.59.2.173:7180/api/v9/cm/deployment"
{
  "timestamp" : "2017-11-03T10:24:01.909Z",
  "clusters" : [ {
    "name" : "cluster",
    "displayName" : "abarbi69",
    "version" : "CDH5",
    "fullVersion" : "5.8.5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-35-238.eu-central-1.compute.internal"
        }, {
          "name" : "hive_metastore_database_name",
          "value" : "hive"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_password"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "spark_on_yarn_service",
          "value" : "spark_on_yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-04d6b4a64945c8a21168427a63211e8b",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "615bdc90-8ccf-4a0f-a8e9-ac5caacf23ba"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-11d18c39656f44680d74907107c30883",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "1decd012-f3d6-4eb3-b02e-1af0ddcf3e69"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-6b8393aefce6d34bced2115b693b67e1",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "97becf4b-d771-4a73-9c9e-a74eadce920a"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-788edb71483826ffa04785f443dc8265",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "e1923cf5-a4c2-4f0a-908c-5c35a11a5649"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-ce2d03b352948c5789a7d193471a0a4d",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "181db817-4fbd-4889-acf8-264a227f5cbc"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-HIVEMETASTORE-6b8393aefce6d34bced2115b693b67e1",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "97becf4b-d771-4a73-9c9e-a74eadce920a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ttm2116lpsi194omxuvxf13b"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVEMETASTORE-BASE"
        }
      }, {
        "name" : "hive-HIVESERVER2-04d6b4a64945c8a21168427a63211e8b",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "615bdc90-8ccf-4a0f-a8e9-ac5caacf23ba"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "edttvbe1my3222v6c0hun48w9"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVESERVER2-BASE"
        }
      } ],
      "displayName" : "Hive",
      "roleConfigGroups" : [ {
        "name" : "hive-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-BASE",
        "displayName" : "Hive Metastore Server Default Group",
        "roleType" : "HIVEMETASTORE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "1233125376"
          }, {
            "name" : "hive_metastore_server_max_message_size",
            "value" : "123312537"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-BASE",
        "displayName" : "HiveServer2 Default Group",
        "roleType" : "HIVESERVER2",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "1181745152"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "1124807475"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "189"
          } ]
        }
      }, {
        "name" : "hive-WEBHCAT-BASE",
        "displayName" : "WebHCat Server Default Group",
        "roleType" : "WEBHCAT",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ ]
        }
      } ],
      "replicationSchedules" : [ ]
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-04d6b4a64945c8a21168427a63211e8b",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "615bdc90-8ccf-4a0f-a8e9-ac5caacf23ba"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bsfjrbole378lz9kuvbcc7fyb"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      } ],
      "displayName" : "ZooKeeper",
      "roleConfigGroups" : [ {
        "name" : "zookeeper-SERVER-BASE",
        "displayName" : "Server Default Group",
        "roleType" : "SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "zookeeper"
        },
        "config" : {
          "items" : [ ]
        }
      } ]
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-35-238.eu-central-1.compute.internal"
        }, {
          "name" : "database_password",
          "value" : "hue_password"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-ce2d03b352948c5789a7d193471a0a4d"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-6b8393aefce6d34bced2115b693b67e1",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "97becf4b-d771-4a73-9c9e-a74eadce920a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "94ksjf4dt7rh44c16a20peb8v"
          }, {
            "name" : "secret_key",
            "value" : "AheeEUIN1SRY07J42gfcuW7AqtxaFC"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hue-HUE_SERVER-BASE"
        }
      } ],
      "displayName" : "Hue",
      "roleConfigGroups" : [ {
        "name" : "hue-HUE_LOAD_BALANCER-BASE",
        "displayName" : "Load Balancer Default Group",
        "roleType" : "HUE_LOAD_BALANCER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hue-HUE_SERVER-BASE",
        "displayName" : "Hue Server Default Group",
        "roleType" : "HUE_SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hue-KT_RENEWER-BASE",
        "displayName" : "Kerberos Ticket Renewer Default Group",
        "roleType" : "KT_RENEWER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      } ]
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "spark_on_yarn_service",
          "value" : "spark_on_yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-6b8393aefce6d34bced2115b693b67e1",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "97becf4b-d771-4a73-9c9e-a74eadce920a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9wty5idito6ow8ydrve6k5yym"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "oozie-OOZIE_SERVER-BASE"
        }
      } ],
      "displayName" : "Oozie",
      "roleConfigGroups" : [ {
        "name" : "oozie-OOZIE_SERVER-BASE",
        "displayName" : "Oozie Server Default Group",
        "roleType" : "OOZIE_SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "oozie"
        },
        "config" : {
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-35-238.eu-central-1.compute.internal"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie_password"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          } ]
        }
      } ]
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "FcMtHlbWm0VxC3Lq2SSg6rXxYtNohM"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-ce2d03b352948c5789a7d193471a0a4d",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "181db817-4fbd-4889-acf8-264a227f5cbc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bfm8juvk0gjvp6h53w5lr3f2n"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-JOBHISTORY-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-04d6b4a64945c8a21168427a63211e8b",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "615bdc90-8ccf-4a0f-a8e9-ac5caacf23ba"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bk753q5267qk63qmvwa4m4g54"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-1"
        }
      }, {
        "name" : "yarn-NODEMANAGER-11d18c39656f44680d74907107c30883",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "1decd012-f3d6-4eb3-b02e-1af0ddcf3e69"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bexnu4dmue7u2rhjbrtnxutdu"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-4"
        }
      }, {
        "name" : "yarn-NODEMANAGER-6b8393aefce6d34bced2115b693b67e1",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "97becf4b-d771-4a73-9c9e-a74eadce920a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9vbfuxm100z63vuq0pajyg717"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-788edb71483826ffa04785f443dc8265",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "e1923cf5-a4c2-4f0a-908c-5c35a11a5649"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2pmabv6obam9ii9cajw2a4qle"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-2"
        }
      }, {
        "name" : "yarn-NODEMANAGER-ce2d03b352948c5789a7d193471a0a4d",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "181db817-4fbd-4889-acf8-264a227f5cbc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5tzv0jcx6pt3q7ixlqhsvlwwk"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-3"
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-04d6b4a64945c8a21168427a63211e8b",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "615bdc90-8ccf-4a0f-a8e9-ac5caacf23ba"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "133"
          }, {
            "name" : "role_jceks_password",
            "value" : "2cbl13t1hbb7zb1xh40ha2qnh"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-RESOURCEMANAGER-BASE"
        }
      } ],
      "displayName" : "YARN (MR2 Included)",
      "roleConfigGroups" : [ {
        "name" : "yarn-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "10"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "yarn-JOBHISTORY-BASE",
        "displayName" : "JobHistory Server Default Group",
        "roleType" : "JOBHISTORY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-1",
        "displayName" : "NodeManager Group 1",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "1465"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-2",
        "displayName" : "NodeManager Group 2",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "node_manager_java_heapsize",
            "value" : "1018167296"
          }, {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "1262"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-3",
        "displayName" : "NodeManager Group 3",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "3685"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-4",
        "displayName" : "NodeManager Group 4",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "3852"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-BASE",
        "displayName" : "NodeManager Default Group",
        "roleType" : "NODEMANAGER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "1529"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-BASE",
        "displayName" : "ResourceManager Default Group",
        "roleType" : "RESOURCEMANAGER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "3852"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "4"
          } ]
        }
      } ]
    }, {
      "name" : "spark_on_yarn",
      "type" : "SPARK_ON_YARN",
      "config" : {
        "items" : [ {
          "name" : "yarn_service",
          "value" : "yarn"
        } ]
      },
      "roles" : [ {
        "name" : "spar40365358-SPARK_YARN_HISTORY_SERVER-04d6b4a64945c8a21168427a6",
        "type" : "SPARK_YARN_HISTORY_SERVER",
        "hostRef" : {
          "hostId" : "615bdc90-8ccf-4a0f-a8e9-ac5caacf23ba"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "erhd98xm0qgmevmuybrjo3hc2"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "spark_on_yarn-SPARK_YARN_HISTORY_SERVER-BASE"
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-04d6b4a64945c8a21168427a63211e8b",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "615bdc90-8ccf-4a0f-a8e9-ac5caacf23ba"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "spark_on_yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-11d18c39656f44680d74907107c30883",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "1decd012-f3d6-4eb3-b02e-1af0ddcf3e69"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "spark_on_yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-6b8393aefce6d34bced2115b693b67e1",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "97becf4b-d771-4a73-9c9e-a74eadce920a"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "spark_on_yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-788edb71483826ffa04785f443dc8265",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "e1923cf5-a4c2-4f0a-908c-5c35a11a5649"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "spark_on_yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-ce2d03b352948c5789a7d193471a0a4d",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "181db817-4fbd-4889-acf8-264a227f5cbc"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "spark_on_yarn-GATEWAY-BASE"
        }
      } ],
      "displayName" : "Spark",
      "roleConfigGroups" : [ {
        "name" : "spark_on_yarn-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "spark_on_yarn"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "spark_on_yarn-SPARK_YARN_HISTORY_SERVER-BASE",
        "displayName" : "History Server Default Group",
        "roleType" : "SPARK_YARN_HISTORY_SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "spark_on_yarn"
        },
        "config" : {
          "items" : [ ]
        }
      } ]
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "nZv63551EePFRNyhgsQkqqr2JWQWrb"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "ojg6ES2ww1VEbDvpEHoT8nLF7vWxmU"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "zQGLLs77CHCMPzflQkVxLgYGlP1O8Y"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-11d18c39656f44680d74907107c30883",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "1decd012-f3d6-4eb3-b02e-1af0ddcf3e69"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-BALANCER-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-04d6b4a64945c8a21168427a63211e8b",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "615bdc90-8ccf-4a0f-a8e9-ac5caacf23ba"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "axr92ee9uyea141ovy1x3yfhi"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-4"
        }
      }, {
        "name" : "hdfs-DATANODE-11d18c39656f44680d74907107c30883",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "1decd012-f3d6-4eb3-b02e-1af0ddcf3e69"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3a3rgh072f3ltt6uxgmclf5pd"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-2"
        }
      }, {
        "name" : "hdfs-DATANODE-6b8393aefce6d34bced2115b693b67e1",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "97becf4b-d771-4a73-9c9e-a74eadce920a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "10gp6xk39f5jcxhmbxat3do4b"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-3"
        }
      }, {
        "name" : "hdfs-DATANODE-788edb71483826ffa04785f443dc8265",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "e1923cf5-a4c2-4f0a-908c-5c35a11a5649"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "84c5xaixnb5ku7jep0u7hazld"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-ce2d03b352948c5789a7d193471a0a4d",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "181db817-4fbd-4889-acf8-264a227f5cbc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "272f2pbz1w788nxwakk0ywkc0"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-1"
        }
      }, {
        "name" : "hdfs-HTTPFS-ce2d03b352948c5789a7d193471a0a4d",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "181db817-4fbd-4889-acf8-264a227f5cbc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "f14x59z7tm9q9dkm55pguh5qr"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-HTTPFS-BASE"
        }
      }, {
        "name" : "hdfs-NAMENODE-6b8393aefce6d34bced2115b693b67e1",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "97becf4b-d771-4a73-9c9e-a74eadce920a"
        },
        "config" : {
          "items" : [ {
            "name" : "namenode_id",
            "value" : "142"
          }, {
            "name" : "role_jceks_password",
            "value" : "5a2b15r6cqgqpvzcwmwi9etf1"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-NAMENODE-BASE"
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-04d6b4a64945c8a21168427a63211e8b",
        "type" : "SECONDARYNAMENODE",
        "hostRef" : {
          "hostId" : "615bdc90-8ccf-4a0f-a8e9-ac5caacf23ba"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "a41lqxj33xwwoph79b7qy1ttw"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-SECONDARYNAMENODE-BASE"
        }
      } ],
      "displayName" : "HDFS",
      "roleConfigGroups" : [ {
        "name" : "hdfs-BALANCER-BASE",
        "displayName" : "Balancer Default Group",
        "roleType" : "BALANCER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-1",
        "displayName" : "DataNode Group 1",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "3864002560"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-2",
        "displayName" : "DataNode Group 2",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4039114752"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-3",
        "displayName" : "DataNode Group 3",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "1603272704"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-4",
        "displayName" : "DataNode Group 4",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "1536163840"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-BASE",
        "displayName" : "DataNode Default Group",
        "roleType" : "DATANODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1018167296"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "1323302912"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-BASE",
        "displayName" : "Failover Controller Default Group",
        "roleType" : "FAILOVERCONTROLLER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-BASE",
        "displayName" : "HttpFS Default Group",
        "roleType" : "HTTPFS",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-BASE",
        "displayName" : "JournalNode Default Group",
        "roleType" : "JOURNALNODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-NAMENODE-BASE",
        "displayName" : "NameNode Default Group",
        "roleType" : "NAMENODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_handler_count",
            "value" : "32"
          }, {
            "name" : "dfs_namenode_service_handler_count",
            "value" : "32"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "1181745152"
          } ]
        }
      }, {
        "name" : "hdfs-NFSGATEWAY-BASE",
        "displayName" : "NFS Gateway Default Group",
        "roleType" : "NFSGATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-BASE",
        "displayName" : "SecondaryNameNode Default Group",
        "roleType" : "SECONDARYNAMENODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "1181745152"
          } ]
        }
      } ],
      "replicationSchedules" : [ ],
      "snapshotPolicies" : [ ]
    } ],
    "parcels" : [ {
      "product" : "CDH",
      "version" : "5.8.5-1.cdh5.8.5.p0.5",
      "stage" : "DISTRIBUTED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    }, {
      "product" : "CDH",
      "version" : "5.8.5-1.cdh5.8.5.p0.5",
      "stage" : "ACTIVATED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "97becf4b-d771-4a73-9c9e-a74eadce920a",
    "ipAddress" : "172.31.35.238",
    "hostname" : "ip-172-31-35-238.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "615bdc90-8ccf-4a0f-a8e9-ac5caacf23ba",
    "ipAddress" : "172.31.42.252",
    "hostname" : "ip-172-31-42-252.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "1decd012-f3d6-4eb3-b02e-1af0ddcf3e69",
    "ipAddress" : "172.31.44.217",
    "hostname" : "ip-172-31-44-217.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "e1923cf5-a4c2-4f0a-908c-5c35a11a5649",
    "ipAddress" : "172.31.45.9",
    "hostname" : "ip-172-31-45-9.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "181db817-4fbd-4889-acf8-264a227f5cbc",
    "ipAddress" : "172.31.46.99",
    "hostname" : "ip-172-31-46-99.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-788edb71483826ffa04785f443dc8265",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "8c1adbc827212d99c0dd5cea9bfbc60caf6f92fc201dfacf4071b2dbf74d58bc",
    "pwSalt" : 837289656202807380,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-788edb71483826ffa04785f443dc8265",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "6c87a1b7c7057daba41393019a651092bc2f08195f5cc174d4f1927fea6f3b6c",
    "pwSalt" : -1684935710164225304,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-6b8393aefce6d34bced2115b693b67e1",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "05a6f7e8f8e13e23340665dc4d2630c7a2c54cb6bf1549128f8c2631957e5c7f",
    "pwSalt" : 4842455834136318342,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-788edb71483826ffa04785f443dc8265",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "28c19bd92290976ea5359d9ebd2b9eadfa5473444d9b1feaa9fbc0480cf6b503",
    "pwSalt" : 8209709387312401330,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "39772a4d01e84148eec4420833f73abdd81111551f71fe0ad97f328be360b894",
    "pwSalt" : 7387601257485033196,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.11.2",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170811-0014",
    "gitHash" : "3c3ea33a12076fb83a8f11c4452c52fac685d01b",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-788edb71483826ffa04785f443dc8265",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "e1923cf5-a4c2-4f0a-908c-5c35a11a5649"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "dlpeek3h7l1sblc43pbnme5q4"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-ALERTPUBLISHER-BASE"
      }
    }, {
      "name" : "mgmt-EVENTSERVER-788edb71483826ffa04785f443dc8265",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "e1923cf5-a4c2-4f0a-908c-5c35a11a5649"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "6vb6869ez128xmtqvfleeix33"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-EVENTSERVER-BASE"
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-788edb71483826ffa04785f443dc8265",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "e1923cf5-a4c2-4f0a-908c-5c35a11a5649"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "crkuvmn9hhur9a3t060get5s6"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-HOSTMONITOR-BASE"
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-6b8393aefce6d34bced2115b693b67e1",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "97becf4b-d771-4a73-9c9e-a74eadce920a"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "3vcrmz2541by9ojgpygzq5bkt"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-REPORTSMANAGER-BASE"
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-788edb71483826ffa04785f443dc8265",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "e1923cf5-a4c2-4f0a-908c-5c35a11a5649"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "60a6wutr37wpebl1keh6r544m"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-SERVICEMONITOR-BASE"
      }
    } ],
    "displayName" : "Cloudera Management Service",
    "roleConfigGroups" : [ {
      "name" : "mgmt-ACTIVITYMONITOR-BASE",
      "displayName" : "Activity Monitor Default Group",
      "roleType" : "ACTIVITYMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-ALERTPUBLISHER-BASE",
      "displayName" : "Alert Publisher Default Group",
      "roleType" : "ALERTPUBLISHER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-BASE",
      "displayName" : "Event Server Default Group",
      "roleType" : "EVENTSERVER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "1018167296"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-BASE",
      "displayName" : "Host Monitor Default Group",
      "roleType" : "HOSTMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "1018167296"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1323302912"
        } ]
      }
    }, {
      "name" : "mgmt-NAVIGATOR-BASE",
      "displayName" : "Navigator Audit Server Default Group",
      "roleType" : "NAVIGATOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-NAVIGATORMETASERVER-BASE",
      "displayName" : "Navigator Metadata Server Default Group",
      "roleType" : "NAVIGATORMETASERVER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-BASE",
      "displayName" : "Reports Manager Default Group",
      "roleType" : "REPORTSMANAGER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-35-238.eu-central-1.compute.internal"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_password"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-BASE",
      "displayName" : "Service Monitor Default Group",
      "roleType" : "SERVICEMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "1018167296"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1323302912"
        } ]
      }
    }, {
      "name" : "mgmt-TELEMETRYPUBLISHER-BASE",
      "displayName" : "Telemetry Publisher Default Group",
      "roleType" : "TELEMETRYPUBLISHER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    } ]
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/23/2012 5:40"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh5/parcels/5.8,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,http://archive.cloudera.com/kudu/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  },
  "allHostsConfig" : {
    "items" : [ ]
  },
  "peers" : [ ],
  "hostTemplates" : {
    "items" : [ ]
  }


 beeline -u jdbc:hive2://18.194.116.159:10000
scan complete in 2ms
Connecting to jdbc:hive2://18.194.116.159:10000
Connected to: Apache Hive (version 1.1.0-cdh5.8.5)
Driver: Hive JDBC (version 1.1.0-cdh5.8.5)
Transaction isolation: TRANSACTION_REPEATABLE_READ
Beeline version 1.1.0-cdh5.8.5 by Apache Hive
0: jdbc:hive2://18.194.116.159:10000> show tables;
INFO  : Compiling command(queryId=hive_20171103062929_4552d272-ddda-4a8c-94d8-694361554700): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20171103062929_4552d272-ddda-4a8c-94d8-694361554700); Time taken: 0.006 seconds
INFO  : Executing command(queryId=hive_20171103062929_4552d272-ddda-4a8c-94d8-694361554700): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171103062929_4552d272-ddda-4a8c-94d8-694361554700); Time taken: 0.036 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.127 seconds)
0: jdbc:hive2://18.194.116.159:10000>
