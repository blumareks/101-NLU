# 101-NLU
This is 101 workshop on Natural Language Understanding with Watson. If you like it give me a star.

## Intro
In the provided examples you will analyze text from web pages with  Watson Natural Language Understanding (NLU).
The NLU service can be used for advanced text analytics, including uncovering insights from structured and unstructured data, understanding sentiment and emotion, and interpreting multiple languages.

You can test the service here - [demo https://natural-language-understanding-demo.ng.bluemix.net/](https://natural-language-understanding-demo.ng.bluemix.net/)


# Example 1
The first simple example is based on the Node.red - the super simple way of coding by connecting programmable nodes.

## instructions for example 1
0. prerequisit:
- [IBM Cloud account](https://ibm.biz/BdZVYb)

1.	Open the following github repo: [NLU example in Node.Red](https://github.com/watson-developer-cloud/node-red-labs/tree/master/basic_examples/natural_language_understanding)
 
2. copy the flow:
``https://raw.githubusercontent.com/watson-developer-cloud/node-red-labs/master/basic_examples/natural_language_understanding/nlu_flow.json``

3. you need to instantiate the Node.Red boilerplate - look at the catalog - [node red boiler plate](https://console.bluemix.net/catalog/starters/node-red-starter)


4. import the flow to your Node.Red 
- you need to bind the NLU service to Node.Red
- you need to deploy the flow with the updated link

# Example 2
In this example you will analyze Hacker news by using the IBM Watson Natural Language Understanding service in the IBM Cloud. 

You will add the Watson service to the IBM Kitura web application to demonstrate how to add a new dimension to text analysis from Kitura.
You will use an existing Swift-based developer pattern (https://github.com/IBM/Hackernews-NLU) that installs Watson NLU and connects it to a popular news site, Hacker News, all running in Swift. 
This can be done in almost any language of your choice using Watson Developer Cloud SDKs - https://github.com/watson-developer-cloud - however this example runs in Swift.

## instructions for example 2
0. prerequisit:
- [IBM Cloud account](https://ibm.biz/BdZVYb)
- [IBM Cloud CLI: ibmcloud cli](https://console.bluemix.net/docs/cli/reference/bluemix_cli/get_started.html#getting-started)

You can test it here: https://hackernewsnlu-multilateral-pinweed.mybluemix.net/

1.	Clone the Hacker News-NLU repository from GitHub: 
``$ git clone https://github.com/IBM/Hackernews-NLU.git``

2.	Change the directory to the new repository and log in to IBM Cloud:
``$ cd Hackernews-NLU``
``$ bx api https://api.ng.bluemix.net`` 
``$ bx login –u your@ibmid.email.com -o org_name –s space_name``

If you have a federated ID, use the SSO option: 
``bx login -o org_name –s space_name –sso``

3.	Create the NLU service by using this prepared command: 
``$ Cloud-Scripts/services/services.sh``

4.	Deploy the app to IBM Cloud:
``$ bx app push``

5. When application starts you should be able to visit the provided URL to your application and run it

