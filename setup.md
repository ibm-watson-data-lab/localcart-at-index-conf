## Setup
***

The LocalCart scenarios are build on [IBM Cloud services](https://console.bluemix.net/catalog/), the [Watson Data Platform](https://www.ibm.com/analytics/us/en/watson-data-platform/) and third-party cloud storage services.

<img src="https://raw.githubusercontent.com/ibm-watson-data-lab/localcart-at-index-conf/master/images/localcart%20overview.png"></img>


Complete the following steps to get set up for the scenarios.

1. Login to the [Watson Data Platform](https://dataplatform.ibm.com) or sign up.

1. Provision the required Cloud services
    1. Open the Data Services page
        * Click [this link](https://dataplatform.ibm.com/data/services?target=data-services&context=analytics) or choose **Services** > **Data Services** from the main menu
    1. Provision the following data services (if you don't already have an instance provisioned)
       * Cloud Object Storage (Lite plan, which is free) [[Learn more about this service...]](https://console.bluemix.net/catalog/infrastructure/cloud-object-storage)
    1. Open the Compute Services page
        * Click [this link](https://dataplatform.ibm.com/data/services?target=compute-services&context=analytics) or choose **Services** > **Compute Services** from the main menu
    1. Provision the following compute services (if you don't already have an instance provisioned)
       * Apache Spark (Lite plan, which is free) [[Learn more about this service...]](https://console.bluemix.net/catalog/services/apache-spark)
       * Machine Learning (Lite, which is free) [[Learn more about this service...]](https://console.bluemix.net/catalog/services/machine-learning)
       * Streaming Analytics (Lite plan, which is free) [[Learn more about this service...]](https://console.bluemix.net/catalog/services/streaming-analytics)
       
1. Add the Data Catalog app to your Watson Data Platform
   * Click the avatar icon on the upper right hand side and choose **Add Other Apps**. Skip the next step if this option is not displayed. 
   * Choose the **Data Catalog Lite** plan, which is free. 
1. Create a project  
   * Click [this link](https://dataplatform.ibm.com/projects/new-project?context=analytics) or choose **Projects** > **View All Projects** from the main menu
   * Enter a name and select a Cloud Object Storage and Spark service instance. If no instances are available, add new ones.

1. Take note of the information for the shared Message Hub service, which distributes the events that drive some of the workshop scenarios
    * **Name**: `clickstream` 
    * **API key**: `4Xy7RHj24N8v96hBj6vphZVJspYfIh5uGRGFM2NywaHFM1El`
    * **Brokers**: `kafka02-prod01.messagehub.services.us-south.bluemix.net:9093,kafka01-prod01.messagehub.services.us-south.bluemix.net:9093,kafka04-prod01.messagehub.services.us-south.bluemix.net:9093,kafka03-prod01.messagehub.services.us-south.bluemix.net:9093,kafka05-prod01.messagehub.services.us-south.bluemix.net:9093`
    * **Username**: `4Xy7RHj24N8v96hB`
    * **Password**: `j6vphZVJspYfIh5uGRGFM2NywaHFM1El`


### Scenario: Static data analysis using Python, Apache Spark, and PixieDust

In the project add a new notebook from URL https://raw.github.ibm.com/ibm-watson-data-lab/localcart-at-index-conf/master/notebooks/localcart-scenario-two.ipynb?token=AAAf8J59ByGDthIm7JRkB_gBhegsz4c9ks5akFBQwA%3D%3D

### Scenario: Build a product recommendation engine

In the project add a new notebook from URL https://raw.github.ibm.com/ibm-watson-data-lab/localcart-at-index-conf/master/notebooks/localcart-scenario-three.ipynb?token=AAAf8H8dIsg1Z5OqJ-GRumG3VeEmbUTrks5akFAvwA%3D%3D

### Scenario: Build a revenue dashboard using PixieApps
In the project add a new notebook from URL https://raw.github.ibm.com/ibm-watson-data-lab/localcart-at-index-conf/master/notebooks/localcart-scenario-four.ipynb?token=AAAf8JvkrA0Xf0rUlN1uI2a34Y-DaGRJks5akE_5wA%3D%3D
