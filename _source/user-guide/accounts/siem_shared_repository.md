---
layout: article
title: Manage the shared SIEM Repository
permalink: /user-guide/accounts/shared_repository.html
flags:
  admin: true
  logzio-plan: pro
tags:
  - security
  - security-account
  - accounts
  - logz.io-security
  - siem
contributors:
  - yberlinger
---

## About the shared SIEM Repository 

Build, prepare, and test your security content in a single sub account, set it as the  as the shared SIEM Repository, and share the content in the Repository with your other SIEM accounts.

The Repository acts as a centralized resource for all your SIEM content. When you set up a shared Repository, you can configure your other SIEM accounts to pull dashboards, visualizations, saved searches, and [private security feeds](/user-guide/cloud-siem/private-feeds) from it. 

All new SIEM accounts automatically pull from the shared Repository: You can manually disable access to the shared Repository for any SIEM account.

When you change which account is defined as the Repository, by default, the change creates an automatic dependency for all the existing SIEM accounts. 

If you don't have a Repository set, the Repository status is grayed out, with a link to **Set repository account**. 

<!--WIP placeholder for shared Repository topic WIIFM  -->

### Set a shared Repository account
To define a Repository account, you must have at least two related Cloud SIEM accounts.

To configure the shared Repository, in **Settings > Manage accounts**, navigate to your Cloud SIEM Plan, and **Set repository account**.


![Set a shared SIEM Repository](https://dytvr9ot2sszz.cloudfront.net/logz-docs/accounts/repo_set-account.png)

Select an existing account to be the shared Repository account.
![Pick a designated Repo](https://dytvr9ot2sszz.cloudfront.net/logz-docs/accounts/repo_picklist.gif) 

Configure the accounts that can pull SIEM content from the shared Repository and **Save** or **Cancel** your change. 
![Set a shared SIEM Repository ](https://dytvr9ot2sszz.cloudfront.net/logz-docs/accounts/repo_dependent_accts.png)

After you set the Repository, it's flagged with the Repository icon <i class="li li-repository"></i> in the list of Security accounts, and the **Repository account** status changes to display the Repository name.  **<i class="li li-repository"></i>** <i class="li li-signal"></i>

![Configured account](https://dytvr9ot2sszz.cloudfront.net/logz-docs/accounts/repo_all_set.png)

<!--![repo icon](https://dytvr9ot2sszz.cloudfront.net/logz-docs/accounts/repo-icon.png) -->  




### Check account dependencies

Open the account details to check if the account is associated with a SIEM Repository. 


### Reset and replace a Repository

When you replace the SIEM Repository, you automatically create dependencies for all your other SIEM accounts: They will pull content from the new Repository unless you manually remove the dependency for the Repository.


### Set dependent accounts

[placeholder text]



### Private feeds in the shared Security Repository

Define a private feed once in your SIEM Repository and share it with the relevant Security accounts.


### Remove access to the Repository account

[placeholder ]


### Reset a Repository account

To change the status of a shared Repository to a regular Cloud SIEM account, use the Reset operation. Dependent accounts will no longer be able to pull content from the Repository.

![Reset the existing Repository account](https://dytvr9ot2sszz.cloudfront.net/logz-docs/accounts/repo_reset.png)

### Delete a Repository 

If your current Repository is set as the repository for other SIEM accounts, you must first reset it to remove the dependencies for the other SIEM accounts. Once the Repository status is removed, the account can be deleted.