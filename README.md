# 101-NLU
This is 101 workshop on Natural Language Understanding with Watson. If you like it give me a star.

##Intro
In this example you will analyze Hacker news by using the IBM Watson Natural Language Understanding service in the IBM Cloud. It is based on the code pattern: https://github.com/IBM/Hackernews-NLU

The Watson Natural Language Understanding (NLU) service can be used for advanced text analytics, including uncovering insights from structured and unstructured data, understanding sentiment and emotion, and interpreting multiple languages.

You will add the Watson service to the IBM Kitura web application to demonstrate how to add a new dimension to text analysis from Kitura.
You will use an existing Swift-based developer pattern (https://github.com/IBM/Hackernews-NLU) that installs Watson NLU and connects it to a popular news site, Hacker News, all running in Swift. 
This can be done in almost any language of your choice using Watson Developer Cloud SDKs - https://github.com/watson-developer-cloud - however this example runs in Swift.

##setup
0. prerequisit:
- IBM Cloud account
- IBM Cloud CLI: [ibmcloud cli](https://console.bluemix.net/docs/cli/reference/bluemix_cli/get_started.html#getting-started)

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

