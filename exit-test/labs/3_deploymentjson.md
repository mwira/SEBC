```
json
{
  "timestamp" : "2018-05-18T05:24:30.644Z",
  "clusters" : [ {
    "name" : "cluster",
    "displayName" : "mwira",
    "version" : "CDH5",
    "fullVersion" : "5.11.2",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "items" : [ {
          "name" : "hbase_service",
          "value" : "hbase",
          "sensitive" : false
        }, {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-28-149.ap-southeast-1.compute.internal",
          "sensitive" : false
        }, {
          "name" : "hive_metastore_database_name",
          "value" : "hive",
          "sensitive" : false
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_password",
          "sensitive" : true
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-524a6bb0267206aeda278931f7fa35d0",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-8ce14f518144c26e727f0f850feb32d8",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "56b922af-e8a9-4cca-ad30-070a5e6fc234"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-8efcefbac6705e96fa0a3a6a5d39d3b5",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "21db6b77-9bef-44d8-8220-c8698b39e77e"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-bca810a75dcaff85a56816aa5ee58e03",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "eec0068d-0fc6-4b98-8c5b-c4bc72f44137"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-c0f39c297491608d79332148a985f14d",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2bd2a37f-5107-410b-88d9-22598a68d314"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-HIVEMETASTORE-524a6bb0267206aeda278931f7fa35d0",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9aihvp08wod820672p01rd9c6",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVEMETASTORE-BASE"
        }
      }, {
        "name" : "hive-HIVESERVER2-524a6bb0267206aeda278931f7fa35d0",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "clvbg3ihlyqsjpti0xdbkhhyn",
            "sensitive" : true
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
            "value" : "609222656",
            "sensitive" : false
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
            "value" : "609222656",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "2284375244",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "384",
            "sensitive" : false
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
      "name" : "hbase",
      "type" : "HBASE",
      "config" : {
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs",
          "sensitive" : false
        }, {
          "name" : "rm_dirty",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hbase-MASTER-524a6bb0267206aeda278931f7fa35d0",
        "type" : "MASTER",
        "hostRef" : {
          "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "djel6fc4j6v7zyxmxo6ydnjc9",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hbase-MASTER-BASE"
        }
      }, {
        "name" : "hbase-REGIONSERVER-8ce14f518144c26e727f0f850feb32d8",
        "type" : "REGIONSERVER",
        "hostRef" : {
          "hostId" : "56b922af-e8a9-4cca-ad30-070a5e6fc234"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2z90oknye8w3yswz42sngyho4",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hbase-REGIONSERVER-BASE"
        }
      }, {
        "name" : "hbase-REGIONSERVER-8efcefbac6705e96fa0a3a6a5d39d3b5",
        "type" : "REGIONSERVER",
        "hostRef" : {
          "hostId" : "21db6b77-9bef-44d8-8220-c8698b39e77e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5o3042qjq50qarvvhnl2pt3qb",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hbase-REGIONSERVER-1"
        }
      }, {
        "name" : "hbase-REGIONSERVER-bca810a75dcaff85a56816aa5ee58e03",
        "type" : "REGIONSERVER",
        "hostRef" : {
          "hostId" : "eec0068d-0fc6-4b98-8c5b-c4bc72f44137"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1aqvfnxodg08mumf5p4768ywp",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hbase-REGIONSERVER-1"
        }
      }, {
        "name" : "hbase-REGIONSERVER-c0f39c297491608d79332148a985f14d",
        "type" : "REGIONSERVER",
        "hostRef" : {
          "hostId" : "2bd2a37f-5107-410b-88d9-22598a68d314"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dl3atxqqsaabi4zhcv6drbkjo",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hbase-REGIONSERVER-BASE"
        }
      } ],
      "displayName" : "HBase",
      "roleConfigGroups" : [ {
        "name" : "hbase-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hbase-HBASERESTSERVER-BASE",
        "displayName" : "HBase REST Server Default Group",
        "roleType" : "HBASERESTSERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hbase-HBASETHRIFTSERVER-BASE",
        "displayName" : "HBase Thrift Server Default Group",
        "roleType" : "HBASETHRIFTSERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hbase-MASTER-BASE",
        "displayName" : "Master Default Group",
        "roleType" : "MASTER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ {
            "name" : "hbase_master_java_heapsize",
            "value" : "609222656",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hbase-REGIONSERVER-1",
        "displayName" : "RegionServer Group 1",
        "roleType" : "REGIONSERVER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ {
            "name" : "hbase_regionserver_java_heapsize",
            "value" : "2425356288",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hbase-REGIONSERVER-BASE",
        "displayName" : "RegionServer Default Group",
        "roleType" : "REGIONSERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hbase"
        },
        "config" : {
          "items" : [ {
            "name" : "hbase_regionserver_java_heapsize",
            "value" : "2066743296",
            "sensitive" : false
          } ]
        }
      } ],
      "snapshotPolicies" : [ ]
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-524a6bb0267206aeda278931f7fa35d0",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bmk1zcuoi9fgqezfncup84kcw",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "1",
            "sensitive" : false
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-8ce14f518144c26e727f0f850feb32d8",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "56b922af-e8a9-4cca-ad30-070a5e6fc234"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6detr3imc2188gveki6pft9ye",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "2",
            "sensitive" : false
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-c0f39c297491608d79332148a985f14d",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "2bd2a37f-5107-410b-88d9-22598a68d314"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5utinkh7ncaoxbijavikq3g7a",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "3",
            "sensitive" : false
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
          "items" : [ {
            "name" : "maxSessionTimeout",
            "value" : "60000",
            "sensitive" : false
          }, {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "609222656",
            "sensitive" : false
          } ]
        }
      } ]
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-28-149.ap-southeast-1.compute.internal",
          "sensitive" : false
        }, {
          "name" : "database_password",
          "value" : "huepassword",
          "sensitive" : true
        }, {
          "name" : "database_type",
          "value" : "mysql",
          "sensitive" : false
        }, {
          "name" : "hbase_service",
          "value" : "hbase",
          "sensitive" : false
        }, {
          "name" : "hive_service",
          "value" : "hive",
          "sensitive" : false
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-524a6bb0267206aeda278931f7fa35d0",
          "sensitive" : false
        }, {
          "name" : "oozie_service",
          "value" : "oozie",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-524a6bb0267206aeda278931f7fa35d0",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "atr6nmys77xz3eputteny0kmu",
            "sensitive" : true
          }, {
            "name" : "secret_key",
            "value" : "kgqzWMYLuCWTMJwhz8vYAsGVKc5gbM",
            "sensitive" : true
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
          "value" : "hive",
          "sensitive" : false
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-524a6bb0267206aeda278931f7fa35d0",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "42xis77w36hrfcg1cz69y6pgt",
            "sensitive" : true
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
            "value" : "ip-172-31-28-149.ap-southeast-1.compute.internal",
            "sensitive" : false
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie",
            "sensitive" : true
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql",
            "sensitive" : false
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie",
            "sensitive" : false
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "609222656",
            "sensitive" : false
          } ]
        }
      } ]
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs",
          "sensitive" : false
        }, {
          "name" : "rm_dirty",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "c10cRh0PJBww1YyLeCgvAjkdKlsMKl",
          "sensitive" : true
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-524a6bb0267206aeda278931f7fa35d0",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "deq8wcv6hok6c6kwe5wshd9xd",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-JOBHISTORY-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-8ce14f518144c26e727f0f850feb32d8",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "56b922af-e8a9-4cca-ad30-070a5e6fc234"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8vfn49lee2wb7bgl37kgxdu44",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-8efcefbac6705e96fa0a3a6a5d39d3b5",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "21db6b77-9bef-44d8-8220-c8698b39e77e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3n91jjiowtw0yb9n5ficthwru",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-1"
        }
      }, {
        "name" : "yarn-NODEMANAGER-bca810a75dcaff85a56816aa5ee58e03",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "eec0068d-0fc6-4b98-8c5b-c4bc72f44137"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3e9wlmhhe3i58ezm4wohgdnkg",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-1"
        }
      }, {
        "name" : "yarn-NODEMANAGER-c0f39c297491608d79332148a985f14d",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "2bd2a37f-5107-410b-88d9-22598a68d314"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "d7hhnocc3dxtpbkykn39xkdml",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-BASE"
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-524a6bb0267206aeda278931f7fa35d0",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "63",
            "sensitive" : false
          }, {
            "name" : "role_jceks_password",
            "value" : "44z7cq1fxqpp1keossz2dcjcy",
            "sensitive" : true
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
            "value" : "8",
            "sensitive" : false
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2",
            "sensitive" : false
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
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "609222656",
            "sensitive" : false
          } ]
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
            "value" : "100",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "3007",
            "sensitive" : false
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
            "value" : "100",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "2563",
            "sensitive" : false
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
            "name" : "resource_manager_java_heapsize",
            "value" : "609222656",
            "sensitive" : false
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "3007",
            "sensitive" : false
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "4",
            "sensitive" : false
          } ]
        }
      } ]
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "95uLZsRWcIgoSAQWgNWjU3Xh3gIPk2",
          "sensitive" : true
        }, {
          "name" : "dfs_namenode_acls_enabled",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "xlrmk94zB0bEzUTQSogEqGzVqK3BRP",
          "sensitive" : true
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "hujxIp8j16EmT8ydlM6BneK5vpE5bw",
          "sensitive" : true
        }, {
          "name" : "rm_dirty",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-524a6bb0267206aeda278931f7fa35d0",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-BALANCER-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-8ce14f518144c26e727f0f850feb32d8",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "56b922af-e8a9-4cca-ad30-070a5e6fc234"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "t3pxuu7iujx4nm0iwq3292l5",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-8efcefbac6705e96fa0a3a6a5d39d3b5",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "21db6b77-9bef-44d8-8220-c8698b39e77e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dn1f886h66777omrzz64yybrw",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-1"
        }
      }, {
        "name" : "hdfs-DATANODE-bca810a75dcaff85a56816aa5ee58e03",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "eec0068d-0fc6-4b98-8c5b-c4bc72f44137"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ct83ucg4egf5xvqapmcz95arf",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-1"
        }
      }, {
        "name" : "hdfs-DATANODE-c0f39c297491608d79332148a985f14d",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "2bd2a37f-5107-410b-88d9-22598a68d314"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "41fn31mh37l3h3h77ii54vt2j",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-NAMENODE-524a6bb0267206aeda278931f7fa35d0",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
        },
        "config" : {
          "items" : [ {
            "name" : "namenode_id",
            "value" : "65",
            "sensitive" : false
          }, {
            "name" : "role_jceks_password",
            "value" : "a51z6xp3o5y2zy2fcdl7ugt1b",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-NAMENODE-BASE"
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-524a6bb0267206aeda278931f7fa35d0",
        "type" : "SECONDARYNAMENODE",
        "hostRef" : {
          "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8394a7kpy33504mu2l7tntak9",
            "sensitive" : true
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
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "609222656",
            "sensitive" : false
          } ]
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
            "value" : "/dfs/dn",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367553638",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "3153068032",
            "sensitive" : false
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
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367553638",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "2687500288",
            "sensitive" : false
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
            "value" : "true",
            "sensitive" : false
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
            "value" : "/dfs/nn",
            "sensitive" : false
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022",
            "sensitive" : false
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "609222656",
            "sensitive" : false
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
            "value" : "/dfs/snn",
            "sensitive" : false
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "609222656",
            "sensitive" : false
          } ]
        }
      } ],
      "replicationSchedules" : [ ],
      "snapshotPolicies" : [ ]
    } ],
    "parcels" : [ {
      "product" : "CDH",
      "version" : "5.11.2-1.cdh5.11.2.p0.4",
      "stage" : "DISTRIBUTED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    }, {
      "product" : "CDH",
      "version" : "5.11.2-1.cdh5.11.2.p0.4",
      "stage" : "ACTIVATED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e",
    "ipAddress" : "172.31.16.192",
    "hostname" : "ip-172-31-16-192.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "2bd2a37f-5107-410b-88d9-22598a68d314",
    "ipAddress" : "172.31.16.69",
    "hostname" : "ip-172-31-16-69.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "56b922af-e8a9-4cca-ad30-070a5e6fc234",
    "ipAddress" : "172.31.24.40",
    "hostname" : "ip-172-31-24-40.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "eec0068d-0fc6-4b98-8c5b-c4bc72f44137",
    "ipAddress" : "172.31.28.149",
    "hostname" : "ip-172-31-28-149.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "21db6b77-9bef-44d8-8220-c8698b39e77e",
    "ipAddress" : "172.31.30.24",
    "hostname" : "ip-172-31-30-24.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-524a6bb0267206aeda278931f7fa35d0",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "c02a12b228f056f69c51f8c7332ddc80abb93b127c7335eda88edbaf7fa0c80c",
    "pwSalt" : 6926481304961308196,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-524a6bb0267206aeda278931f7fa35d0",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "6bf2a89b1e158488619d6a35df55dd17a56fdb7d581f87aee32efb2fccc45927",
    "pwSalt" : -5215546943039822041,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-524a6bb0267206aeda278931f7fa35d0",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "93f553eb02dec18b54821d96f69908c3fdca685c98715125a62e6883c545b97c",
    "pwSalt" : -2268177620434170181,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-524a6bb0267206aeda278931f7fa35d0",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "57c3e7af95c125e2345345897cae92bfea0f179f72702415c9ff7da614b69c8e",
    "pwSalt" : -1973324098169489736,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "b32d226b70ed8c8eaebc5c90b3c51577b45dc24393ebb71529b4ce137bba093b",
    "pwSalt" : -4873654651373713347,
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
      "name" : "mgmt-ALERTPUBLISHER-524a6bb0267206aeda278931f7fa35d0",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "b7mpt4eev5mnftjgnt6dayl63",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-ALERTPUBLISHER-BASE"
      }
    }, {
      "name" : "mgmt-EVENTSERVER-524a6bb0267206aeda278931f7fa35d0",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "54gwmhgyxph3vcpw07wvvdtuq",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-EVENTSERVER-BASE"
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-524a6bb0267206aeda278931f7fa35d0",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "dl5ggjfjkyoz2rjnaedjrhvxh",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-HOSTMONITOR-BASE"
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-524a6bb0267206aeda278931f7fa35d0",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "czk65mkc7bt06inv57sgjhj62",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-REPORTSMANAGER-BASE"
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-524a6bb0267206aeda278931f7fa35d0",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "0b7231c7-2331-45bf-98b7-683b93e6017e"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "3f08zbwys0ducfxdq7eesl4n8",
          "sensitive" : true
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
          "value" : "609222656",
          "sensitive" : false
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
          "value" : "609222656",
          "sensitive" : false
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368",
          "sensitive" : false
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
          "value" : "ip-172-31-28-149.ap-southeast-1.compute.internal",
          "sensitive" : false
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman",
          "sensitive" : false
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_password",
          "sensitive" : true
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman",
          "sensitive" : false
        }, {
          "name" : "headlamp_heapsize",
          "value" : "609222656",
          "sensitive" : false
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
          "value" : "609222656",
          "sensitive" : false
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368",
          "sensitive" : false
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
      "value" : "10/21/2012 23:40",
      "sensitive" : false
    }, {
      "name" : "PARCEL_REPO_PATH",
      "value" : "/etc/yum.repos.d",
      "sensitive" : false
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD",
      "sensitive" : false
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,http://archive.cloudera.com/kudu/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/",
      "sensitive" : false
    } ]
  },
  "allHostsConfig" : {
    "items" : [ ]
  },
  "peers" : [ ],
  "hostTemplates" : {
    "items" : [ ]
  }
}
```
