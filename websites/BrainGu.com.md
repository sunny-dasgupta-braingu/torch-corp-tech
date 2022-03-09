# Updating the BrainGu website
*The BrainGu website is a flat site. It is not managed through a CMS, all updates are done via HTML, CSS, and JS. The framework is Bootstrap 4.*
## Where is the site hosted?
The BrainGu site is hosted on AWS. Individuals who have access include:
* Matt Shaver
* Sunny Dasgupta
* Asa Yeamans
## Who manages the site?
Sunny Dasgupta, Marketing & Communications Manager, manages all updates to the site. If you would like any changes made reach out to Sunny. 
## How is the site updated?
*These instructions should only be followed in the case that Sunny Dasgupta is unavailable and a site update is urgent. Otherwise, please reach out to Sunny Dasgupta for any changes.*
#### Step 1
Download the files for the site here: https://github.com/braingu/dot-com-2.0 
#### Step 2
Find the appropriate subfolder, and file you want to make content edits to and make your updates using HTML, CSS, or JS. Reminder, the framework is *Bootstrap 4*.
#### Step 3
Once you've made you changes, commit your changes to the main branch. 
#### Step 4
Deploy the site using the steps below:
1. Launch Terminal
2. cd FolderLocation/dot-com-2.0 [enter]
3. ls [enter]
4. ./deploy-prod.sh [enter]
5. Are you sure: Y [enter]
6. Assets: (if you updated any images) Y | (if you did not update any images) N [enter]
7. Webpages: Y [enter]
#### Step 4 Alternate
Additionally, you can also deploy the site directly via AWS
1. S3 Bucket: select the specific files you want to update and delete those files.
2. S3 Bucket: upload the new replacement file - ensure the file name is the same as what you deleted.
3. CloudFront: https://console.aws.amazon.com/cloudfront/home?region=us-east-2#distribution-settings:E2JZUZRV0UPAVU 
4. Click on Invalidations -> Create
5. /*
