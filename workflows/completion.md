# Completion Workflows
This will outline all the data points, typically in order, that need to be maintained / imported. Once all data points are met, all the data for completion reports will be ready.

## Import the casing reports
- Python scripts exist to import casing reports
- Make sure the ground level and KB are verified before importing
- Make sure the surveys are run all the way to TMD
  - if they are not getting with engineering to get the certified surveys updated
- create the wellbore diagram using Python
- create the completion workbook

## Certified Surveys
- After receiving zip files from drilling
  - Unzip the zip file, and rename the folders containing them to 
  - Certified Surveys
- The zip file should be in the yyyy DRLG/Reports folder
- Copy the Certified Surveys folder to
  - yyyy DRLG/Reports
  - yyyy COMP/Reports
- import the surveys using Python, or DBeaver

## Perforations
- Once perforations are picked, import the perforations
- Use the website
  - well/wellbore/perforations
  - use download button to download perf sheet
  - use wireline memo to get the content to populate
  - use upload button to upload the perfs

## Update the WBD
- run the create WBD script again
- add the frac plugs between perf stages
- add the import perf sheet and rename it to Perfs

## Create well packet for engineering
- Add all the pdfs in the memos folder to a combined pdf once engineering verifies everything is ready
- Engineering can provide a file order

## Send as drilled to surveyors
- run Python script to get update the as drilled information
- at PHT, PHB, and PHB footage from FNL/FSL and FEL/FWL
- query the information, and send it to the surveyors to request the as drilled latitude and longitude
  - request updated plat also

## Frac PJR
- Make sure all frac PJR files are in the frac pjr folder
- Run python script to import all PJR
- Send to engineering to verify data

## Validate planned vs producing perfs
- Put together worksheet comparing planned vs. actual perforations
- Send any discrepancies to engineering for resolution
- Use website to update perf status

## Flowback
- get the final flowback that has been certified by engineering
- import it into the website
  - every time flowback is imported it deletes the previous flowback for that AFE

## Tubing report
- import the tubing report using Python

## Update WBD
- manually add tubing information
- add fill top if well was cleaned out or bottom was tagged
- send final WBD to engineering for approval
  - make sure everything else is up to date

## Get together supporting documentation for completion report
## Run scripts / queries for completion report
