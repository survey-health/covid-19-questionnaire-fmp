# COVID-19 Questionnaire
This is the FileMaker application for the covid questionnaire and requires the web client and api to work.

## About

This open source application is free to use or modify, however, it does not include detailed documentation or instructions.

This COVID-19 Questionnaire solution is a public preview of parts of a custom solution which was purpose-built for Glenbrook High School District 225 in Northfield Township, Cook County, Illinois.

This public previvew release has been modified to make it more suitable for use by other districts by removing features and integrations which are Glenbrook-specific. The application is being provided as-is free of charge for any school district with the development and infrastructure resources to customize and deploy it for their own use.

If you are interested in a turnkey solution, visit https://www.soliantconsulting.com/school-covid-questionnaire/ for more information.

# System Requirements

Requires FileMaker 19 platform. (See: https://community.claris.com/en/s/article/FileMaker-Server-19-System-Requirements)

Note: FMS on MacOS not supported

## Scale

A single stack instance can support up to 10k users. For larger districts, user data must be split into separate groups of 10k users or less. For example, K-6 and 7-12 groups.

## Data Format

### User Photo Requirements
* 2:3 ratio ~200x300px in portrait orientation
* jpeg format
* Filename must contain the matching id and be formatted as `{id}.jpg`

### CSV user data
Data columns must be in the following order with no header row. Non-required columns must be included in the CSV, even if they contain only empty values.

#### Faculty Table

| Column | Required
| --- | ---
| SchoolID | X
| Employee ID | X
| DOB | X
| Last Name | X
| First Name | X
| Middle Name |  
| Prefix |  
| Department |  
| Location Code |  
| Location Description |  
| Active |  

#### Student Table

| Column | Required
| --- | ---
| School ID | X
| Student ID | X
| Last Name | X
| First Name | X
| Grade |  
| Gender |  
| DOB | X
| Street |  
| City |  
| State |  
| Zip |  
| Emergency Contact 1 Name |  
| Emergency Contact 1 Relationship |  
| Emergency Contact 1 Phone |  
| Emergency Contact 2 Name |  
| Emergency Contact 2 Relationship |  
| Emergency Contact 2 Phone |  
| Emergency Contact 3 Name |  
| Emergency Contact 3 Relationship |  
| Emergency Contact 3 Phone |  

## Version Updates
Updating between release versions requires YADMT (Yet another data migration tool)

https://www.soliantconsulting.com/blog/yet-another-data-migration-tool/

### YADMT Requirements

FDS (Filemaker Developer Subscription)
https://store.claris.com/product/FDS 
FileMaker Pro 19 on a supported version of Windows
