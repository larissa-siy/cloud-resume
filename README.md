# cloud-resume
This is where I will track my progress with my cloud resume challenge

Here are the steps I followed for the Cloud Resume Challenge. 

Whilst it is not yet complete, it is an ongoing project and I intend to implement all these steps for the final product.

1. HTML - I coded my CV in HTML for format
2. CSS - styled with CSS.
3. Static Website - I deployed the CV online as an Azure Storage static website using the Azure Static Web App, use Azure Storage to store the files.
5. HTTPS - Use HTTPS on the Azure Storage website URL should for security - AzureCDN to helped with this. You can view my Static Website at: https://cloudresumechallenge1.z13.web.core.windows.net/
6. DNS - I am going to create a custom DNS domain name to the Azure CDN endpoint using Azure DNS.
7. Javascript - I am going to  include a visitor counter that displays how many people have accessed the site. I will need to write a bit of Javascript to make this happen.
8. Database - The visitor counter will need to retrieve and update its count in a database somewhere. I will use the Table API of Azure’s CosmosDB for this. The erverless capacity mode will ensure that I keep costs low.
9. 9. API - I will not communicate directly with CosmosDB from my Javascript code. Instead, I will need to create an API that accepts requests from my web app and communicates with the database. I am going to use Azure Functions with a HTTP trigger for this.
10. Python - The code I write in the Azure Functions will be in Python as it is a common language used in back-end programs and scripts – and its Azure SDK.
11. Tests - I will test my python code
12. Infrastructure as Code - Instead of configuring my API
resources (the Azure Function, the
CosmosDB) manually, I will define them in anAzure Resource Manager (ARM) template on a Consumption plan, which will save me a lot of time in the long run
13. Source Control - Instead of constantly updating my back-end API or my front-end website through VS Code, I want them to update automatically wheneverI make a change to the code using continuous integration and deployment, or CI/CD. Therefore I have created *this* a GitHub repository for my (front-end) code.
14. CI/CD (Front-end) - I have created this GitHub repository for my website code and will create GitHub Actions such that when I push new website code, the Azure Storage blob automatically gets updated.
15. CI/CD (Back-end) - I will create a second GitHub repository for my back-end code I will set up GitHub Actions such that when I push an update to my ARM template or Python code, my Python tests get run. If the tests pass, the ARM application should get packaged and deployed to Azure.


As of 24/04/2023 I am currently on step 6 of the process but I aim to be completed by the end of the month! 

Stay tuned.
