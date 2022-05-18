# <img src="Media/Power%20app%20Logo.png" width="100" height="50">   Power Platform App in a Day 

Overview and Pre-requisites Hands-on Lab Step-by-Step
### Lab Overview and Pre-requisites
##### Abstract
This is a beginner level lab for you to get hands on experience with the [Microsoft Power Platform](https://powerplatform.microsoft.com/en-us/) technologies – [Power
Apps](https://powerapps.microsoft.com/en-in/), [Power Automate](https://powerplatform.microsoft.com/en-us/power-automate/), and [Microsoft Dataverse](https://powerplatform.microsoft.com/en-in/dataverse/). The lab includes step-by-step instructions for someone new to these
technologies to build a device ordering solution within a day. Technologies covered are:

**Power Apps:** A software as a service (SAAS) application platform that enables power users in line of business roles
to easily build and deploy custom business apps. You will learn how to build Canvas and Model-driven style of
apps.

**Power Automate:** A business service for line of business specialists and IT pros to build automated workflows
intuitively.

**Microsoft Dataverse:** Makes it easier to bring your data together and quickly create powerful apps using a
compliant and scalable data service and app platform that is integrated into Power Apps.
Make sure to follow all the pre-requisite steps listed in this document before starting the labs. Because the Power Platform
is a cloud-based solution, you can complete all labs remotely.
For a list of additional learning resources and introductory videos, see [Learning Resources](https://powerapps.microsoft.com/en-us/blog/microsoft-powerapps-learning-resources/)

## Lab Structure and Learning Objectives

The lab is divided into four modules, with one lab document provided for each module.

1. #### **01-Power Apps Canvas App Lab Manual:**

   Focuses on the basic concepts involved in building Power Apps Canvas apps. You will learn how to:
 
      • Connect to data sources and filter results based on specified criteria
  
      • Work with screens and navigation
   
      • Use controls, properties, formulas, and actions to customize the user experience
      
      • Display the logged in user’s name
      
      • Configure app settings
      
      • Save and share an app
      
      • Run an app on a mobile device.

2. #### **02- Microsoft Dataverse Lab Manual:**
    Introduces you to the Microsoft Dataverse. You will learn how to:
     
      • Create and customize a custom table
     
      • Use the Form control
    
      • Save data into the Microsoft Dataverse using the Form control.

3. #### **03-Power Apps Model-driven App Lab Manual:**
     Introduces you to building Model-driven Power Apps. You will learn how to:
     
      • Create a standalone Model-driven app.
       
      • Customize forms for the Model-driven app
     
      • Use a Business Process Flow to guide users through a process.
 

4. #### **04-Power Automate Lab Manual:**
   Introduces you to Power Automate. You will learn how to:
   
      • Create a flow that is triggered when a new Microsoft Dataverse row is created
  
      • Automate sending approval requests
  
      • Customize the approval based on the Microsoft Dataverse row
  
      • Use the Approval center
      
#### How to start a module without completing previous module(s)
The lab package includes a \ **Completed** folder which consists of a set of app packages. If you wish to start on a module
without having completed the previous module(s), you may import a partially built app package. See the corresponding
instructions in each of the subfolders within the “Completed” folder.

   • To directly start working on Module 2 -> see instructions in \Completed\Module1 subfolder

   • To directly start on Module 3 -> see instructions in \Completed\Module2 subfolder

   • To directly start on Module 4 -> see instructions in \Completed\Module3 subfolder

#### Pre-requisites: Before starting the hands-on labs

NOTE: To participate in this training, you require an internet connection, and you will use the web version of the Power
Apps Studio, which will run in a browser: Microsoft Edge, Google Chrome, or Safari.

### Task 1: Download the Lab Files
1. Download file [Lab Files](http://aka.ms/appinaday) (Copy Link)

2. **Save a local copy of the lab contents:** Download the **PAHandsOnLabContent.zip** file for the lab from [Lab Files](http://aka.ms/appinaday).
Save it to a local folder, such as C:\AppInADay. Extract the ZIP package. This package contains the sample data for the app, PDF copies of the lab manuals, and pre-built app packages.

### Task 2: Sign-in to Power Apps
<img src="Media/Causion.jpeg" width="40" height="30"> Find the group you most closely relate to below.

|Instructions|Steps|
| ---------------------------------------------  | --------------------------------------------------------- |
| You are in a classroom led by an instructor.   | Follow their direction for all environment set-up details |
| You are a licensed user of Microsoft products  | Follow step 1 below, and then proceed to the next task.  |
| You are starting from scratch with no licenses and no instructor.  | Follow step 2 below, and then proceed to the next task.  |
|You are a licensed user of Microsoft products, BUT your admin has policies in place to restrict your use of PowerApps|Follow step 2 below using a personal email account, and then proceed to the next task.|
|You are really not sure which of the above you are.|Follow step 2 below using  personal email account a private/incognito browsersession,and then proceed to next task.|

1. **Confirm that you are licensed to use Power Apps:** Go to [Make Power Apps](http://make.powerapps.com/) and sign-in with your business
or school account. This is the same as your Office 365 or Dynamics 365 login. Sign up for a free developer plan for
individual use, see [here](https://docs.microsoft.com/en-us/powerapps/maker/dev-community-plan). If you are not able to use Power Apps with your organizational credentials, you may review
the instructions for provisioning a demo tenant in the next step using a personal email.
2. **Start a trial of Power Apps:** Usage of Microsoft Dataverse requires a Power Apps premium
license. Go to [Power Apps Pricing](https://powerapps.microsoft.com/pricing) and select the “Try free” option to start a free 30-day trial. For more detailed
information on signing up for a free trial, see [here](https://docs.microsoft.com/en-us/powerapps/maker/signup-for-powerapps). Follow the prompts to set up your free trial of Power Apps.
a. You will also need to add a free trial of Office E3 and Power Automate per user. After you have the Power
Apps trial set-up, navigate to **admin.microsoft.com** and select **Purchase Services** from the left
navigation area of **Billing**.


b. Search for and select **Office E3.** Click **details.** Find and select **start your free trial.**

c.Search for and select **Power Automate per user** and **start your free trial.**

d. **Assign licenses** for each of these to your **Power Apps user.** Select Active Users from the left
navigation area of Users. Select your user, then select Licenses and Apps. Select the desired licenses and **Save
changes.** You may need to refresh your browser to see the changes take effect.

### Task 3: Install the Power Apps and Power Automate mobile applications (optional)
1. **Install the Power Apps mobile application:** Go to the app store on your mobile device. Search for **“Power
Apps”** and install the Power Apps mobile application. If prompted, keep push notifications enabled.
2. **Install the Power Automate mobile application:** Go to the app store on your mobile device. Search for **“Power
Automate”** and install the application. If prompted, keep push notifications enabled.

### Task 4: Create a new environment and Microsoft Dataverse database instance
If your environment is being provided for you, you can skip this task.

You must have a newly created Microsoft Dataverse environment and database instance, that was **created just for this
lab.** If you don’t have a new environment or have an older environment, follow the steps below to create the environment
and provision the database instance.

1. Open the Power Apps admin center by navigating to [Admin Power Apps](http://admin.powerapps.com/) in a web browser.

2. In the Admin center, select **Environments** and click **+New**
      
 3. Provide a name for the environment. A common practice is to use your name followed by “Test” so it is clear this
is a test environment.

4. Select **Trial**, select your **Region**, make sure **Create a database** is set to **Yes** , and click **Next.

5. Select your **Language** and your **Currency** . Check **Yes** for Deploy sample apps and data, and then click **Save**

**Note:** You can choose your local language and currency. However, the lab manuals were created using US dollars and
English language configurations.

6. You will see a screen listing all environments that will show the newly created environment.

7. **IMPORANT:** You need to wait for the database to finish provisioning before trying to create an application. The
**Status** will change to Ready when done.

8. This may take few minutes to complete. Wait for it to complete before proceeding with creating an app. If it has
been over two minutes, try refreshing the browser. Once the database has been created you should no longer see
this “Preparing Instance” message. You can then proceed with the lab.


Information in this document, including URL and other Internet Web site references, is subject to change without notice.
Unless otherwise noted, the example companies, organizations, products, domain names, e-mail addresses, logos, people,
places, and events depicted herein are fictitious, and no association with any real company, organization, product, domain
name, e-mail address, logo, person, place or event is intended or should be inferred. Complying with all applicable
copyright laws is the responsibility of the user. Without limiting the rights under copyright, no part of this document may
be reproduced, stored in or introduced into a retrieval system, or transmitted in any form or by any means (electronic,
mechanical, photocopying, recording, or otherwise), or for any purpose, without the express written permission of
Microsoft Corporation.
Microsoft may have patents, patent applications, trademarks, copyrights, or other intellectual property rights covering
subject matter in this document. Except as expressly provided in any written license agreement from Microsoft, the
furnishing of this document does not give you any license to these patents, trademarks, copyrights, or other intellectual
property.
The names of manufacturers, products, or URLs are provided for informational purposes only and Microsoft makes no
representations and warranties, either expressed, implied, or statutory, regarding these manufacturers or the use of the
products with any Microsoft technologies. The inclusion of a manufacturer or product does not imply endorsement of
Microsoft of the manufacturer or product. Links may be provided to third party sites. Such sites are not under the control
of Microsoft and Microsoft is not responsible for the contents of any linked site or any link contained in a linked site, or
any changes or updates to such sites. Microsoft is not responsible for webcasting or any other form of transmission
received from any linked site. Microsoft is providing these links to you only as a convenience, and the inclusion of any link
does not imply endorsement of Microsoft of the site or the products contained therein.
© 2022 Microsoft Corporation. All rights reserved.
Microsoft and the trademarks listed at https://www.microsoft.com/enus/legal/intellectualproperty/Trademarks/Usage/General.aspx are trademarks of the Microsoft group of companies. All
other trademarks are property of their respective owners.
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
  
