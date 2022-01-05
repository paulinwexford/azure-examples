# Java on Azure Examples

This GitHub repository contains a set of Azure examples specifically for Java developers to quickly get started with Azure.
Please use the issue tracker to leave feedback, file issues or to propose other examples.

## Getting started

To work with these examples it is assumed you have the Azure CLI installed, and you have logged in and set your default subscription.
If you haven't done so follow the steps below.

_Note: Logging in and setting your default subscription needs to be done once per terminal session._

### Install Azure CLI

To setup the Azure CLI, please visit [Install the Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli).
And once you are done come back to this README.

### Login into Azure

<!-- workflow.skip() -->
````shell
  az login
````

### Set your default subscription

Get a list of your subscriptions (notice the `refresh` parameter that retrieves up-to-date subscriptions from the server) :

<!-- workflow.skip() -->
````shell
  az account list --output table --refresh
````

Set your default subscription for this session using the subscription id from the previous output:

<!-- workflow.skip() -->
````shell
  az account set --subscription "subscription-id"
````

<!-- workflow.run() 
exit 0
  -->

## Analytics

### Azure Data Explorer examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Create a database](analytics/adx/create-database/README.md) | [Workflow](.github/workflows/analytics_adx_create-database_README_md.yml) | ![adx/create-database/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/adx/create-database/README.md/badge.svg)
| 2. [Create a table](analytics/adx/create-table/README.md) | [Workflow](.github/workflows/analytics_adx_create-table_README_md.yml) |
| 3. [Create an Azure Data Explorer cluster](analytics/adx/create/README.md) | [Workflow](.github/workflows/analytics_adx_create_README_md.yml) | ![adx/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/adx/create/README.md/badge.svg)
| 4. [Ingest Client](analytics/adx/ingest-client/README.md) | [Workflow](.github/workflows/analytics_adx_ingest-client_README_md.yml) |

### Azure Event Hubs examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Create an event hub](analytics/eventhubs/create-eventhub/README.md) | [Workflow](.github/workflows/analytics_eventhubs_create-eventhub_README_md.yml) |  [![eventhubs/create-eventhub/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/eventhubs_create-eventhub_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/eventhubs_create-eventhub_README_md.yml)
| 2. [Create a namespace](analytics/eventhubs/create-namespace/README.md) | [Workflow](.github/workflows/analytics_eventhubs_create-namespace_README_md.yml) | [![eventhubs/create-namespace/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/eventhubs_create-namespace_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/eventhubs_create-namespace_README_md.yml)
| 3. [Receive an event](analytics/eventhubs/receive-event/README.md) | [Workflow](.github/workflows/analytics_eventhubs_receive-event_README_md.yml) |  [![eventhubs/receive-event/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/eventhubs_receive-event_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/eventhubs_receive-event_README_md.yml)
| 4. [Send an event](analytics/eventhubs/send-event/README.md) | [Workflow](.github/workflows/analytics_eventhubs_send-event_README_md.yml) | [![eventhubs/send-event/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/eventhubs_send-event_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/eventhubs_send-event_README_md.yml)

## Compute

### Azure App Service examples

| Name | Link | Status
| ---- | ---- | ------ 
| 1. [Create a deployment slot](compute/appservice/create-deployment-slot/README.md) | [Workflow](.github/workflows/compute_appservice_create-deployment-slot_README_md.yml) | [![appservice/create-deployment-slot/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_create-deployment-slot_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_create-deployment-slot_README_md.yml)
| 2. [Create an App Service Plan](compute/appservice/create-plan/README.md) | [Workflow](.github/workflows/compute_appservice_create-plan_README_md.yml) | ![appservice/create-plan/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/appservice/create-plan/README.md/badge.svg)
| 3. [Delete an App Service Plan](compute/appservice/delete-plan/README.md) | [Workflow](.github/workflows/compute_appservice_delete-plan_README_md.yml) | ![appservice/delete-plan/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/appservice/delete-plan/README.md/badge.svg)
| 4. [Delete your web application](compute/appservice/delete-webapp/README.md) | [Workflow](.github/workflows/compute_appservice_delete-webapp_README_md.yml) | [![appservice/delete-webapp/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_delete-webapp_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_delete-webapp_README_md.yml)
| 5. [Deploy to a deployment slot](compute/appservice/deploy-to-deployment-slot/README.md) | [Workflow](.github/workflows/compute_appservice_deploy-to-deployment-slot_README_md.yml) | [![appservice/deploy-to-deployment-slot/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_deploy-to-deployment-slot_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_deploy-to-deployment-slot_README_md.yml)
| 6. [Deploy Glassfish using a Docker image](compute/appservice/docker-glassfish/README.md) | [Workflow](.github/workflows/compute_appservice_docker-glassfish_README_md.yml) | [![appservice/docker-glassfish/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_docker-glassfish_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_docker-glassfish_README_md.yml)
| 7. [Deploy a GraalVM application using a Docker image](compute/appservice/docker-graalvm/README.md) | [Workflow](.github/workflows/compute_appservice_docker-graalvm_README_md.yml) | [![appservice/docker-graalvm/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_docker-graalvm_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_docker-graalvm_README_md.yml)
| 8. [Deploy Jetty using a Docker image](compute/appservice/docker-jetty/README.md) | [Workflow](.github/workflows/compute_appservice_docker-jetty_README_md.yml) | [![appservice/docker-jetty/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_docker-jetty_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_docker-jetty_README_md.yml)
| 9. [Deploy Payara using a Docker image](compute/appservice/docker-payara/README.md) | [Workflow](.github/workflows/compute_appservice_docker-payara_README_md.yml) | [![appservice/docker-payara/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_docker-payara_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_docker-payara_README_md.yml)
| 10. [Deploy Tomcat using a Docker image](compute/appservice/docker-tomcat/README.md) | [Workflow](.github/workflows/compute_appservice_docker-tomcat_README_md.yml) | [![appservice/docker-tomcat/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_docker-tomcat_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_docker-tomcat_README_md.yml)
| 11. [Deploy WildFly using a Docker image](compute/appservice/docker-wildfly/README.md) | [Workflow](.github/workflows/compute_appservice_docker-wildfly_README_md.yml) | [![appservice/docker-wildfly/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_docker-wildfly_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_docker-wildfly_README_md.yml)
| 12. [Deploy a managed JavaSE Quarkus application](compute/appservice/javase-quarkus/README.md) | [Workflow](.github/workflows/compute_appservice_javase-quarkus_README_md.yml) | [![appservice/javase-quarkus/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_javase-quarkus_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_javase-quarkus_README_md.yml)
| 13. [Deploy a Spring Boot application using managed JavaSE](compute/appservice/javase-springboot/README.md) | [Workflow](.github/workflows/compute_appservice_javase-springboot_README_md.yml) | [![appservice/javase-springboot/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_javase-springboot_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_javase-springboot_README_md.yml)
| 14. [Deploy a web application on a managed JBoss EAP](compute/appservice/jboss-eap-helloworld/README.md) | [Workflow](.github/workflows/compute_appservice_jboss-eap-helloworld_README_md.yml) | [![appservice/jboss-eap-helloworld/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_jboss-eap-helloworld_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_jboss-eap-helloworld_README_md.yml)
| 15. [List your web applications](compute/appservice/list-webapp/README.md) | [Workflow](.github/workflows/compute_appservice_list-webapp_README_md.yml) | [![appservice/list-webapp/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_list-webapp_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_list-webapp_README_md.yml)
| 16. [Scale your App Service Plan manually](compute/appservice/scale-manually/README.md) | [Workflow](.github/workflows/compute_appservice_scale-manually_README_md.yml) | [![appservice/scale-manually/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_scale-manually_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_scale-manually_README_md.yml)
| 17. [Swap a deployment slot](compute/appservice/swap-deployment-slot/README.md) | [Workflow](.github/workflows/compute_appservice_swap-deployment-slot_README_md.yml) | [![appservice/swap-deployment-slot/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_swap-deployment-slot_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/appservice_swap-deployment-slot_README_md.yml)
| 18. [Deploy a web application on a managed Tomcat](compute/appservice/tomcat-helloworld/README.md) | [Workflow](.github/workflows/compute_appservice_tomcat-helloworld_README_md.yml) | ![appservice/tomcat-helloworld/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/appservice/tomcat-helloworld/README.md/badge.svg)

### Azure Functions examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Deploy a Cosmos DB output Function](compute/functions/cosmosdb-output/README.md) | [Workflow](.github/workflows/compute_functions_cosmosdb-output_README_md.yml) | [![functions/cosmosdb-output/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/functions_cosmosdb-output_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/functions_cosmosdb-output_README_md.yml)
| 2. [Install Azure Functions Core Tools](compute/functions/install-tools/README.md) | [Workflow](.github/workflows/compute_functions_install-tools_README_md.yml) | [![functions/install-tools/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/functions_install-tools_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/functions_install-tools_README_md.yml)
| 3. [Deploy a Java Function](compute/functions/java/README.md) | [Workflow](.github/workflows/compute_functions_java_README_md.yml) | [![functions/java/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/functions_java_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/functions_java_README_md.yml)

### Azure Spring Cloud examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Configure the Azure Spring Cloud Config Server](compute/spring-cloud/config-server/README.md) | [Workflow](.github/workflows/compute_spring-cloud_config-server_README_md.yml) | [![spring-cloud/config-server/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/spring-cloud_config-server_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/spring-cloud_config-server_README_md.yml)
| 3. [Create an Azure Spring Cloud](compute/spring-cloud/create/README.md) | [Workflow](.github/workflows/compute_spring-cloud_create_README_md.yml) | [![spring-cloud/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/spring-cloud_create_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/spring-cloud_create_README_md.yml)
| 3. [Deploy a Spring Boot application to Azure Spring Cloud](compute/spring-cloud/helloworld/README.md) | [Workflow](.github/workflows/compute_spring-cloud_helloworld_README_md.yml) | [![spring-cloud/helloworld/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/spring-cloud_helloworld_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/spring-cloud_helloworld_README_md.yml)

## Containers

### Azure Container Instances examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Deploy a Quarkus application](containers/aci/quarkus/README.md) | [Workflow](.github/workflows/containers_aci_quarkus_README_md.yml) | [![aci/quarkus/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aci_quarkus_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aci_quarkus_README_md.yml)
| 2. [Deploy Tomcat](containers/aci/tomcat/README.md) | [Workflow](.github/workflows/containers_aci_tomcat_README_md.yml) | [![aci/tomcat/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aci_tomcat_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aci_tomcat_README_md.yml)
| 3. [Deploy WildFly](containers/aci/wildfly/README.md) | [Workflow](.github/workflows/containers_aci_wildfly_README_md.yml) | [![aci/wildfly/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aci_wildfly_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aci_wildfly_README_md.yml)

### Azure Container Registry examples

| Name | Link | Status
| ---- | ---- | ------ 
| 1. [Create an 'acrpull' Service Principal](containers/acr/create-acrpull-service-principal/README.md) | [Workflow](.github/workflows/containers_acr_create-acrpull-service-principal_README_md.yml) | ![acr/create-acrpull-service-principal/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/acr/create-acrpull-service-principal/README.md/badge.svg)
| 2. [Create Maven settings.xml](containers/acr/create-settings-xml/README.md) | [Workflow](.github/workflows/containers_acr_create-settings-xml_README_md.yml) | ![acr/create-settings-xml/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/acr/create-settings-xml/README.md/badge.svg)
| 3. [Create an Azure Container registry](containers/acr/create/README.md) | [Workflow](.github/workflows/containers_acr_create_README_md.yml) | ![acr/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/acr/create/README.md/badge.svg)
| 4. [Push a Glassfish Docker image](containers/acr/glassfish/README.md) | [Workflow](.github/workflows/containers_acr_glassfish_README_md.yml) | ![acr/glassfish/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/acr/glassfish/README.md/badge.svg)
| 5. [Push a GraalVM Docker image](containers/acr/graalvm/README.md) | [Workflow](.github/workflows/containers_acr_graalvm_README_md.yml) | ![acr/graalvm/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/acr/graalvm/README.md/badge.svg)
| 6. [Push a Jetty Docker image](containers/acr/jetty/README.md) | [Workflow](.github/workflows/containers_acr_jetty_README_md.yml) | ![acr/jetty/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/acr/jetty/README.md/badge.svg)
| 7. [Push a Payara Docker image](containers/acr/payara/README.md) | [Workflow](.github/workflows/containers_acr_payara_README_md.yml) | ![acr/payara/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/acr/payara/README.md/badge.svg)
| 8. [Push a Quarkus Docker image](containers/acr/quarkus/README.md) | [Workflow](.github/workflows/containers_acr_quarkus_README_md.yml) | ![acr/quarkus/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/acr/quarkus/README.md/badge.svg)
| 9. [Push a Tomcat Docker image](containers/acr/tomcat/README.md) | [Workflow](.github/workflows/containers_acr_tomcat_README_md.yml) | ![acr/tomcat/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/acr/tomcat/README.md/badge.svg)
| 10. [Push a WildFly Docker image](containers/acr/wildfly/README.md) | [Workflow](.github/workflows/containers_acr_wildfly_README_md.yml) | ![acr/wildfly/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/acr/wildfly/README.md/badge.svg)

### Azure Kubernetes Service examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Create a Kube config file using admin access](containers/aks/create-kube-config/README.md) | [Workflow](.github/workflows/containers_aks_create-kube-config_README_md.yml) | [![aks/create-kube-config/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aks_create-kube-config_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aks_create-kube-config_README_md.yml)
| 2. [Create an Azure Kubernetes Service cluster](containers/aks/create/README.md) | [Workflow](.github/workflows/containers_aks_create_README_md.yml) | [![aks/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aks_create_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aks_create_README_md.yml)
| 3. [Deploy a Spring Boot application](containers/aks/springboot/README.md) | [Workflow](.github/workflows/containers_aks_springboot_README_md.yml) | [![aks/springboot/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aks_springboot_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aks_springboot_README_md.yml)
| 4. [Deploy Tomcat](containers/aks/tomcat/README.md) | [Workflow](.github/workflows/containers_aks_tomcat_README_md.yml) | [![aks/tomcat/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aks_tomcat_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aks_tomcat_README_md.yml)
| 5. [Update your cluster to use your Azure Container Registry](containers/aks/use-your-acr/README.md) | [Workflow](.github/workflows/containers_aks_use-your-acr_README_md.yml) | [![aks/use-your-acr/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aks_use-your-acr_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aks_use-your-acr_README_md.yml)
| 6. [Deploy WildFly](containers/aks/wildfly/README.md) | [Workflow](.github/workflows/containers_aks_wildfly_README_md.yml) | [![aks/wildfly/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aks_wildfly_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/aks_wildfly_README_md.yml)

### Azure Red Hat OpenShift examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Deploy an Azure Red Hat OpenShift cluster](containers/aro/create/README.md) | [Workflow](.github/workflows/containers_aro_create_README_md.yml) |

## Databases

### Azure Cosmos DB examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Create a SQL container](databases/cosmosdb/create-sql-container/README.md) | [Workflow](.github/workflows/databases_cosmosdb_create-sql-container_README_md.yml) | [![cosmosdb/create-sql-container/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/cosmosdb_create-sql-container_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/cosmosdb_create-sql-container_README_md.yml)
| 2. [Create a SQL database](databases/cosmosdb/create-sql-database/README.md) | [Workflow](.github/workflows/databases_cosmosdb_create-sql-database_README_md.yml) | [![cosmosdb/create-sql-database/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/cosmosdb_create-sql-database_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/cosmosdb_create-sql-database_README_md.yml)
| 3. [Create SQL leases container](databases/cosmosdb/create-sql-leases-container/README.md) | [Workflow](.github/workflows/databases_cosmosdb_create-sql-leases-container_README_md.yml) | [![cosmosdb/create-sql-leases-container/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/cosmosdb_create-sql-leases-container_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/cosmosdb_create-sql-leases-container_README_md.yml)
| 4. [Create an Azure Cosmos DB](databases/cosmosdb/create/README.md) | [Workflow](.github/workflows/databases_cosmosdb_create_README_md.yml) | [![cosmosdb/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/cosmosdb_create_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/cosmosdb_create_README_md.yml)
| 5. [Insert item into a SQL container](databases/cosmosdb/insert-item-into-sql-container/README.md) | [Workflow](.github/workflows/databases_cosmosdb_insert-item-into-sql-container_README_md.yml) | [![cosmosdb/insert-item-into-sql-container/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/cosmosdb_insert-item-into-sql-container_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/cosmosdb_insert-item-into-sql-container_README_md.yml)
| 6. [SQL Change Feed Processor](databases/cosmosdb/sql-change-feed-processor/README.md) | [Workflow](.github/workflows/databases_cosmosdb_sql-change-feed-processor_README_md.yml) | [![cosmosdb/sql-change-feed-processor/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/cosmosdb_sql-change-feed-processor_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/cosmosdb_sql-change-feed-processor_README_md.yml)

### Azure SQL Database examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Deploy an Azure SQL Database](databases/mssql/create/README.md) | [Workflow](.github/workflows/databases_mssql_create_README_md.yml) | [![mssql/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mssql_create_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mssql_create_README_md.yml)
| 2. [Get country information (JDBC client)](databases/mssql/get-country/README.md) | [Workflow](.github/workflows/databases_mssql_get-country_README_md.yml) | [![mssql/get-country/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mssql_get-country_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mssql_get-country_README_md.yml)
| 3. [Load your Azure SQL database with data](databases/mssql/load-your-mssql-database-with-data/README.md) | [Workflow](.github/workflows/databases_mssql_load-your-mssql-database-with-data_README_md.yml) | [![mssql/load-your-mssql-database-with-data/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mssql_load-your-mssql-database-with-data_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mssql_load-your-mssql-database-with-data_README_md.yml)
| 4. [Open Azure SQL server firewall to your IP address](databases/mssql/open-firewall-to-your-ip/README.md) | [Workflow](.github/workflows/databases_mssql_open-firewall-to-your-ip_README_md.yml) | [![mssql/open-firewall-to-your-ip/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mssql_open-firewall-to-your-ip_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mssql_open-firewall-to-your-ip_README_md.yml)

### Azure Database for MySQL examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Deploy an Azure Database for MySQL](databases/mysql/create/README.md) | [Workflow](.github/workflows/databases_mysql_create_README_md.yml) | [![mysql/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mysql_create_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mysql_create_README_md.yml)
| 2. [Get country information (JDBC client)](databases/mysql/get-country/README.md) | [Workflow](.github/workflows/databases_mysql_get-country_README_md.yml) | [![mysql/get-country/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mysql_get-country_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mysql_get-country_README_md.yml)
| 3. [Load your MySQL database with data](databases/mysql/load-your-mysql-database-with-data/README.md) | [Workflow](.github/workflows/databases_mysql_load-your-mysql-database-with-data_README_md.yml) | [![mysql/load-your-mysql-database-with-data/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mysql_load-your-mysql-database-with-data_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mysql_load-your-mysql-database-with-data_README_md.yml)
| 4. [Open MySQL server firewall to your IP address](databases/mysql/open-firewall-to-your-ip/README.md) | [Workflow](.github/workflows/mysql_open-databases_mysql_open-firewall-to-your-ip_README_md.yml) | [![mysql/open-firewall-to-your-ip/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mysql_open-firewall-to-your-ip_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/mysql_open-firewall-to-your-ip_README_md.yml)

### Azure Database for PostgreSQL examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Deploy an Azure Database for PostgreSQL](databases/postgresql/create/README.md) | [Workflow](.github/workflows/databases_postgresql_create_README_md.yml) | [![postgresql/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/postgresql_create_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/postgresql_create_README_md.yml)
| 2. [Get country information (JDBC client)](databases/postgresql/get-country/README.md) | [Workflow](.github/workflows/databases_postgresql_get-country_README_md.yml) | [![postgresql/get-country/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/postgresql_get-country_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/postgresql_get-country_README_md.yml)
| 3. [Load your PostgreSQL database with data](databases/postgresql/load-your-postgresql-database-with-data/README.md) | [Workflow](.github/workflows/databases_postgresql_load-your-postgresql-database-with-data_README_md.yml) | [![postgresql/load-your-postgresql-database-with-data/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/postgresql_load-your-postgresql-database-with-data_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/postgresql_load-your-postgresql-database-with-data_README_md.yml)
| 4. [Open PostgreSQL server firewall to your IP address](databases/postgresql/open-firewall-to-your-ip/README.md) | [Workflow](.github/workflows/databases_postgresql_open-firewall-to-your-ip_README_md.yml) | [![postgresql/open-firewall-to-your-ip/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/postgresql_open-firewall-to-your-ip_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/postgresql_open-firewall-to-your-ip_README_md.yml)

### Azure Cache for Redis examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Create an Azure Cache for Redis](databases/redis/create/README.md) | [Workflow](.github/workflows/databases_redis_create_README_md.yml) | ![redis/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/redis/create/README.md/badge.svg)

## General

### Azure Resource Group examples

| Name | Link | Status
| ---- | ---- | ------ 
| 1. [Create an Azure Resource Group](general/group/create/README.md) | [Workflow](.github/workflows/general_group_create_README_md.yml) | ![group/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/group/create/README.md/badge.svg)
| 2. [Delete an Azure Resource Group](general/group/delete/README.md) | [Workflow](.github/workflows/general_group_delete_README_md.yml) | ![group/delete/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/group/delete/README.md/badge.svg)

## Integration

### Azure Service Bus examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Create an Azure Service Bus Queue](integration/servicebus/create-queue/README.md) | [Workflow](.github/workflows/integration_servicebus_create-queue_README_md.yml) | [![servicebus/create-queue/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/servicebus_create-queue_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/servicebus_create-queue_README_md.yml)
| 2. [Create an Azure Service Bus](integration/servicebus/create/README.md) | [Workflow](.github/workflows/integration_servicebus_create_README_md.yml)  | [![servicebus/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/servicebus_create_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/servicebus_create_README_md.yml)
| 3. [Receive a JMS message](integration/servicebus/receive-jms-message/README.md) | [Workflow](.github/workflows/integration_servicebus_receive-jms-message_README_md.yml) | [![servicebus/receive-jms-message/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/servicebus_receive-jms-message_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/servicebus_receive-jms-message_README_md.yml)
| 4. [Receive a message](integration/servicebus/receive-message/README.md) | [Workflow](.github/workflows/integration_servicebus_receive-message_README_md.yml) | [![servicebus/receive-message/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/servicebus_receive-message_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/servicebus_receive-message_README_md.yml)
| 5. [Send a JMS message](integration/servicebus/send-jms-message/README.md) | [Workflow](.github/workflows/integration_servicebus_send-jms-message_README_md.yml) | [![servicebus/send-jms-message/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/servicebus_send-jms-message_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/servicebus_send-jms-message_README_md.yml)
| 6. [Send a message](integration/servicebus/send-message/README.md) | [Workflow](.github/workflows/integration_servicebus_send-message_README_md.yml) | [![servicebus/send-message/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/servicebus_send-message_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/servicebus_send-message_README_md.yml)

## Security

### Azure Key Vault examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Add a Secret](security/keyvault/add-secret/README.md) | [Workflow](.github/workflows/security_keyvault_add-secret_README_md.yml) | ![keyvault/add-secret/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/keyvault/add-secret/README.md/badge.svg)
| 2. [Create a self-signed certificate](security/keyvault/create-self-signed-certificate/README.md) | [Workflow](.github/workflows/security_keyvault_create-self-signed-certificate_README_md.yml) |
| 3. [Create an Azure Key Vault](security/keyvault/create/README.md) | [Workflow](.github/workflows/security_keyvault_create_README_md.yml) | ![keyvault/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/workflows/keyvault/create/README.md/badge.svg)
| 4. [Create a Spring Boot application with client-side mTLS](security/keyvault/spring-boot-mtls-client-side/README.md) | [Workflow](.github/workflows/security_keyvault_spring-boot-mtls-client-side_README_md.yml) |
| 5. [Create a Spring Boot application with server-side mTLS](security/keyvault/spring-boot-mtls-server-side/README.md) | [Workflow](.github/workflows/security_keyvault_spring-boot-mtls-server-side_README_md.yml) |
| 6. [Create a server-side SSL Spring Boot application](security/keyvault/spring-boot-ssl-server-side/README.md) | [Workflow](.github/workflows/security_keyvault_spring-boot-ssl-server-side_README_md.yml) |

## Storage

### Azure Storage examples

| Name | Link | Status
| ---- | ---- | ------
| 1. [Create an Azure Storage Account](storage/storage/create/README.md) | [Workflow](.github/workflows/storage_storage_create_README_md.yml) | [![storage/create/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/storage_create_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/storage_create_README_md.yml)
| 2. [Enabled static website hosting](storage/storage/enable-static-website/README.md) | [Workflow](.github/workflows/storage_storage_enable-static-website_README_md.yml) | [![storage/enable-static-website/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/storage_enable-static-website_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/storage_enable-static-website_README_md.yml)
| 3. [Upload files to static website](storage/storage/upload-files-to-static-website/README.md) | [Workflow](.github/workflows/storage_storage_upload-files-to-static-website_README_md.yml) | [![storage/upload-files-to-static-website/README.md](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/storage_upload-files-to-static-website_README_md.yml/badge.svg)](https://github.com/Azure-Samples/java-on-azure-examples/actions/workflows/storage_upload-files-to-static-website_README_md.yml)
