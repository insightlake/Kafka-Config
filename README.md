What is InsightLake Kafka Config?
-----------

InsightLake Kafka Config solution for Kafka Cluster. It provides Export kafka component configuration and create Kafka component in kafka Cluster

User can get following component configuration
1)Topic </n>
2)Connectors </n>
3)Schema-Registry </n>

# Update your configuration files
You can use the supplied cluster.properties.example </n>

## Run the Jar
1)Download or clone project
2)form lib folder ther is executatble jar files </n>
### For Export 
Go to Export folder under lib folder run following command</n>
   
   java -cp edp-kafka-config-0.0.1-SNAPSHOT-jar-with-dependencies.jar com.insightlake.edp.config.app.ExportApp configFile=<Cluster Configuration file>/cluster.properties localPath=<LOCAL-FOLDER-PATH> tags=connectors,topics,schemas</n>
   
   configFile: provide your cluster configuration file</n>
   localPath: Provide path where you want to generate configuration</n>
   tags: connectors,topics,schemas you can provider multiple tag with comma separated</n>
   
### For Import
Go to Import folder under lib folder run following command</n>

java -cp edp-kafka-config-0.0.1-SNAPSHOT-jar-with-dependencies.jar com.insightlake.edp.config.app.ImportApp configFile=<Cluster Configuration file>/cluster.properties    componentFile=<Component-file-path> type=connectors </n>
   configFile: provide your cluster configuration file</n>
   localPath: Provide path where you want to generate configuration</n>
   tags: connectors,topics,schemas you can provider multiple tag with comma separated</n>







