### Using the shared producer to generate clickstream events

To simplify the workshop environment a Shopping app event producer has been deployed in the workshop environment you are using. 
This producer simulates shopping events (such as users logging in, browsing items, adding items to the cart, etc) and sends them to a pre-provisioned Message Hub service instance that you have access to.
![shared producer setup](https://raw.githubusercontent.com/ibm-watson-data-lab/localcart-at-index-conf/master/images/shared_producer.png)

To capture these events use the Message Hub connectivity information (API key, broker URLs, username, password) that was provided to you.

### Using a dedicated producer to generate clickstream events

If desired (or if you don't have access to the shared producer) you can set up your own instance.

TODO instructions from https://github.com/wdp-beta/get-started/blob/master/notebooks/localcart-scenario-part-1.ipynb
