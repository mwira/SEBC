{<br />
	"timestamp": "2018-05-16T17:46:14.521Z",<br />
	"clusters": [<br />
		{<br />
			"name": "mwira",<br />
			"version": "CDH5",<br />
			"services": [<br />
				{<br />
					"name": "hive",<br />
					"type": "HIVE",<br />
					"config": {<br />
						"roleTypeConfigs": [<br />
							{<br />
								"roleType": "HIVEMETASTORE",<br />
								"items": [<br />
									{<br />
										"name": "hive_metastore_java_heapsize",<br />
										"value": "52428800"<br />
									}<br />
								]<br />
							},<br />
							{<br />
								"roleType": "HIVESERVER2",<br />
								"items": [<br />
									{<br />
										"name": "hiveserver2_java_heapsize",<br />
										"value": "1915748352"<br />
									},<br />
									{<br />
										"name": "hiveserver2_spark_driver_memory",<br />
										"value": "966367641"<br />
									},<br />
									{<br />
										"name": "hiveserver2_spark_executor_cores",<br />
										"value": "4"<br />
									},<br />
									{<br />
										"name": "hiveserver2_spark_executor_memory",<br />
										"value": "912680550"<br />
									},<br />
									{<br />
										"name": "hiveserver2_spark_yarn_driver_memory_overhead",<br />
										"value": "102"<br />
									},<br />
									{<br />
										"name": "hiveserver2_spark_yarn_executor_memory_overhead",<br />
										"value": "153"<br />
									}<br />
								]<br />
							}<br />
						],<br />
						"items": [<br />
							{<br />
								"name": "hive_metastore_database_host",<br />
								"value": "ip-172-31-28-220.ap-southeast-1.compute.internal"<br />
							},<br />
							{<br />
								"name": "hive_metastore_database_password",<br />
								"value": "hive_password"<br />
							},<br />
							{<br />
								"name": "mapreduce_yarn_service",<br />
								"value": "yarn"<br />
							},<br />
							{<br />
								"name": "zookeeper_service",<br />
								"value": "zookeeper"<br />
							}<br />
						]<br />
					},<br />
					"roles": [<br />
						{<br />
							"name": "hive-GATEWAY-37e7e272139d6e22b92d52121b2fda18",<br />
							"type": "GATEWAY",<br />
							"hostRef": {<br />
								"hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"<br />
							},<br />
							"config": {<br />
								"items": []<br />
							}<br />
						},<br />
						{<br />
							"name": "hive-GATEWAY-96f12e9873efe5e716c4b969548788d3",<br />
							"type": "GATEWAY",<br />
							"hostRef": {<br />
								"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
							},<br />
							"config": {<br />
								"items": []<br />
							}<br />
						},<br />
						{<br />
							"name": "hive-GATEWAY-9fe84b8104f1a573da9bd4e3e8761f2e",<br />
							"type": "GATEWAY",<br />
							"hostRef": {<br />
								"hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"<br />
							},<br />
							"config": {<br />
								"items": []<br />
							}<br />
						},<br />
						{<br />
							"name": "hive-GATEWAY-f52dfe6a60fb35fe9f6327ea3faf1010",<br />
							"type": "GATEWAY",<br />
							"hostRef": {<br />
								"hostId": "c0de22dc-2ddd-4449-a9bf-be89cb6646b7"<br />
							},<br />
							"config": {<br />
								"items": []<br />
							}<br />
						},<br />
						{<br />
							"name": "hive-GATEWAY-fc2f458838a9141f6c4972b92c876277",<br />
							"type": "GATEWAY",<br />
							"hostRef": {<br />
								"hostId": "d3e1ba3b-ead8-45fe-a393-7d3b6bb84d82"<br />
							},<br />
							"config": {<br />
								"items": []<br />
							}<br />
						},<br />
						{<br />
							"name": "hive-HIVEMETASTORE-96f12e9873efe5e716c4b969548788d3",<br />
							"type": "HIVEMETASTORE",<br />
							"hostRef": {<br />
								"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "2moapv86wck7a59sq9rkbydsg"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hive-HIVESERVER2-37e7e272139d6e22b92d52121b2fda18",<br />
							"type": "HIVESERVER2",<br />
							"hostRef": {<br />
								"hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "1uvfehgxq0p9we7mwofaxmxlw"<br />
									}<br />
								]<br />
							}<br />
						}<br />
					],<br />
					"displayName": "Hive"<br />
				},<br />
				{<br />
					"name": "zookeeper",<br />
					"type": "ZOOKEEPER",<br />
					"config": {<br />
						"roleTypeConfigs": [<br />
							{<br />
								"roleType": "SERVER",<br />
								"items": [<br />
									{<br />
										"name": "zookeeper_server_java_heapsize",<br />
										"value": "52428800"<br />
									}<br />
								]<br />
							}<br />
						],<br />
						"items": []<br />
					},<br />
					"roles": [<br />
						{<br />
							"name": "zookeeper-SERVER-37e7e272139d6e22b92d52121b2fda18",<br />
							"type": "SERVER",<br />
							"hostRef": {<br />
								"hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "e3yuhrchlalj53a9ur64zv914"<br />
									},<br />
									{<br />
										"name": "serverId",<br />
										"value": "1"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "zookeeper-SERVER-96f12e9873efe5e716c4b969548788d3",<br />
							"type": "SERVER",<br />
							"hostRef": {<br />
								"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "9jfpppxb3ub3u8wusabr8oyc3"<br />
									},<br />
									{<br />
										"name": "serverId",<br />
										"value": "3"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "zookeeper-SERVER-9fe84b8104f1a573da9bd4e3e8761f2e",<br />
							"type": "SERVER",<br />
							"hostRef": {<br />
								"hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "7xcqwte16d6mx0q76xky3bf5d"<br />
									},<br />
									{<br />
										"name": "serverId",<br />
										"value": "2"<br />
									}<br />
								]<br />
							}<br />
						}<br />
					],<br />
					"displayName": "ZooKeeper"<br />
				},<br />
				{<br />
					"name": "hue",<br />
					"type": "HUE",<br />
					"config": {<br />
						"roleTypeConfigs": [],<br />
						"items": [<br />
							{<br />
								"name": "database_host",<br />
								"value": "ip-172-31-28-220.ap-southeast-1.compute.internal"<br />
							},<br />
							{<br />
								"name": "database_password",<br />
								"value": "huepassword"<br />
							},<br />
							{<br />
								"name": "database_type",<br />
								"value": "mysql"<br />
							},<br />
							{<br />
								"name": "hive_service",<br />
								"value": "hive"<br />
							},<br />
							{<br />
								"name": "hue_webhdfs",<br />
								"value": "hdfs-HTTPFS-9fe84b8104f1a573da9bd4e3e8761f2e"<br />
							},<br />
							{<br />
								"name": "oozie_service",<br />
								"value": "oozie"<br />
							},<br />
							{<br />
								"name": "zookeeper_service",<br />
								"value": "zookeeper"<br />
							}<br />
						]<br />
					},<br />
					"roles": [<br />
						{<br />
							"name": "hue-HUE_LOAD_BALANCER-37e7e272139d6e22b92d52121b2fda18",<br />
							"type": "HUE_LOAD_BALANCER",<br />
							"hostRef": {<br />
								"hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "6q5gfb8yctk5qo95thyihwu95"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hue-HUE_SERVER-96f12e9873efe5e716c4b969548788d3",<br />
							"type": "HUE_SERVER",<br />
							"hostRef": {<br />
								"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "navmetadataserver_cmdb_password",<br />
										"value": "cf424475-c452-4549-b0aa-204760de9541"<br />
									},<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "9crjj4wwgnbvbb3s6ymn2z2dl"<br />
									},<br />
									{<br />
										"name": "secret_key",<br />
										"value": "dRZYhfHHFh36ARO8rWDUgVmsH6whpc"<br />
									}<br />
								]<br />
							}<br />
						}<br />
					],<br />
					"displayName": "Hue"<br />
				},<br />
				{<br />
					"name": "oozie",<br />
					"type": "OOZIE",<br />
					"config": {<br />
						"roleTypeConfigs": [<br />
							{<br />
								"roleType": "OOZIE_SERVER",<br />
								"items": [<br />
									{<br />
										"name": "oozie_database_host",<br />
										"value": "ip-172-31-28-220.ap-southeast-1.compute.internal"<br />
									},<br />
									{<br />
										"name": "oozie_database_password",<br />
										"value": "oozie"<br />
									},<br />
									{<br />
										"name": "oozie_database_type",<br />
										"value": "mysql"<br />
									},<br />
									{<br />
										"name": "oozie_database_user",<br />
										"value": "oozie"<br />
									},<br />
									{<br />
										"name": "oozie_java_heapsize",<br />
										"value": "52428800"<br />
									}<br />
								]<br />
							}<br />
						],<br />
						"items": [<br />
							{<br />
								"name": "hive_service",<br />
								"value": "hive"<br />
							},<br />
							{<br />
								"name": "mapreduce_yarn_service",<br />
								"value": "yarn"<br />
							},<br />
							{<br />
								"name": "oozie_upload_sharelib_cmd_timeout",<br />
								"value": "2000"<br />
							},<br />
							{<br />
								"name": "zookeeper_service",<br />
								"value": "zookeeper"<br />
							}<br />
						]<br />
					},<br />
					"roles": [<br />
						{<br />
							"name": "oozie-OOZIE_SERVER-96f12e9873efe5e716c4b969548788d3",<br />
							"type": "OOZIE_SERVER",<br />
							"hostRef": {<br />
								"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "8rsc6ng0cqfg4lop7kiljvwk5"<br />
									}<br />
								]<br />
							}<br />
						}<br />
					],<br />
					"displayName": "Oozie"<br />
				},<br />
				{<br />
					"name": "yarn",<br />
					"type": "YARN",<br />
					"config": {<br />
						"roleTypeConfigs": [<br />
							{<br />
								"roleType": "GATEWAY",<br />
								"items": [<br />
									{<br />
										"name": "mapred_reduce_tasks",<br />
										"value": "8"<br />
									},<br />
									{<br />
										"name": "mapred_submit_replication",<br />
										"value": "3"<br />
									}<br />
								]<br />
							},<br />
							{<br />
								"roleType": "NODEMANAGER",<br />
								"items": [<br />
									{<br />
										"name": "yarn_nodemanager_heartbeat_interval_ms",<br />
										"value": "100"<br />
									},<br />
									{<br />
										"name": "yarn_nodemanager_local_dirs",<br />
										"value": "/yarn/nm"<br />
									},<br />
									{<br />
										"name": "yarn_nodemanager_log_dirs",<br />
										"value": "/yarn/container-logs"<br />
									},<br />
									{<br />
										"name": "yarn_nodemanager_resource_cpu_vcores",<br />
										"value": "4"<br />
									},<br />
									{<br />
										"name": "yarn_nodemanager_resource_memory_mb",<br />
										"value": "5949"<br />
									}<br />
								]<br />
							},<br />
							{<br />
								"roleType": "RESOURCEMANAGER",<br />
								"items": [<br />
									{<br />
										"name": "yarn_scheduler_maximum_allocation_mb",<br />
										"value": "5949"<br />
									},<br />
									{<br />
										"name": "yarn_scheduler_maximum_allocation_vcores",<br />
										"value": "4"<br />
									}<br />
								]<br />
							}<br />
						],<br />
						"items": [<br />
							{<br />
								"name": "hdfs_service",<br />
								"value": "hdfs"<br />
							},<br />
							{<br />
								"name": "rm_dirty",<br />
								"value": "true"<br />
							},<br />
							{<br />
								"name": "zk_authorization_secret_key",<br />
								"value": "YBrnqMN44XUQOz6HidCWP1poHZjgwH"<br />
							},<br />
							{<br />
								"name": "zookeeper_service",<br />
								"value": "zookeeper"<br />
							}<br />
						]<br />
					},<br />
					"roles": [<br />
						{<br />
							"name": "yarn-JOBHISTORY-37e7e272139d6e22b92d52121b2fda18",<br />
							"type": "JOBHISTORY",<br />
							"hostRef": {<br />
								"hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "c2om919k3366ted5qi6jnbhs3"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "yarn-NODEMANAGER-96f12e9873efe5e716c4b969548788d3",<br />
							"type": "NODEMANAGER",<br />
							"hostRef": {<br />
								"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "7sdxoo9adjo51jtv4wmfzbfm2"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "yarn-NODEMANAGER-9fe84b8104f1a573da9bd4e3e8761f2e",<br />
							"type": "NODEMANAGER",<br />
							"hostRef": {<br />
								"hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "bnh3bcxaj4vatirejc4woeq7m"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "yarn-NODEMANAGER-f52dfe6a60fb35fe9f6327ea3faf1010",<br />
							"type": "NODEMANAGER",<br />
							"hostRef": {<br />
								"hostId": "c0de22dc-2ddd-4449-a9bf-be89cb6646b7"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "2t5smumvvuxipzz7hughsep1n"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "yarn-NODEMANAGER-fc2f458838a9141f6c4972b92c876277",<br />
							"type": "NODEMANAGER",<br />
							"hostRef": {<br />
								"hostId": "d3e1ba3b-ead8-45fe-a393-7d3b6bb84d82"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "6s9000hniwjjaqwxnymzndz5m"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "yarn-RESOURCEMANAGER-37e7e272139d6e22b92d52121b2fda18",<br />
							"type": "RESOURCEMANAGER",<br />
							"hostRef": {<br />
								"hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "rm_id",<br />
										"value": "160"<br />
									},<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "3tgcbg7884h4qw8fp8q9mh0n8"<br />
									}<br />
								]<br />
							}<br />
						}<br />
					],<br />
					"displayName": "YARN (MR2 Included)"<br />
				},<br />
				{<br />
					"name": "hdfs",<br />
					"type": "HDFS",<br />
					"config": {<br />
						"roleTypeConfigs": [<br />
							{<br />
								"roleType": "DATANODE",<br />
								"items": [<br />
									{<br />
										"name": "dfs_data_dir_list",<br />
										"value": "/dfs/dn"<br />
									},<br />
									{<br />
										"name": "dfs_datanode_du_reserved",<br />
										"value": "4293811814"<br />
									}<br />
								]<br />
							},<br />
							{<br />
								"roleType": "GATEWAY",<br />
								"items": [<br />
									{<br />
										"name": "dfs_client_use_trash",<br />
										"value": "true"<br />
									}<br />
								]<br />
							},<br />
							{<br />
								"roleType": "JOURNALNODE",<br />
								"items": [<br />
									{<br />
										"name": "dfs_journalnode_edits_dir",<br />
										"value": "/dfs/jn"<br />
									}<br />
								]<br />
							},<br />
							{<br />
								"roleType": "NAMENODE",<br />
								"items": [<br />
									{<br />
										"name": "dfs_name_dir_list",<br />
										"value": "/dfs/nn"<br />
									},<br />
									{<br />
										"name": "dfs_namenode_servicerpc_address",<br />
										"value": "8022"<br />
									},<br />
									{<br />
										"name": "namenode_java_heapsize",<br />
										"value": "1915748352"<br />
									}<br />
								]<br />
							},<br />
							{<br />
								"roleType": "SECONDARYNAMENODE",<br />
								"items": [<br />
									{<br />
										"name": "fs_checkpoint_dir_list",<br />
										"value": "/dfs/snn"<br />
									},<br />
									{<br />
										"name": "secondary_namenode_java_heapsize",<br />
										"value": "1915748352"<br />
									}<br />
								]<br />
							}<br />
						],<br />
						"items": [<br />
							{<br />
								"name": "dfs_ha_fencing_cloudera_manager_secret_key",<br />
								"value": "1sUUn8iD9xPPwTkMoPMwvDADggaMse"<br />
							},<br />
							{<br />
								"name": "dfs_namenode_acls_enabled",<br />
								"value": "true"<br />
							},<br />
							{<br />
								"name": "fc_authorization_secret_key",<br />
								"value": "G273Q1XUdXizE6kRNsXk6dmy36aSyh"<br />
							},<br />
							{<br />
								"name": "http_auth_signature_secret",<br />
								"value": "Lj3Er84290rJ5LhBfpQR3mSp44oBr6"<br />
							},<br />
							{<br />
								"name": "rm_dirty",<br />
								"value": "true"<br />
							},<br />
							{<br />
								"name": "zookeeper_service",<br />
								"value": "zookeeper"<br />
							}<br />
						]<br />
					},<br />
					"roles": [<br />
						{<br />
							"name": "hdfs-BALANCER-37e7e272139d6e22b92d52121b2fda18",<br />
							"type": "BALANCER",<br />
							"hostRef": {<br />
								"hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"<br />
							},<br />
							"config": {<br />
								"items": []<br />
							}<br />
						},<br />
						{<br />
							"name": "hdfs-DATANODE-96f12e9873efe5e716c4b969548788d3",<br />
							"type": "DATANODE",<br />
							"hostRef": {<br />
								"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "7wjjv1bmi05b90u1rmy55m1jm"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hdfs-DATANODE-9fe84b8104f1a573da9bd4e3e8761f2e",<br />
							"type": "DATANODE",<br />
							"hostRef": {<br />
								"hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "2iqjwq249t9l2zbkr42vj2b0r"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hdfs-DATANODE-f52dfe6a60fb35fe9f6327ea3faf1010",<br />
							"type": "DATANODE",<br />
							"hostRef": {<br />
								"hostId": "c0de22dc-2ddd-4449-a9bf-be89cb6646b7"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "2evy3gsih3tm46bl9bbjq7rdz"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hdfs-DATANODE-fc2f458838a9141f6c4972b92c876277",<br />
							"type": "DATANODE",<br />
							"hostRef": {<br />
								"hostId": "d3e1ba3b-ead8-45fe-a393-7d3b6bb84d82"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "8x7y3ez2k2mfgi18zen8imvtd"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hdfs-FAILOVERCONTROLLER-37e7e272139d6e22b92d52121b2fda18",<br />
							"type": "FAILOVERCONTROLLER",<br />
							"hostRef": {<br />
								"hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "1lcqu2ffx7j5yu7wy8vik9kft"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hdfs-FAILOVERCONTROLLER-9fe84b8104f1a573da9bd4e3e8761f2e",<br />
							"type": "FAILOVERCONTROLLER",<br />
							"hostRef": {<br />
								"hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "f14v0dfgxexipnunhynxzsnzl"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hdfs-HTTPFS-9fe84b8104f1a573da9bd4e3e8761f2e",<br />
							"type": "HTTPFS",<br />
							"hostRef": {<br />
								"hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "57w7cfh8jrsbr3ftjyfl76mjr"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hdfs-JOURNALNODE-37e7e272139d6e22b92d52121b2fda18",<br />
							"type": "JOURNALNODE",<br />
							"hostRef": {<br />
								"hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "7egeotk391l2bf94mlg7dsgjx"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hdfs-JOURNALNODE-9fe84b8104f1a573da9bd4e3e8761f2e",<br />
							"type": "JOURNALNODE",<br />
							"hostRef": {<br />
								"hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "1v7vkg7diby3umyehv5u1go89"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hdfs-JOURNALNODE-fc2f458838a9141f6c4972b92c876277",<br />
							"type": "JOURNALNODE",<br />
							"hostRef": {<br />
								"hostId": "d3e1ba3b-ead8-45fe-a393-7d3b6bb84d82"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "97f4rqj0pnccjbt49st6w5ive"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hdfs-NAMENODE-37e7e272139d6e22b92d52121b2fda18",<br />
							"type": "NAMENODE",<br />
							"hostRef": {<br />
								"hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "autofailover_enabled",<br />
										"value": "true"<br />
									},<br />
									{<br />
										"name": "dfs_federation_namenode_nameservice",<br />
										"value": "nameservice1"<br />
									},<br />
									{<br />
										"name": "dfs_namenode_quorum_journal_name",<br />
										"value": "nameservice1"<br />
									},<br />
									{<br />
										"name": "namenode_id",<br />
										"value": "162"<br />
									},<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "arjhpga3v62zw8yq3jivxu8ms"<br />
									}<br />
								]<br />
							}<br />
						},<br />
						{<br />
							"name": "hdfs-NAMENODE-9fe84b8104f1a573da9bd4e3e8761f2e",<br />
							"type": "NAMENODE",<br />
							"hostRef": {<br />
								"hostId": "9d54f582-4362-4488-8f65-219d4a33ed33"<br />
							},<br />
							"config": {<br />
								"items": [<br />
									{<br />
										"name": "autofailover_enabled",<br />
										"value": "true"<br />
									},<br />
									{<br />
										"name": "dfs_federation_namenode_nameservice",<br />
										"value": "nameservice1"<br />
									},<br />
									{<br />
										"name": "dfs_namenode_quorum_journal_name",<br />
										"value": "nameservice1"<br />
									},<br />
									{<br />
										"name": "namenode_id",<br />
										"value": "172"<br />
									},<br />
									{<br />
										"name": "role_jceks_password",<br />
										"value": "9rs6h5f3h2fmd3c2n57i0eldu"<br />
									}<br />
								]<br />
							}<br />
						}<br />
					],<br />
					"displayName": "HDFS"<br />
				}<br />
			]<br />
		}<br />
	],<br />
	"hosts": [<br />
		{<br />
			"hostId": "e22df64c-e53b-43e3-b8fb-79f3dec81d59",<br />
			"ipAddress": "172.31.17.222",<br />
			"hostname": "ip-172-31-17-222.ap-southeast-1.compute.internal",<br />
			"rackId": "/default",<br />
			"config": {<br />
				"items": []<br />
			}<br />
		},<br />
		{<br />
			"hostId": "9d54f582-4362-4488-8f65-219d4a33ed33",<br />
			"ipAddress": "172.31.23.18",<br />
			"hostname": "ip-172-31-23-18.ap-southeast-1.compute.internal",<br />
			"rackId": "/default",<br />
			"config": {<br />
				"items": []<br />
			}<br />
		},<br />
		{<br />
			"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc",<br />
			"ipAddress": "172.31.28.220",<br />
			"hostname": "ip-172-31-28-220.ap-southeast-1.compute.internal",<br />
			"rackId": "/default",<br />
			"config": {<br />
				"items": []<br />
			}<br />
		},<br />
		{<br />
			"hostId": "d3e1ba3b-ead8-45fe-a393-7d3b6bb84d82",<br />
			"ipAddress": "172.31.28.41",<br />
			"hostname": "ip-172-31-28-41.ap-southeast-1.compute.internal",<br />
			"rackId": "/default",<br />
			"config": {<br />
				"items": []<br />
			}<br />
		},<br />
		{<br />
			"hostId": "c0de22dc-2ddd-4449-a9bf-be89cb6646b7",<br />
			"ipAddress": "172.31.28.50",<br />
			"hostname": "ip-172-31-28-50.ap-southeast-1.compute.internal",<br />
			"rackId": "/default",<br />
			"config": {<br />
				"items": []<br />
			}<br />
		}<br />
	],<br />
	"users": [<br />
		{<br />
			"name": "__cloudera_internal_user__hue-HUE_SERVER-96f12e9873efe5e716c4b969548788d3",<br />
			"roles": [<br />
				"ROLE_NAVIGATOR_ADMIN"<br />
			],<br />
			"pwHash": "84a110feb17713a180cbc30f0eb85b101b5e657a1fb6b2d23e5f107794918249",<br />
			"pwSalt": 4617898858791690637,<br />
			"pwLogin": true<br />
		},<br />
		{<br />
			"name": "__cloudera_internal_user__mgmt-ACTIVITYMONITOR-96f12e9873efe5e716c4b969548788d3",<br />
			"roles": [<br />
				"ROLE_USER"<br />
			],<br />
			"pwHash": "926f60ce1ba3728def271715cefa831aa9e99a5b57a488887df13bed4cbd1571",<br />
			"pwSalt": 3756777870399121384,<br />
			"pwLogin": true<br />
		},<br />
		{<br />
			"name": "__cloudera_internal_user__mgmt-EVENTSERVER-96f12e9873efe5e716c4b969548788d3",<br />
			"roles": [<br />
				"ROLE_USER"<br />
			],<br />
			"pwHash": "16a28f0767fcf6eac17624fddc8ee0dd2c1eab43b1dedac2f21c7fddeaaf3e25",<br />
			"pwSalt": -7338933284551352999,<br />
			"pwLogin": true<br />
		},<br />
		{<br />
			"name": "__cloudera_internal_user__mgmt-HOSTMONITOR-96f12e9873efe5e716c4b969548788d3",<br />
			"roles": [<br />
				"ROLE_USER"<br />
			],<br />
			"pwHash": "e40dbc0cb57397d6f2aa99c84d280d9e952bf5120fc29b1e50d97bf481329594",<br />
			"pwSalt": -8368346909352992251,<br />
			"pwLogin": true<br />
		},<br />
		{<br />
			"name": "__cloudera_internal_user__mgmt-NAVIGATOR-96f12e9873efe5e716c4b969548788d3",<br />
			"roles": [<br />
				"ROLE_USER"<br />
			],<br />
			"pwHash": "25e9697deaf489d7bc25edbb561b298ef4cb0886ea39c0c778250acf6333bd7a",<br />
			"pwSalt": 3669424674689533297,<br />
			"pwLogin": true<br />
		},<br />
		{<br />
			"name": "__cloudera_internal_user__mgmt-NAVIGATORMETASERVER-96f12e9873efe5e716c4b969548788d3",<br />
			"roles": [<br />
				"ROLE_ADMIN"<br />
			],<br />
			"pwHash": "90e151656f0183809edf4942fc579dca47be452354fedcba9ae045ca1532a91d",<br />
			"pwSalt": 5488732577907527515,<br />
			"pwLogin": true<br />
		},<br />
		{<br />
			"name": "__cloudera_internal_user__mgmt-REPORTSMANAGER-96f12e9873efe5e716c4b969548788d3",<br />
			"roles": [<br />
				"ROLE_USER"<br />
			],<br />
			"pwHash": "93caddc90eb7c21114759a4d03704b4d278e44f395d39f36bd7ba955011ca4ea",<br />
			"pwSalt": -4978520779599535087,<br />
			"pwLogin": true<br />
		},<br />
		{<br />
			"name": "__cloudera_internal_user__mgmt-SERVICEMONITOR-96f12e9873efe5e716c4b969548788d3",<br />
			"roles": [<br />
				"ROLE_USER"<br />
			],<br />
			"pwHash": "72c561d0f3e488c54340d09274f49bdcfa01a2d4f95a44cb7f1cd002efa96369",<br />
			"pwSalt": 4895842479454989859,<br />
			"pwLogin": true<br />
		},<br />
		{<br />
			"name": "admin",<br />
			"roles": [<br />
				"ROLE_LIMITED"<br />
			],<br />
			"pwHash": "68107b6961cbf4a0953cc031caffaf3aa069abd041d0f96a4c0bed38930a4f8f",<br />
			"pwSalt": -8570728715721155791,<br />
			"pwLogin": true<br />
		},<br />
		{<br />
			"name": "minotaur",<br />
			"roles": [<br />
				"ROLE_CONFIGURATOR"<br />
			],<br />
			"pwHash": "d5e7f682050a8d1fb184424d2fd6a8cab3a6fb6cab02c1606f5adc13eadabbe7",<br />
			"pwSalt": -6633181738536505671,<br />
			"pwLogin": true<br />
		},<br />
		{<br />
			"name": "mwira",<br />
			"roles": [<br />
				"ROLE_ADMIN"<br />
			],<br />
			"pwHash": "e6e1c10139bf22993a0a87e4cf3a273e0899927b16750d1bfa473e433ac5bab4",<br />
			"pwSalt": -3607734412307643475,<br />
			"pwLogin": true<br />
		}<br />
	],<br />
	"versionInfo": {<br />
		"version": "5.14.3",<br />
		"buildUser": "jenkins",<br />
		"buildTimestamp": "20180414-0409",<br />
		"gitHash": "7f2725eea4edeb1d184a2888db790d332167b6f8",<br />
		"snapshot": false<br />
	},<br />
	"managementService": {<br />
		"name": "mgmt",<br />
		"type": "MGMT",<br />
		"config": {<br />
			"roleTypeConfigs": [<br />
				{<br />
					"roleType": "ACTIVITYMONITOR",<br />
					"items": [<br />
						{<br />
							"name": "firehose_database_host",<br />
							"value": "ip-172-31-28-220.ap-southeast-1.compute.internal"<br />
						},<br />
						{<br />
							"name": "firehose_database_name",<br />
							"value": "amon"<br />
						},<br />
						{<br />
							"name": "firehose_database_password",<br />
							"value": "amon_password"<br />
						},<br />
						{<br />
							"name": "firehose_database_user",<br />
							"value": "amon"<br />
						}<br />
					]<br />
				},<br />
				{<br />
					"roleType": "HOSTMONITOR",<br />
					"items": [<br />
						{<br />
							"name": "firehose_non_java_memory_bytes",<br />
							"value": "1533018112"<br />
						}<br />
					]<br />
				},<br />
				{<br />
					"roleType": "NAVIGATOR",<br />
					"items": [<br />
						{<br />
							"name": "navigator_database_host",<br />
							"value": "ip-172-31-28-220.ap-southeast-1.compute.internal"<br />
						},<br />
						{<br />
							"name": "navigator_database_name",<br />
							"value": "navms"<br />
						},<br />
						{<br />
							"name": "navigator_database_password",<br />
							"value": "navms_password"<br />
						},<br />
						{<br />
							"name": "navigator_database_user",<br />
							"value": "navms"<br />
						}<br />
					]<br />
				},<br />
				{<br />
					"roleType": "NAVIGATORMETASERVER",<br />
					"items": [<br />
						{<br />
							"name": "nav_metaserver_database_host",<br />
							"value": "ip-172-31-28-220.ap-southeast-1.compute.internal"<br />
						},<br />
						{<br />
							"name": "nav_metaserver_database_name",<br />
							"value": "nav"<br />
						},<br />
						{<br />
							"name": "nav_metaserver_database_password",<br />
							"value": "nav_password"<br />
						},<br />
						{<br />
							"name": "nav_metaserver_database_user",<br />
							"value": "nav"<br />
						},<br />
						{<br />
							"name": "navigator_heapsize",<br />
							"value": "1179648000"<br />
						}<br />
					]<br />
				},<br />
				{<br />
					"roleType": "REPORTSMANAGER",<br />
					"items": [<br />
						{<br />
							"name": "headlamp_database_host",<br />
							"value": "ip-172-31-28-220.ap-southeast-1.compute.internal"<br />
						},<br />
						{<br />
							"name": "headlamp_database_name",<br />
							"value": "rman"<br />
						},<br />
						{<br />
							"name": "headlamp_database_password",<br />
							"value": "rman_password"<br />
						},<br />
						{<br />
							"name": "headlamp_database_user",<br />
							"value": "rman"<br />
						}<br />
					]<br />
				},<br />
				{<br />
					"roleType": "SERVICEMONITOR",<br />
					"items": [<br />
						{<br />
							"name": "firehose_non_java_memory_bytes",<br />
							"value": "1533018112"<br />
						}<br />
					]<br />
				}<br />
			],<br />
			"items": []<br />
		},<br />
		"roles": [<br />
			{<br />
				"name": "mgmt-ACTIVITYMONITOR-96f12e9873efe5e716c4b969548788d3",<br />
				"type": "ACTIVITYMONITOR",<br />
				"hostRef": {<br />
					"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
				},<br />
				"config": {<br />
					"items": [<br />
						{<br />
							"name": "role_jceks_password",<br />
							"value": "f4cnxqtjt8dnaaw41imx5lyp7"<br />
						}<br />
					]<br />
				}<br />
			},<br />
			{<br />
				"name": "mgmt-ALERTPUBLISHER-96f12e9873efe5e716c4b969548788d3",<br />
				"type": "ALERTPUBLISHER",<br />
				"hostRef": {<br />
					"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
				},<br />
				"config": {<br />
					"items": [<br />
						{<br />
							"name": "role_jceks_password",<br />
							"value": "4cz15kkx7djhns0wabheca5q"<br />
						}<br />
					]<br />
				}<br />
			},<br />
			{<br />
				"name": "mgmt-EVENTSERVER-96f12e9873efe5e716c4b969548788d3",<br />
				"type": "EVENTSERVER",<br />
				"hostRef": {<br />
					"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
				},<br />
				"config": {<br />
					"items": [<br />
						{<br />
							"name": "role_jceks_password",<br />
							"value": "5sy9ylhey1o3d3bcnv3geo1z3"<br />
						}<br />
					]<br />
				}<br />
			},<br />
			{<br />
				"name": "mgmt-HOSTMONITOR-96f12e9873efe5e716c4b969548788d3",<br />
				"type": "HOSTMONITOR",<br />
				"hostRef": {<br />
					"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
				},<br />
				"config": {<br />
					"items": [<br />
						{<br />
							"name": "role_jceks_password",<br />
							"value": "26fizrink8t8ewjynjxrc94y4"<br />
						}<br />
					]<br />
				}<br />
			},<br />
			{<br />
				"name": "mgmt-NAVIGATOR-96f12e9873efe5e716c4b969548788d3",<br />
				"type": "NAVIGATOR",<br />
				"hostRef": {<br />
					"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
				},<br />
				"config": {<br />
					"items": [<br />
						{<br />
							"name": "role_jceks_password",<br />
							"value": "eo8esq9uma3jkzte5qovgl2hq"<br />
						}<br />
					]<br />
				}<br />
			},<br />
			{<br />
				"name": "mgmt-NAVIGATORMETASERVER-96f12e9873efe5e716c4b969548788d3",<br />
				"type": "NAVIGATORMETASERVER",<br />
				"hostRef": {<br />
					"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
				},<br />
				"config": {<br />
					"items": [<br />
						{<br />
							"name": "role_jceks_password",<br />
							"value": "1lju26kz7u3zb16ovezr55yk4"<br />
						}<br />
					]<br />
				}<br />
			},<br />
			{<br />
				"name": "mgmt-REPORTSMANAGER-96f12e9873efe5e716c4b969548788d3",<br />
				"type": "REPORTSMANAGER",<br />
				"hostRef": {<br />
					"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
				},<br />
				"config": {<br />
					"items": [<br />
						{<br />
							"name": "role_jceks_password",<br />
							"value": "3o4jqzx98kev3ql51cs4fp33w"<br />
						}<br />
					]<br />
				}<br />
			},<br />
			{<br />
				"name": "mgmt-SERVICEMONITOR-96f12e9873efe5e716c4b969548788d3",<br />
				"type": "SERVICEMONITOR",<br />
				"hostRef": {<br />
					"hostId": "970e107b-a435-4cfd-a7ca-0809a60530bc"<br />
				},<br />
				"config": {<br />
					"items": [<br />
						{<br />
							"name": "role_jceks_password",<br />
							"value": "bfjufyqfjpj3cq70ye8o9pc10"<br />
						}<br />
					]<br />
				}<br />
			}<br />
		],<br />
		"displayName": "Cloudera Management Service"<br />
	},<br />
	"managerSettings": {<br />
		"items": [<br />
			{<br />
				"name": "CLUSTER_STATS_START",<br />
				"value": "10/27/2012 18:10"<br />
			},<br />
			{<br />
				"name": "PUBLIC_CLOUD_STATUS",<br />
				"value": "ON_PUBLIC_CLOUD"<br />
			},<br />
			{<br />
				"name": "REMOTE_PARCEL_REPO_URLS",<br />
				"value": "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,http://archive.cloudera.com/kudu/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"<br />
			}<br />
		]<br />
	}<br />
}<br />
