#Activation Spreadsheet Workflows

### Requirement 1: Admin Upload initial Template:
* Use lambda to read all sheets and headers.
* Return JSON data packet with sheets and header information (sheet names, and the header names for each sheet)

### Requirement 2:  Admin Replaces Existing Template With New Template
* Delete all existing data for old template.
* Use lambda to read sheets and headers.
* Return JSON data packet with sheets and header information (sheet names, and the header names for each sheet)


### Requirement 3:  User From a Lab Uploads New Data Entry Spreadsheet
* Use lambda to strip data from spreadsheet and store in DynamoDB
* Return good/bad response to user depending on if data was processed successfully


### Requirement 4:  User From a Lab Uploads Replacement Data Entry Spreadsheet
* Use lambda to strip data from spreadsheet and store in DynamoDB.
* Return good/bad response to user depending on if data was processed successfully.


### Requirement 5:  Admin Gets Final Overall Data Report
* Generate on demand report spreadsheet with data from all labs that have uploaded data.
* Allow admin to download completed report when generated.
