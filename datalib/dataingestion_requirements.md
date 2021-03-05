# Preparing Data for ingestion

The Data Library will be able to accept various type of data files from different sources. 

### File types

For the pilot implementation, the Data Library can accept the following types of files:

* Word documents with DOCX/DOC file extension
* Documents with PDF file extension
* Text files with TXT file extension
* Tagged image files with TIF file extension
* Shapefiles (containing geographical data) with SHP file extension
* Excel Spreadsheets with XLSX/XLS file extension 
* Comma-separated value files with CSV file extension
* Stata datasets with DTA file extension
* SAS datasets with SAS7BDAT file extension
* R data with RDATA file extension


### File size

File size limitation - You cannot upload files of sizes larger than 5 GB. Is there a limit to the storage size for a project.

File names - File names can include spaces

### Data source origin

For the pilot implementation, you are able to upload data from the following sources:

* On-prem location: This location refers to files that can be uploaded from your system, or from the N:drive.

### Data Storage

The dataset files that you ingest (upload) in the Data Library are stored in AWS S3 (Amazon Simple Storage Service) buckets. The S3 buckets offer secure storage and include permission policies to allow only authorized users access to the datasets. With the S3 buckets categorized on the project unit/focus areas (Health,Human Services, International), the Data Library makes it easy to manage, analyze the diverse datasets in the library and break down the data silos at the organization level.

When you upload the files via Packages in the Data Library, they store in a landing zone bucket, which is a short term storage location for the uploaded files. File type validation checks initiated on the uploaded files then decide where to move the data files. On passing the validation, files transfer from a landing zone bucket to a project unit storage bucket, and files that fail move to a quarantine bucket. Email notifications are sent to the project System Leads, file uploader, and the administrators indicating the ingestion status, the dataset details, and the storage bucket.

Question:

1. What should the data user do if receiving a unsuccessful ingestion notification?


