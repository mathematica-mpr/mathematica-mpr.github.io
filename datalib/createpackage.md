# Creating packages

Consider packages as containers to store the datasets (a file or a collection of files) from different sources.  Tags, metadata added to packages help to catalog the datasets and make them discoverable, accessible to the project users in the library. You can create multiple packages to store different versions of the data or categories of data.

> Project system leads, project data users can create packages to ingest datasets. You can upload only one dataset file in a package.


#### To create a package: 

* Click **Create a Package** tab or the **Create Package** button in the Dashboard page.
    * Note that project System Leads are automatically directed to the package creation page when setting up a project in the library.
* Select the project number associated with the package. **Note that you can view and select the project numbers only for the projects you have access to.??**

#### Catalog the package:

* Enter the required fields to provide information on the package, such as the description of the dataset, focus area, data classification, data source. 
* We recommend you provide information for all the fields in the package creation page. Cataloging the packages allow for 
    * consistent way to categorize, locate the datasets using the Search feature.
    * view the list of datasets in the data library, and identify the datasets available to public, or are private.

* In the MVP implementation of the Data Library, only on-premise location works for uploading datasets. Though you see the different data source origin, select *On-prem* as the Data Source Origin.
* Note that Data Storage Status is at *loading* - this indicates 
* By default, the library assigns an initial version number to the package you create. Each time you update the package, you will need to provide a new Data Version Comment for the package.
* Click **Create Package**. You now see the package details in the Overview page and can add files and additional metadata to build the package contents.

<!--Add metadata:

* In the Overview tab where you see the package details, scroll down to the bottom, and click **Add Metadata**.
* Enter the tag name and value.
* Add as many metadata tags as needed.
* To edit an existing tag, select the tag/value and enter the new name/value.

-->

Add dataset file:

* To upload data file for the dataset, select the **Content** tab at the top of the package page.
* Click **Publish a local file**.
* Click the folder icon at the right to browse and upload the file. If you accidentally uploaded a wrong data file, click X next to the folder icon to cancel the file selected, then select the correct data file to upload. **Confirm**
* Next, you need to update the package version comment - select the Overview tab, enter a comment of the file upload in the Data Version Comment textbox.
* Click **Save** at the top of the page to save uploading the file and the version comment. 
* You will receive an email about the data file ingestion, including the file details and the S3 bucket where the dataset is stored.

> You will see the file uploaded in the Content tab even if the ingestion process was a failure because of an invalid file type. Email notifications indicate whether the file ingestion process was a success or a failure.

For details on what data files can be ingested, refer to the [Data Ingestion Requirements](dataingestion_requirements.md)

See below for the metadata field descriptions:

| Field Name | Description |
|------------|--------------|
| Project Number | Mathematica's project number. You see only the projects you have access to. |
| Short Description | The package name that displays on searching - a brief description of the data in the file (alternative file name).|
| Data Summary | Detailed description of the data in the file. The description is displayed when you search for packages. |
| Data Purchased | Indicates if the data file was purchased from an outside source, and to identify the data license agreements.  |
| Aggregation Level | Indicates how each row in the data file is uniquely identified (e.g. Beneficiary, Provider) |
| Focus Area | Indicates the Mathematica focus area represented in the data file. |
| Data Use | Indicates the intended use of the data file for the project. This designates the data files as TEST or PROD to differentiate between development and production data.  |
| PII/PHI | Indicates if the data file contains any PII/PHI data elements. |
| Data Classification | Indicates the security access level of the data file, and to limit the visibility of the package to the appropriate audience. |
| Data Storage Status| The status of the data file in the package. On creating a package, this field is set to loading by default. **You can edit the package details to change the status to show the package is destroyed based on the Data Use expiration date or deleted. ???? In future implementation of the Data Libary, the storage status would update automatically to Active if the data file is transferred to the project unit bucket or Quarantine if the data file ingestion failed.** |
| Data Storage Date | The date the package is created. |
| Requestor Name | The name of the package creator. |
| Data Source Origin | The source location of the data file. For the MVP implementation, you upload the data file from the on-premise data source | 
| Data Tags | One or two-word tag for categorizing the data file (e.g., Inpatient Claims, COVID-19). | 
| Date Published| The creation date of the package. | 
| Data Version Comment| Brief description of the version of the data file. New comments are added for each update to the package such as editing package details, or uploading a dataset. | 
| Data Source Years: Start Year, End Year| Time span represented in the data file in year format. |
| No Data Source Years Apply| Indicates the time span is not applicable to the data file. |  
| Geographic Region| US State or US Region represented in the data file. | 
| Visibility| A check to indicate the package is visible to all in the data library. | 

Questions:

1. Do groups apply
2. What should the data user do if receiving a unsuccessful ingestion notification? Should users change the Data Storage Status 
You can edit the package details to change the status to show the package is destroyed based on the Data Use expiration date or deleted. ????
3. If permissions are not ready in MVP, should we add a note say "Please create packages only for your projects"
2. What's govt-test-tag
