Write curl statements that stop, start, and check the current state of your Hive service.
Add these statements and their output to enterprise/labs/3_api_hive_state.md



Check Current State

<code>curl -u mwira:cloudera 'http://54.169.208.182:7180/api/v12/clusters/mwira/services/hive/'</code> <br/>
Output  
```json
{  
  "name" : "hive",  
  "type" : "HIVE",  
  "clusterRef" : {  
    "clusterName" : "cluster"  
  },  
  "serviceUrl" : "http://ip-172-31-28-220.ap-southeast-1.compute.internal:7180/cmf/serviceRedirect/hive",  
  "roleInstancesUrl" :   "http://ip-172-31-28-220.ap-southeast-1.compute.internal:7180/cmf/serviceRedirect/hive/instances",  
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
}
```

Stop Hive Services
<code>curl -X POST -u mwira:cloudera 'http://54.169.208.182:7180/api/v12/clusters/mwira/services/hive/commands/stop'</code>
Output  
```json
{
  "id" : 1583,
  "name" : "Stop",
  "startTime" : "2018-05-17T01:08:20.987Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```



Start Hive Services
<code>curl -X POST -u mwira:cloudera 'http://54.169.208.182:7180/api/v12/clusters/mwira/services/hive/commands/start'</code>

output  

```json
{
  "id" : 1587,
  "name" : "Start",
  "startTime" : "2018-05-17T01:10:06.163Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```
