
## Getting Started with IBM Blockchain on Bluemix

We have developed the [Hyperledger Fabric](https://github.com/hyperledger/fabric) into a service on Bluemix.  Provisioning an instance of this service gives you a small blockchain network consisting of two peers and one certificate authority server (CA).  You can then deploy and test your own smart contract code (chaincode) on this blockchain network and implement applications utilizing it.

Provisioning your own instance of the Bluemix service:
1. Find the service [in Bluemix](https://console.ng.bluemix.net/catalog/services/blockchain/).
2. Sign up for a Bluemix account and/or provision an instance.
![Catalog Page](https://github.com/IBM-Blockchain/getting-started/images/blockchain_catalog.png "Blockchain Bluemix Service Catalog Page")
3. After the service is created and you are taken to the service panel, view the credentials that were created for your service.  These credentials should be passed into the Blockchain SDK when you start building your blockchain application.
4. Open the monitoring dashboard for your service instance.
The monitoring dashboard you see should appear as shown below and have the tabs: Network, Live Logs, Blockchain, APIs, and Deploy.


## Getting Started with the Blockchain SDK
1. Find the [SDK documentation](https://github.com/hyperledger/fabric/tree/master/sdk/node). 
2. Read the documentation.  It will walk you through the process of initializing the SDK with connection information for your network and some information about the chaincode you want to deploy.  After that, you can deploy, invoke, and query you chaincode from whatever NodeJS application you want to build.

## Deploying your application to Bluemix
First, deploy your own instance of the [marbles demo](https://github.com/IBM-Blockchain/marbles).  It’s just a few clicks, and it will show you what it takes to get an application running on Bluemix.  After you have configured your app to run on Bluemix, deploying it from the command line is easy.  See, the marbles demo [manifest file](https://github.com/IBM-Blockchain/marbles/blob/master/manifest.yml), [app.js](https://github.com/IBM-Blockchain/marbles/blob/master/app.js), and [setup.js](https://github.com/IBM-Blockchain/marbles/blob/master/setup.js) in order to see how to configure a NodeJS application for Bluemix.  If reference documentation is more your style, see the [Cloud Foundry documentation](https://docs.cloudfoundry.org/devguide/deploy-apps/deploy-app.html) on deploying applications.

## Getting started with the Hyperledger Fabric
[Fabric](https://github.com/hyperledger/fabric) is a blockchain project in incubation that proposed to the community and documented [here](https://goo.gl/RYQZ5N) . Information on what incubation entails can be found in the [Hyperledger Project Lifecycle document](https://goo.gl/4edNRc).

The documentation around the Fabric changes as new features and enhancements are added to the Fabric.  Consider what you see there as the ultimate truth.  Here is a quick summary of what you need to do to run the Fabric code yourself:

1. Set up a development environment on your machine.  This will involve installing Go, Vagrant, and some other dependencies.  This environment will let you run a Hyperledger network on your local machine. 
2. Download, build, and test the Fabric code, just to make sure you set everything up correctly.
3. Create a blockchain network by starting and connecting some peers.
4. Deploy some example chaincode and play around with querying it and invoking transaction on it.
5. Learn how to write your own chaincode.
6. Build your own blockchain app!