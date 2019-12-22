# Business-App-Development-in-Dynamics-365-for-Non-programmers
Business App Development in Dynamics 365 for Non-programmers [Video], Packt Publishing

You are viewing a companion solution intended to be installed into a PowerApps/Dynamics environment Version 1710 (9.1.0.10743) online or later

In this file I have included several entities and sample apps that have features and components configured similarly to the video material.

This solution is a managed solution. All the entities are named with the affix sample for ease of identification when configuring areas such as the site map and using tools like advanced find.

Because this is a managed solution you will be able to easily uninstall it and the uninstallation process will remove all of the affected components and artifacts (entities, processes, etc).

####Included in the solution:

* Apps
  * "Sales"
    * This is the sales model-driven power app and contains entities and features similar what is seen in sections 2 and 3
  * "Canvas App sample"
    * This is a canvas app sample that contains entities and features similar to what is seen in sections 4 and 5
* Entities
  * Account Sample
    * This is a record intended to mimic the Account entity for sample purposes. It would represent a company or business
  * Contact Sample
    * This is a record intended to mimic the contact record and would represent a person
  * Lead Sample
    * This record is used to represent a lead record.
  * Service Sample
    * The service sample represents a complex property of a work order record which represents a service performed as part of a work order for a contact/account
  * Work Order Sample
    * The work order sample record represents a custom entity used to extend a standard common data service instance to fulfill a business need and process.
* Processes
  * Account Sample
  * Contact Sample
  * Lead Sample
    * "Lead Sample Business Process Flow"
      * This is the default business process flow similar to what is used in Section 3.4
  * Lead Sample Business Process Flow
    * RT - Lead Sample Business Process Flow - control sales stage
      * The sales stage used in the dashboard chart for leads included in this solution needs a value to group and sort the records appropriatly based on where the leads are in the Business Process Flow stage. Business process flows created for entities also create a special entity used to track the state of the process independantly from the record. This workflow monitors that special business process flow entity and keeps a value maintained on the related lead record so that the funnel will display and be grouped in a desired order and in real time.
  * Service Sample
    * RT - Service Sample - Set Account Sample from Work Order Sample
      * This is used to set a lookup for the Account Sample record on the Service Sample record. This is used as a "trick" to display the Service Sample records in the canvas app for the selected account. Within a canvas app you can only link one record set deep at the time of this writing. So the account sample record is related to the work order sample records and the work order sample records for the account sample are related to the service sample records. Because of this limitation service sample records need to be related to the account sample record and this workflow executes on the busines
  * Work Order Sample

####Not Included:
* Weather integration
  * The weather integration used in the related canvas app videos uses a personal developer account to access the 3rd party weather API. for this reason it is not included in the samples
* Flow / Power Automate
  * At the time of this writing Flow/Power Automate is undergoing many changes which have been effecting maps used in this course. Eventually automation features missing here but used in the course will be added. Please reach out with any questions or comments in the meantime.
* Camera Access
  * The camera access features of the canvas app were not migrated to this manage solution. They are easy to implement and there is no plan to add this feature into the sample solution. Please reach out with any questions or comments.

#### Installation
The following guide provided by Microsoft can explain the import solution process if needed: https://docs.microsoft.com/en-us/powerapps/maker/common-data-service/import-update-export-solutions

For questions, comments, or suggestions please contact me via twitter: https://twitter.com/stalkjimmy