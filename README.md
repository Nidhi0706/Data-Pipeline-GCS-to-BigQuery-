# Data-Pipeline-GCS-to-BigQuery-

This project is done for exploring Google Cloud Dataflow, a powerful service for both batch processing and stream processing data.

Setting up a simple pipeline to load data from Google Cloud Storage (GCS) into BigQuery.
Step-by-step path to configure and run the job using a Dataflow template.
Monitoring and verifying the job execution.

# Create a Bucket-
upload all the files in the bucket

# Open Google DataFlow
step1: Create job from template
1.1: Give a unique job name 
1.2: In DataFlow template choose "Text Files on clous storage to BigQuery

step2: Source
Choose the employee_data file through browse (or) copy URL

step 3: Target
Choose the JSON File which is cloud storage location of your BigQuery schema.

step 4: Open BigQuery and create an empty table
Browse for empty table for "BigQuery output table".
For temporary directory select existing bucket.

step 5: Next for Temporary location browse the bucket location and add /temp at the end.

Encryption:
Select any key as per requirement
1.Google-Managed Encryption Key (GMEK) - Fully managed by Google.
2.Cloud Key Management Service (Cloud KMS) Key - Managed by the user (customer-controlled).

step 6: Optional parameters

upload the udf.js pathfile and give the correct ugf name

Finally, Run Job.

