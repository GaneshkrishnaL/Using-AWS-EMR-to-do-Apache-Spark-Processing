# Using-AWS-EMR-to-do-Apache-Spark-Processing
setting up an Amazon EMR cluster and running Spark jobs using  Cloud9 CLI andEMR steps.

Sure, here are the steps written in the past tense as if you had already performed them:

### Steps to Set Up and Run a Spark Job on Amazon EMR

1. **Chose a Programming Language:**
   - I wrote my Spark job in the language of my choice (Python, Java, Scala).

2. **Prepared the AWS Environment:**
   - **Created an AWS Account:** I signed up for AWS. Since I already had an account, I signed in using my credentials.

3. **Navigated to the EMR Service:**
   - In the AWS Management Console, I searched for and selected "EMR" (Elastic MapReduce).

4. **Created a New EMR Cluster:**
   - **Cluster Name:** I named my cluster "EMR Master Class".
   - **EMR Version:** I chose the desired version (e.g., 6.14).
   - **Applications:** I selected the applications I needed (e.g., Hadoop, Livy, Spark, Jupyter).

5. **Configured the Cluster:**
   - **Node Configuration:** I left the default node configuration.
   - **EBS Root Volume:** I set it to 15 GB.
   - **Cluster Scaling:** I set the cluster size manually to one node.

6. **Configured Networking:**
   - **VPC Configuration:** I created or selected a VPC.
     - **VPC CIDR Block:** (e.g., `172.31.0.0/16`).
     - **Public and Private Subnets:** I created a public subnet for my EMR cluster.
   - **Security Groups:** I configured security groups to allow necessary traffic.

7. **Set Up Additional Configurations:**
   - **IAM Roles:** I created and configured IAM roles for the EMR cluster to allow access to S3 and other services.
   - **Key Pair:** I created and downloaded a key pair for SSH access to the cluster nodes.

8. **Created an S3 Bucket:**
   - **Bucket Name:** I created a bucket to store my input data and output results (e.g., `emr-master-class-s3bucket`).

9. **Configured Cluster Logging and Monitoring:**
   - **Cluster Logs:** I enabled logging to monitor cluster activity and troubleshoot issues.
   - **Cluster Termination:** I set cluster termination settings to manual or automatic as needed.

10. **Launched the EMR Cluster:**
    - I clicked "Create Cluster" to launch the EMR cluster and waited for the cluster to start and be ready.

11. **Set Up Cloud9 Environment:**
    - **Created a Cloud9 Environment:** I named it `EMR Master Class Cloud9`.
    - **EC2 Instance Type:** I used a t2.micro instance.
    - **VPC:** I selected the VPC created for my EMR cluster.

12. **Uploaded Key Pair to Cloud9:**
    - I uploaded the previously downloaded key pair to the Cloud9 environment.
    - I changed the permissions of the key file to read-only (`chmod 400 <key-file>`).

13. **SSH'ed into EMR Cluster:**
    - I used the key pair to SSH into the master node of the EMR cluster from the Cloud9 environment.

14. **Prepared and Submitted the Spark Job:**
    - **Created Spark Job Script:** I wrote the Spark job script (e.g., `spark_etl.py`).
    - **Uploaded Data to S3:** I ensured the input data was available in the S3 bucket.
    - **Ran Spark Submit:** I used the `spark-submit` command to run the Spark job on the cluster.

15. **Verified Job Execution:**
    - I checked the output in the specified S3 bucket to ensure the job ran successfully.
    - I monitored job status and logs via the EMR console and Spark history server.

