# ICAPI-DataDog
Provides a simple integration script to push data from the Instaclustr Monitoring REST API to DataDog.

For detailed instructions on how to set up see: https://support.instaclustr.com/hc/en-us/articles/215566468


Please see https://www.instaclustr.com/support/documentation/announcements/instaclustr-open-source-project-status/ for Instaclustr support status of this project

## Prerequisites

Install Python and Pip

Install Datadog python client library

`pip install datadog`

## Configuration Examples

This folder contains JSON configuration examples of:
* Kafka (all Metrics)
* Kafka Topic Level Metrics (replace {topic} with your Kafka Topic)

## Field Explainations

* cluster_id: The Instaclustr cluster ID. Available from the cluster details page on the Instaclustr console
* metrics_list: A comma separated list of metrics to retrieve and pass to DataDog. For a full list of available metrics, see the Instaclustr monitoring API documentation (https://www.instaclustr.com/support/api-integrations/api-reference/monitoring-api/).
* dd_options: Your DataDog API key and Application key. Available from Integrations/APIs in the DataDog console (you may need to create a new app key).
* ic_options: Your Instaclustr user name and API key. These can be viewed under the Account/API Keys tab of the Instaclustr console.