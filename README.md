# Apprenda for IBM Cloud Workshop
Apprenda and IBM have partnered together to provide an experience native and natural for the Microsoft and .NET community. The Apprenda Platform integration is built using IBM Cloud tooling and with tooling on the Microsoft platform.  This is critical to ensure the solution is a true integration and not a bolt-on or afterthought. The solution is fully self-service with seamless onboarding. It’s a deep and rich experience for .NET developers.

Before the Apprenda on IBM Cloud solution, customers might have considered rewriting everything they had from the past decade.  Now, they can leverage their expertise and quickly move over existing and new .NET applications and immediately take advantage of numerous cloud capabilities.  High-availability, scalability and the ability to seamlessly tap into the full range of IBM Cloud services are a few notable examples. 

This workshop will walk you through configuring, deploying and scaling a .NET application in Apprenda running on the IBM Cloud.  Then, for bonus points, you’ll enhance that app with a Watson Conversation enabled chatbot! 

It’s important to note that you will be using an HTML portal throughout the workshop, but you could just as easily, if not in most cases easier, take advantage of our REST API, CLI or Microsoft Visual Studio integration.  To take that a step further, you could use TFS or any CI/CD tool to automate steps like these in your CI/CD process.  This is important because it allows you to take all the benefits from the Apprenda and IBM Cloud solution without having to change the tools you use or process you’re accustomed to. 

#### This workshop will walk through the following steps:
1. **Part 1 – Upload and Deploy a .NET Application with Apprenda**
   - Upload .NET app using an Apprenda Archive	
   - Configure app’s Resource Policy
   - Promote app to Sandbox
   - App Configuration
2. **Part 2 – Configure Cloud Features: Monitoring, Scaling, Logging**
   - Monitoring
   - Update scaling strategy
   - Configure a Log Override
3. **Bonus – Integrate an IBM Watson Conversation enabled chatbot!**
   - Turn Watson Chat on
   - Promote application to Published 

## Prerequisites
### An IBM Cloud account  
The account requires an IBMid.  If you don’t have an IBMid, you can create one when you register.

### An Apprenda Platform account.  To create an account follow these steps:
#### 1.	Navigate to the IBM Cloud console
#### 2. Click Catalog
#### 3. Click Application Services 
#### 4. Click Apprenda Cloud Platform 
#### 5. Select the Standard Plan and Click Create
#### 6. Open the Apprenda portal link
#### 7. Create your account

## Part 1 – Upload and Deploy a .NET Application with Apprenda
### Upload .NET app using an Apprenda Archive 

#### 1.	Navigate to the Apprenda on IBM Cloud web portal: https://apps.bm.apprenda.com
#### 2.	Click **+New** button to open the application drawer and fill out a unique application name and description  
>You will notice the application alias is auto populated, you are able to change it if you like. (The alias is used by the platform to uniquely identify your application in the system and generate the URL used to access it.)
#### 3.	Click Select File to bring up a file explorer menu and locate the Apprenda archive in this repo
>**What is an Apprenda Archive?** Apprenda Archives are simply compressed ZIP (.zip) files that contain files organized in a pre-determined way. Apprenda uses this known structure to traverse the archive and extract information it uses to deploy your application. During the process of deployment, Apprenda first validates the contents of your archive against a set of rules that are designed to guarantee that your application will run properly on Apprenda in a secure and reliable fashion. Apprenda then extracts and catalogs your application’s files and resources and uses them as a foundation for serving your application to requesting Users.

>**What happens during upload?** During upload Apprenda will parse the archive structure to extract the various component tiers of your application and will statically analyze both the binaries and configuration of each to discover how your application components are related to one another. Apprenda creates a metadata map of your application that describes how the different tiers and components within tiers relate to one another. This map is useful to Apprenda in many different scenarios, including deployment and execution.  In fact, behind the scenes, Apprenda will use the same process when you deploy your app as well.

#### 4.	Finally select Save and Continue and Apprenda will upload the archive
>**What happens after upload?** After your archive is uploaded, parsed, and mapped Apprenda will create an application and place it in Definition Stage.  Then, you will be navigated to the Configure Tab of your application that Apprenda created.  This is where you can configure and enable different features of Apprenda for your app to take advantage of.  Configuration options include anything from features that help enable traditional applicaitons to function as a cloud enabled app to inject additional functionality like auth N/Z. 

>**What is Definition Stage?** This is one four stages:  Definition, Sandbox, Published, and Archived.  Each stage infers distinct characteristics about how your application is deployed and controls which operations can be conducted. We will learn more about the other stages as we progress through them.  For now, you can think of Definition as an app configuration stage, Sandbox as a deployed development/test stage and Published as a deployed production stage. The Definition stage is designed to allow you to provide information and configuration essential to the deployment of our application.  



#### Let’s move on to setting the amount of resource we want our app to have before we deploy it 

### Configure app’s Resource Policy
### Promote app to Sandbox

## Part 2 – Configure Cloud Features: Monitoring, Scaling, Logging

## Bonus – Integrate an IBM Watson Conversation enabled chatbot!

