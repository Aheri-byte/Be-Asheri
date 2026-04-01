# Creating an S3 bucket in AWS and host and estatic website
-  ## Creating S3 bucket
-  from your AWS home console,go to S3  and in the click S3 service.
-  Click on the "create bucket" button.
-  in the new interface, go to the bucket name, this should be a unique name.
-  Leave all defult setting as the can be configured afterward.
-  click on the "creat bucket" button.
###bucket created
<img width="1920" height="1020" alt="S3 buckets _ S3 _ us-east-1 - Google Chrome 01_04_2026 23_23_05" src="https://github.com/user-attachments/assets/797bdfd3-322d-4cc3-a52b-2b317bddabe6" />
##Hosting an Estatic website on the S3 bucket.
-  Open your S3 to view.
-  Under the name,click on properties.
-  Scroll right down to static website.
-  Click on "edit" on the rifht of teh screen.
-  Take "Enabled" and other configurations will come.
-  In the index document space, type "index.html" and type the same for the error document.
-  save the changes
-  ### downlaoding the website
-  go to the site Tooplate and downlaod a website.
-  go the file, right click and take copy and the extract. This changes the format of the file.
-  ### uploading files and folder
-  go back your S3 bucket view and take upload of the right on the screen.
-  Open the the file and the folder you downloaded in the S3.
-  click upload at the end.
-  <img width="1020" height="1920" alt="S3 buckets _ S3 _ us-east-1 - Google Chrome 01_04_2026 23_55_02" src="https://github.com/user-attachments/assets/73faacfb-c551-4f33-bc10-ba4e65709678" />

-  Close the interface, and go to the where you have the static website.
-  copy the link of the webiste and paste in a new windows to run.
-  You will receive a 403 error.
-  ### setting up a bucket policy
-  back to S3 view, take permission
-  turn of the block public access and save and comfirm.
-  Go to bucket policy and click on "edit Policy"
-  Now on a new windows, search "AWS policy generator"
-  Open the website
-  in type of policy, type "S3 bucket policy"
-  In effect take "allow"
-  In principle type "*"
-  in action, take "getobject"
-  in the souce file, copy the ARN link and paste there,and /*
-  Click generate policy, you will be direct back to the "add statement" field,
-  Click and the add statement and click the generate policy after.
-  the JSON policy will open up, copy the policy.
-  <img width="1920" height="1020" alt="asheri-test-s3 - S3 bucket _ S3 _ eu-north-1 - Google Chrome 31_03_2026 00_20_50" src="https://github.com/user-attachments/assets/87881168-fbc5-48c1-a0d0-c3058b9ea8a0" />
-  go back to the S3 bucket, and the paste code the edit statement space.
-  Click om save change, and you will get:
  <img width="1920" height="1020" alt="S3 buckets _ S3 _ us-east-1 - Google Chrome 02_04_2026 00_20_40" src="https://github.com/user-attachments/assets/b5d0c47d-029c-48c0-add5-bd3ee0278514" />
-  Now go back to teh windows and run the webiste.
  <img width="1920" height="1020" alt="S3 buckets _ S3 _ us-east-1 - Google Chrome 02_04_2026 00_29_19" src="https://github.com/user-attachments/assets/c95ccfc9-2df8-4311-8e6b-0c021a8fc1eb" />
