{
    "timestamp": "2018-05-16T17:46:14.521Z",
    "clusters": [
        {
            "name": "mwira",
            "version": "CDH5",
            "services": [
                {
                    "name": "hive",
                    "type": "HIVE",
                    "config": {
                        "roleTypeConfigs": [
                            {
                                "roleType": "HIVEMETASTORE",
                                "items": [
                                    {
                                        "name": "hive_metastore_java_heapsize",
                                        "value": "52428800"
                                    }
                                ]
                            },
                            {
                                "roleType": "HIVESERVER2",
                                "items": [
                                    {
                                        "name": "hiveserver2_java_heapsize",
                                        "value": "1915748352"
                                    },
                                    {
                                        "name": "hiveserver2_spark_driver_memory",
                                        "value": "966367641"
                                    },
                                    {
                                        "name": "hiveserver2_spark_executor_cores",
                                        "value": "4"
                                    },
                                    {
                                        "name": "hiveserver2_spark_executor_memory",
                                        "value": "912680550"
                                    },
                                    {
                                        "name": "hiveserver2_spark_yarn_driver_memory_overhead",
                                        "value": "102"
                                    },
                                    {
                                        "name": "hiveserver2_spark_yarn_executor_memory_overhead",
                                        "value": "153"
                                    }
                                ]
                            }
                        ],
                        "items": [
                            {
                                "name": "hive_metastore_database_host",
                                "value": "ip-172-31-28-220.ap-southeast-1.compute.internal"
                            },
                            {
                                "name": "hive_metastore_database_password",
                                "value": "hive_password"
                            },
                            {
                                "name": "mapreduce_yarn_service",
                                "value": "yarn"
                            },
                            {
                                "name": "zookeeper_service",
                                "value": "zookeeper"
                            }
                        ]
                    },
                    "roles": [
                        {
                            "name": "hive-GATEWAY-37e7e272139d6e22b92d52121b2fda18",
                            "type": "GATEWAY",
                            "hostRef": {
                                "hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"
                            },
                            "config": {
                                "items": []
                            }
                        },
                        {
                            "name": "hive-GATEWAY-96f12e9873efe5e716c4b969548788d3",
                            "type": "GATEWAY",
                            "hostRef": {
                                "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                            },
                            "config": {
                                "items": []
                            }
                        },
                        {
                            "name": "hive-GATEWAY-9fe84b8104f1a573da9bd4e3e8761f2e",
                            "type": "GATEWAY",
                            "hostRef": {
                                "hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"
                            },
                            "config": {
                                "items": []
                            }
                        },
                        {
                            "name": "hive-GATEWAY-f52dfe6a60fb35fe9f6327ea3faf1010",
                            "type": "GATEWAY",
                            "hostRef": {
                                "hostId": "c0de22dc-2ddd-4449-a9bf-be89cb6646b7"
                            },
                            "config": {
                                "items": []
                            }
                        },
                        {
                            "name": "hive-GATEWAY-fc2f458838a9141f6c4972b92c876277",
                            "type": "GATEWAY",
                            "hostRef": {
                                "hostId": "d3e1ba3b-ead8-45fe-a393-7d3b6bb84d82"
                            },
                            "config": {
                                "items": []
                            }
                        },
                        {
                            "name": "hive-HIVEMETASTORE-96f12e9873efe5e716c4b969548788d3",
                            "type": "HIVEMETASTORE",
                            "hostRef": {
                                "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "2moapv86wck7a59sq9rkbydsg"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hive-HIVESERVER2-37e7e272139d6e22b92d52121b2fda18",
                            "type": "HIVESERVER2",
                            "hostRef": {
                                "hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "1uvfehgxq0p9we7mwofaxmxlw"
                                    }
                                ]
                            }
                        }
                    ],
                    "displayName": "Hive"
                },
                {
                    "name": "zookeeper",
                    "type": "ZOOKEEPER",
                    "config": {
                        "roleTypeConfigs": [
                            {
                                "roleType": "SERVER",
                                "items": [
                                    {
                                        "name": "zookeeper_server_java_heapsize",
                                        "value": "52428800"
                                    }
                                ]
                            }
                        ],
                        "items": []
                    },
                    "roles": [
                        {
                            "name": "zookeeper-SERVER-37e7e272139d6e22b92d52121b2fda18",
                            "type": "SERVER",
                            "hostRef": {
                                "hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "e3yuhrchlalj53a9ur64zv914"
                                    },
                                    {
                                        "name": "serverId",
                                        "value": "1"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "zookeeper-SERVER-96f12e9873efe5e716c4b969548788d3",
                            "type": "SERVER",
                            "hostRef": {
                                "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "9jfpppxb3ub3u8wusabr8oyc3"
                                    },
                                    {
                                        "name": "serverId",
                                        "value": "3"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "zookeeper-SERVER-9fe84b8104f1a573da9bd4e3e8761f2e",
                            "type": "SERVER",
                            "hostRef": {
                                "hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "7xcqwte16d6mx0q76xky3bf5d"
                                    },
                                    {
                                        "name": "serverId",
                                        "value": "2"
                                    }
                                ]
                            }
                        }
                    ],
                    "displayName": "ZooKeeper"
                },
                {
                    "name": "hue",
                    "type": "HUE",
                    "config": {
                        "roleTypeConfigs": [],
                        "items": [
                            {
                                "name": "database_host",
                                "value": "ip-172-31-28-220.ap-southeast-1.compute.internal"
                            },
                            {
                                "name": "database_password",
                                "value": "huepassword"
                            },
                            {
                                "name": "database_type",
                                "value": "mysql"
                            },
                            {
                                "name": "hive_service",
                                "value": "hive"
                            },
                            {
                                "name": "hue_webhdfs",
                                "value": "hdfs-HTTPFS-9fe84b8104f1a573da9bd4e3e8761f2e"
                            },
                            {
                                "name": "oozie_service",
                                "value": "oozie"
                            },
                            {
                                "name": "zookeeper_service",
                                "value": "zookeeper"
                            }
                        ]
                    },
                    "roles": [
                        {
                            "name": "hue-HUE_LOAD_BALANCER-37e7e272139d6e22b92d52121b2fda18",
                            "type": "HUE_LOAD_BALANCER",
                            "hostRef": {
                                "hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "6q5gfb8yctk5qo95thyihwu95"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hue-HUE_SERVER-96f12e9873efe5e716c4b969548788d3",
                            "type": "HUE_SERVER",
                            "hostRef": {
                                "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "navmetadataserver_cmdb_password",
                                        "value": "cf424475-c452-4549-b0aa-204760de9541"
                                    },
                                    {
                                        "name": "role_jceks_password",
                                        "value": "9crjj4wwgnbvbb3s6ymn2z2dl"
                                    },
                                    {
                                        "name": "secret_key",
                                        "value": "dRZYhfHHFh36ARO8rWDUgVmsH6whpc"
                                    }
                                ]
                            }
                        }
                    ],
                    "displayName": "Hue"
                },
                {
                    "name": "oozie",
                    "type": "OOZIE",
                    "config": {
                        "roleTypeConfigs": [
                            {
                                "roleType": "OOZIE_SERVER",
                                "items": [
                                    {
                                        "name": "oozie_database_host",
                                        "value": "ip-172-31-28-220.ap-southeast-1.compute.internal"
                                    },
                                    {
                                        "name": "oozie_database_password",
                                        "value": "oozie"
                                    },
                                    {
                                        "name": "oozie_database_type",
                                        "value": "mysql"
                                    },
                                    {
                                        "name": "oozie_database_user",
                                        "value": "oozie"
                                    },
                                    {
                                        "name": "oozie_java_heapsize",
                                        "value": "52428800"
                                    }
                                ]
                            }
                        ],
                        "items": [
                            {
                                "name": "hive_service",
                                "value": "hive"
                            },
                            {
                                "name": "mapreduce_yarn_service",
                                "value": "yarn"
                            },
                            {
                                "name": "oozie_upload_sharelib_cmd_timeout",
                                "value": "2000"
                            },
                            {
                                "name": "zookeeper_service",
                                "value": "zookeeper"
                            }
                        ]
                    },
                    "roles": [
                        {
                            "name": "oozie-OOZIE_SERVER-96f12e9873efe5e716c4b969548788d3",
                            "type": "OOZIE_SERVER",
                            "hostRef": {
                                "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "8rsc6ng0cqfg4lop7kiljvwk5"
                                    }
                                ]
                            }
                        }
                    ],
                    "displayName": "Oozie"
                },
                {
                    "name": "yarn",
                    "type": "YARN",
                    "config": {
                        "roleTypeConfigs": [
                            {
                                "roleType": "GATEWAY",
                                "items": [
                                    {
                                        "name": "mapred_reduce_tasks",
                                        "value": "8"
                                    },
                                    {
                                        "name": "mapred_submit_replication",
                                        "value": "3"
                                    }
                                ]
                            },
                            {
                                "roleType": "NODEMANAGER",
                                "items": [
                                    {
                                        "name": "yarn_nodemanager_heartbeat_interval_ms",
                                        "value": "100"
                                    },
                                    {
                                        "name": "yarn_nodemanager_local_dirs",
                                        "value": "/yarn/nm"
                                    },
                                    {
                                        "name": "yarn_nodemanager_log_dirs",
                                        "value": "/yarn/container-logs"
                                    },
                                    {
                                        "name": "yarn_nodemanager_resource_cpu_vcores",
                                        "value": "4"
                                    },
                                    {
                                        "name": "yarn_nodemanager_resource_memory_mb",
                                        "value": "5949"
                                    }
                                ]
                            },
                            {
                                "roleType": "RESOURCEMANAGER",
                                "items": [
                                    {
                                        "name": "yarn_scheduler_maximum_allocation_mb",
                                        "value": "5949"
                                    },
                                    {
                                        "name": "yarn_scheduler_maximum_allocation_vcores",
                                        "value": "4"
                                    }
                                ]
                            }
                        ],
                        "items": [
                            {
                                "name": "hdfs_service",
                                "value": "hdfs"
                            },
                            {
                                "name": "rm_dirty",
                                "value": "true"
                            },
                            {
                                "name": "zk_authorization_secret_key",
                                "value": "YBrnqMN44XUQOz6HidCWP1poHZjgwH"
                            },
                            {
                                "name": "zookeeper_service",
                                "value": "zookeeper"
                            }
                        ]
                    },
                    "roles": [
                        {
                            "name": "yarn-JOBHISTORY-37e7e272139d6e22b92d52121b2fda18",
                            "type": "JOBHISTORY",
                            "hostRef": {
                                "hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "c2om919k3366ted5qi6jnbhs3"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "yarn-NODEMANAGER-96f12e9873efe5e716c4b969548788d3",
                            "type": "NODEMANAGER",
                            "hostRef": {
                                "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "7sdxoo9adjo51jtv4wmfzbfm2"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "yarn-NODEMANAGER-9fe84b8104f1a573da9bd4e3e8761f2e",
                            "type": "NODEMANAGER",
                            "hostRef": {
                                "hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "bnh3bcxaj4vatirejc4woeq7m"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "yarn-NODEMANAGER-f52dfe6a60fb35fe9f6327ea3faf1010",
                            "type": "NODEMANAGER",
                            "hostRef": {
                                "hostId": "c0de22dc-2ddd-4449-a9bf-be89cb6646b7"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "2t5smumvvuxipzz7hughsep1n"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "yarn-NODEMANAGER-fc2f458838a9141f6c4972b92c876277",
                            "type": "NODEMANAGER",
                            "hostRef": {
                                "hostId": "d3e1ba3b-ead8-45fe-a393-7d3b6bb84d82"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "6s9000hniwjjaqwxnymzndz5m"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "yarn-RESOURCEMANAGER-37e7e272139d6e22b92d52121b2fda18",
                            "type": "RESOURCEMANAGER",
                            "hostRef": {
                                "hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "rm_id",
                                        "value": "160"
                                    },
                                    {
                                        "name": "role_jceks_password",
                                        "value": "3tgcbg7884h4qw8fp8q9mh0n8"
                                    }
                                ]
                            }
                        }
                    ],
                    "displayName": "YARN (MR2 Included)"
                },
                {
                    "name": "hdfs",
                    "type": "HDFS",
                    "config": {
                        "roleTypeConfigs": [
                            {
                                "roleType": "DATANODE",
                                "items": [
                                    {
                                        "name": "dfs_data_dir_list",
                                        "value": "/dfs/dn"
                                    },
                                    {
                                        "name": "dfs_datanode_du_reserved",
                                        "value": "4293811814"
                                    }
                                ]
                            },
                            {
                                "roleType": "GATEWAY",
                                "items": [
                                    {
                                        "name": "dfs_client_use_trash",
                                        "value": "true"
                                    }
                                ]
                            },
                            {
                                "roleType": "JOURNALNODE",
                                "items": [
                                    {
                                        "name": "dfs_journalnode_edits_dir",
                                        "value": "/dfs/jn"
                                    }
                                ]
                            },
                            {
                                "roleType": "NAMENODE",
                                "items": [
                                    {
                                        "name": "dfs_name_dir_list",
                                        "value": "/dfs/nn"
                                    },
                                    {
                                        "name": "dfs_namenode_servicerpc_address",
                                        "value": "8022"
                                    },
                                    {
                                        "name": "namenode_java_heapsize",
                                        "value": "1915748352"
                                    }
                                ]
                            },
                            {
                                "roleType": "SECONDARYNAMENODE",
                                "items": [
                                    {
                                        "name": "fs_checkpoint_dir_list",
                                        "value": "/dfs/snn"
                                    },
                                    {
                                        "name": "secondary_namenode_java_heapsize",
                                        "value": "1915748352"
                                    }
                                ]
                            }
                        ],
                        "items": [
                            {
                                "name": "dfs_ha_fencing_cloudera_manager_secret_key",
                                "value": "1sUUn8iD9xPPwTkMoPMwvDADggaMse"
                            },
                            {
                                "name": "dfs_namenode_acls_enabled",
                                "value": "true"
                            },
                            {
                                "name": "fc_authorization_secret_key",
                                "value": "G273Q1XUdXizE6kRNsXk6dmy36aSyh"
                            },
                            {
                                "name": "http_auth_signature_secret",
                                "value": "Lj3Er84290rJ5LhBfpQR3mSp44oBr6"
                            },
                            {
                                "name": "rm_dirty",
                                "value": "true"
                            },
                            {
                                "name": "zookeeper_service",
                                "value": "zookeeper"
                            }
                        ]
                    },
                    "roles": [
                        {
                            "name": "hdfs-BALANCER-37e7e272139d6e22b92d52121b2fda18",
                            "type": "BALANCER",
                            "hostRef": {
                                "hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"
                            },
                            "config": {
                                "items": []
                            }
                        },
                        {
                            "name": "hdfs-DATANODE-96f12e9873efe5e716c4b969548788d3",
                            "type": "DATANODE",
                            "hostRef": {
                                "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "7wjjv1bmi05b90u1rmy55m1jm"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hdfs-DATANODE-9fe84b8104f1a573da9bd4e3e8761f2e",
                            "type": "DATANODE",
                            "hostRef": {
                                "hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "2iqjwq249t9l2zbkr42vj2b0r"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hdfs-DATANODE-f52dfe6a60fb35fe9f6327ea3faf1010",
                            "type": "DATANODE",
                            "hostRef": {
                                "hostId": "c0de22dc-2ddd-4449-a9bf-be89cb6646b7"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "2evy3gsih3tm46bl9bbjq7rdz"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hdfs-DATANODE-fc2f458838a9141f6c4972b92c876277",
                            "type": "DATANODE",
                            "hostRef": {
                                "hostId": "d3e1ba3b-ead8-45fe-a393-7d3b6bb84d82"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "8x7y3ez2k2mfgi18zen8imvtd"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hdfs-FAILOVERCONTROLLER-37e7e272139d6e22b92d52121b2fda18",
                            "type": "FAILOVERCONTROLLER",
                            "hostRef": {
                                "hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "1lcqu2ffx7j5yu7wy8vik9kft"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hdfs-FAILOVERCONTROLLER-9fe84b8104f1a573da9bd4e3e8761f2e",
                            "type": "FAILOVERCONTROLLER",
                            "hostRef": {
                                "hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "f14v0dfgxexipnunhynxzsnzl"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hdfs-HTTPFS-9fe84b8104f1a573da9bd4e3e8761f2e",
                            "type": "HTTPFS",
                            "hostRef": {
                                "hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "57w7cfh8jrsbr3ftjyfl76mjr"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hdfs-JOURNALNODE-37e7e272139d6e22b92d52121b2fda18",
                            "type": "JOURNALNODE",
                            "hostRef": {
                                "hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "7egeotk391l2bf94mlg7dsgjx"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hdfs-JOURNALNODE-9fe84b8104f1a573da9bd4e3e8761f2e",
                            "type": "JOURNALNODE",
                            "hostRef": {
                                "hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "1v7vkg7diby3umyehv5u1go89"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hdfs-JOURNALNODE-fc2f458838a9141f6c4972b92c876277",
                            "type": "JOURNALNODE",
                            "hostRef": {
                                "hostId": "d3e1ba3b-ead8-45fe-a393-7d3b6bb84d82"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "role_jceks_password",
                                        "value": "97f4rqj0pnccjbt49st6w5ive"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hdfs-NAMENODE-37e7e272139d6e22b92d52121b2fda18",
                            "type": "NAMENODE",
                            "hostRef": {
                                "hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "autofailover_enabled",
                                        "value": "true"
                                    },
                                    {
                                        "name": "dfs_federation_namenode_nameservice",
                                        "value": "nameservice1"
                                    },
                                    {
                                        "name": "dfs_namenode_quorum_journal_name",
                                        "value": "nameservice1"
                                    },
                                    {
                                        "name": "namenode_id",
                                        "value": "162"
                                    },
                                    {
                                        "name": "role_jceks_password",
                                        "value": "arjhpga3v62zw8yq3jivxu8ms"
                                    }
                                ]
                            }
                        },
                        {
                            "name": "hdfs-NAMENODE-9fe84b8104f1a573da9bd4e3e8761f2e",
                            "type": "NAMENODE",
                            "hostRef": {
                                "hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"
                            },
                            "config": {
                                "items": [
                                    {
                                        "name": "autofailover_enabled",
                                        "value": "true"
                                    },
                                    {
                                        "name": "dfs_federation_namenode_nameservice",
                                        "value": "nameservice1"
                                    },
                                    {
                                        "name": "dfs_namenode_quorum_journal_name",
                                        "value": "nameservice1"
                                    },
                                    {
                                        "name": "namenode_id",
                                        "value": "172"
                                    },
                                    {
                                        "name": "role_jceks_password",
                                        "value": "9rs6h5f3h2fmd3c2n57i0eldu"
                                    }
                                ]
                            }
                        }
                    ],
                    "displayName": "HDFS"
                }
            ]
        }
    ],
    "hosts": [
        {
            "hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59",
            "ipAddress": "172.31.17.222",
            "hostname": "ip-172-31-17-222.ap-southeast-1.compute.internal",
            "rackId": "/default",
            "config": {
                "items": []
            }
        },
        {
            "hostId": "9d54f582-4362-4488-8f65-219d4a33ed33",
            "ipAddress": "172.31.23.18",
            "hostname": "ip-172-31-23-18.ap-southeast-1.compute.internal",
            "rackId": "/default",
            "config": {
                "items": []
            }
        },
        {
            "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc",
            "ipAddress": "172.31.28.220",
            "hostname": "ip-172-31-28-220.ap-southeast-1.compute.internal",
            "rackId": "/default",
            "config": {
                "items": []
            }
        },
        {
            "hostId": "d3e1ba3b-ead8-45fe-a393-7d3b6bb84d82",
            "ipAddress": "172.31.28.41",
            "hostname": "ip-172-31-28-41.ap-southeast-1.compute.internal",
            "rackId": "/default",
            "config": {
                "items": []
            }
        },
        {
            "hostId": "c0de22dc-2ddd-4449-a9bf-be89cb6646b7",
            "ipAddress": "172.31.28.50",
            "hostname": "ip-172-31-28-50.ap-southeast-1.compute.internal",
            "rackId": "/default",
            "config": {
                "items": []
            }
        }
    ],
    "users": [
        {
            "name": "__cloudera_internal_user__hue-HUE_SERVER-96f12e9873efe5e716c4b969548788d3",
            "roles": [
                "ROLE_NAVIGATOR_ADMIN"
            ],
            "pwHash": "84a110feb17713a180cbc30f0eb85b101b5e657a1fb6b2d23e5f107794918249",
            "pwSalt": 4617898858791690637,
            "pwLogin": true
        },
        {
            "name": "__cloudera_internal_user__mgmt-ACTIVITYMONITOR-96f12e9873efe5e716c4b969548788d3",
            "roles": [
                "ROLE_USER"
            ],
            "pwHash": "926f60ce1ba3728def271715cefa831aa9e99a5b57a488887df13bed4cbd1571",
            "pwSalt": 3756777870399121384,
            "pwLogin": true
        },
        {
            "name": "__cloudera_internal_user__mgmt-EVENTSERVER-96f12e9873efe5e716c4b969548788d3",
            "roles": [
                "ROLE_USER"
            ],
            "pwHash": "16a28f0767fcf6eac17624fddc8ee0dd2c1eab43b1dedac2f21c7fddeaaf3e25",
            "pwSalt": -7338933284551352999,
            "pwLogin": true
        },
        {
            "name": "__cloudera_internal_user__mgmt-HOSTMONITOR-96f12e9873efe5e716c4b969548788d3",
            "roles": [
                "ROLE_USER"
            ],
            "pwHash": "e40dbc0cb57397d6f2aa99c84d280d9e952bf5120fc29b1e50d97bf481329594",
            "pwSalt": -8368346909352992251,
            "pwLogin": true
        },
        {
            "name": "__cloudera_internal_user__mgmt-NAVIGATOR-96f12e9873efe5e716c4b969548788d3",
            "roles": [
                "ROLE_USER"
            ],
            "pwHash": "25e9697deaf489d7bc25edbb561b298ef4cb0886ea39c0c778250acf6333bd7a",
            "pwSalt": 3669424674689533297,
            "pwLogin": true
        },
        {
            "name": "__cloudera_internal_user__mgmt-NAVIGATORMETASERVER-96f12e9873efe5e716c4b969548788d3",
            "roles": [
                "ROLE_ADMIN"
            ],
            "pwHash": "90e151656f0183809edf4942fc579dca47be452354fedcba9ae045ca1532a91d",
            "pwSalt": 5488732577907527515,
            "pwLogin": true
        },
        {
            "name": "__cloudera_internal_user__mgmt-REPORTSMANAGER-96f12e9873efe5e716c4b969548788d3",
            "roles": [
                "ROLE_USER"
            ],
            "pwHash": "93caddc90eb7c21114759a4d03704b4d278e44f395d39f36bd7ba955011ca4ea",
            "pwSalt": -4978520779599535087,
            "pwLogin": true
        },
        {
            "name": "__cloudera_internal_user__mgmt-SERVICEMONITOR-96f12e9873efe5e716c4b969548788d3",
            "roles": [
                "ROLE_USER"
            ],
            "pwHash": "72c561d0f3e488c54340d09274f49bdcfa01a2d4f95a44cb7f1cd002efa96369",
            "pwSalt": 4895842479454989859,
            "pwLogin": true
        },
        {
            "name": "admin",
            "roles": [
                "ROLE_LIMITED"
            ],
            "pwHash": "68107b6961cbf4a0953cc031caffaf3aa069abd041d0f96a4c0bed38930a4f8f",
            "pwSalt": -8570728715721155791,
            "pwLogin": true
        },
        {
            "name": "minotaur",
            "roles": [
                "ROLE_CONFIGURATOR"
            ],
            "pwHash": "d5e7f682050a8d1fb184424d2fd6a8cab3a6fb6cab02c1606f5adc13eadabbe7",
            "pwSalt": -6633181738536505671,
            "pwLogin": true
        },
        {
            "name": "mwira",
            "roles": [
                "ROLE_ADMIN"
            ],
            "pwHash": "e6e1c10139bf22993a0a87e4cf3a273e0899927b16750d1bfa473e433ac5bab4",
            "pwSalt": -3607734412307643475,
            "pwLogin": true
        }
    ],
    "versionInfo": {
        "version": "5.14.3",
        "buildUser": "jenkins",
        "buildTimestamp": "20180414-0409",
        "gitHash": "7f2725eea4edeb1d184a2888db790d332167b6f8",
        "snapshot": false
    },
    "managementService": {
        "name": "mgmt",
        "type": "MGMT",
        "config": {
            "roleTypeConfigs": [
                {
                    "roleType": "ACTIVITYMONITOR",
                    "items": [
                        {
                            "name": "firehose_database_host",
                            "value": "ip-172-31-28-220.ap-southeast-1.compute.internal"
                        },
                        {
                            "name": "firehose_database_name",
                            "value": "amon"
                        },
                        {
                            "name": "firehose_database_password",
                            "value": "amon_password"
                        },
                        {
                            "name": "firehose_database_user",
                            "value": "amon"
                        }
                    ]
                },
                {
                    "roleType": "HOSTMONITOR",
                    "items": [
                        {
                            "name": "firehose_non_java_memory_bytes",
                            "value": "1533018112"
                        }
                    ]
                },
                {
                    "roleType": "NAVIGATOR",
                    "items": [
                        {
                            "name": "navigator_database_host",
                            "value": "ip-172-31-28-220.ap-southeast-1.compute.internal"
                        },
                        {
                            "name": "navigator_database_name",
                            "value": "navms"
                        },
                        {
                            "name": "navigator_database_password",
                            "value": "navms_password"
                        },
                        {
                            "name": "navigator_database_user",
                            "value": "navms"
                        }
                    ]
                },
                {
                    "roleType": "NAVIGATORMETASERVER",
                    "items": [
                        {
                            "name": "nav_metaserver_database_host",
                            "value": "ip-172-31-28-220.ap-southeast-1.compute.internal"
                        },
                        {
                            "name": "nav_metaserver_database_name",
                            "value": "nav"
                        },
                        {
                            "name": "nav_metaserver_database_password",
                            "value": "nav_password"
                        },
                        {
                            "name": "nav_metaserver_database_user",
                            "value": "nav"
                        },
                        {
                            "name": "navigator_heapsize",
                            "value": "1179648000"
                        }
                    ]
                },
                {
                    "roleType": "REPORTSMANAGER",
                    "items": [
                        {
                            "name": "headlamp_database_host",
                            "value": "ip-172-31-28-220.ap-southeast-1.compute.internal"
                        },
                        {
                            "name": "headlamp_database_name",
                            "value": "rman"
                        },
                        {
                            "name": "headlamp_database_password",
                            "value": "rman_password"
                        },
                        {
                            "name": "headlamp_database_user",
                            "value": "rman"
                        }
                    ]
                },
                {
                    "roleType": "SERVICEMONITOR",
                    "items": [
                        {
                            "name": "firehose_non_java_memory_bytes",
                            "value": "1533018112"
                        }
                    ]
                }
            ],
            "items": []
        },
        "roles": [
            {
                "name": "mgmt-ACTIVITYMONITOR-96f12e9873efe5e716c4b969548788d3",
                "type": "ACTIVITYMONITOR",
                "hostRef": {
                    "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                },
                "config": {
                    "items": [
                        {
                            "name": "role_jceks_password",
                            "value": "f4cnxqtjt8dnaaw41imx5lyp7"
                        }
                    ]
                }
            },
            {
                "name": "mgmt-ALERTPUBLISHER-96f12e9873efe5e716c4b969548788d3",
                "type": "ALERTPUBLISHER",
                "hostRef": {
                    "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                },
                "config": {
                    "items": [
                        {
                            "name": "role_jceks_password",
                            "value": "4cz15kkx7djhns0wabheca5q"
                        }
                    ]
                }
            },
            {
                "name": "mgmt-EVENTSERVER-96f12e9873efe5e716c4b969548788d3",
                "type": "EVENTSERVER",
                "hostRef": {
                    "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                },
                "config": {
                    "items": [
                        {
                            "name": "role_jceks_password",
                            "value": "5sy9ylhey1o3d3bcnv3geo1z3"
                        }
                    ]
                }
            },
            {
                "name": "mgmt-HOSTMONITOR-96f12e9873efe5e716c4b969548788d3",
                "type": "HOSTMONITOR",
                "hostRef": {
                    "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                },
                "config": {
                    "items": [
                        {
                            "name": "role_jceks_password",
                            "value": "26fizrink8t8ewjynjxrc94y4"
                        }
                    ]
                }
            },
            {
                "name": "mgmt-NAVIGATOR-96f12e9873efe5e716c4b969548788d3",
                "type": "NAVIGATOR",
                "hostRef": {
                    "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                },
                "config": {
                    "items": [
                        {
                            "name": "role_jceks_password",
                            "value": "eo8esq9uma3jkzte5qovgl2hq"
                        }
                    ]
                }
            },
            {
                "name": "mgmt-NAVIGATORMETASERVER-96f12e9873efe5e716c4b969548788d3",
                "type": "NAVIGATORMETASERVER",
                "hostRef": {
                    "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                },
                "config": {
                    "items": [
                        {
                            "name": "role_jceks_password",
                            "value": "1lju26kz7u3zb16ovezr55yk4"
                        }
                    ]
                }
            },
            {
                "name": "mgmt-REPORTSMANAGER-96f12e9873efe5e716c4b969548788d3",
                "type": "REPORTSMANAGER",
                "hostRef": {
                    "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                },
                "config": {
                    "items": [
                        {
                            "name": "role_jceks_password",
                            "value": "3o4jqzx98kev3ql51cs4fp33w"
                        }
                    ]
                }
            },
            {
                "name": "mgmt-SERVICEMONITOR-96f12e9873efe5e716c4b969548788d3",
                "type": "SERVICEMONITOR",
                "hostRef": {
                    "hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"
                },
                "config": {
                    "items": [
                        {
                            "name": "role_jceks_password",
                            "value": "bfjufyqfjpj3cq70ye8o9pc10"
                        }
                    ]
                }
            }
        ],
        "displayName": "Cloudera Management Service"
    },
    "managerSettings": {
        "items": [
            {
                "name": "CLUSTER_STATS_START",
                "value": "10/27/2012 18:10"
            },
            {
                "name": "PUBLIC_CLOUD_STATUS",
                "value": "ON_PUBLIC_CLOUD"
            },
            {
                "name": "REMOTE_PARCEL_REPO_URLS",
                "value": "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,http://archive.cloudera.com/kudu/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
            }
        ]
    }
}
