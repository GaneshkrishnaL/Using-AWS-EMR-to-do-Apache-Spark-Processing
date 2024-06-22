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
![Screenshot 2024-06-22 113157](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/d411d97b-5b17-48e4-bca1-484c53300fdf)



![Screenshot 2024-06-22 134535](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/ed67e206-ab91-4e76-9e7f-3e4e3a4490df)


![Screenshot 2024-06-22 135425](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/561cf204-b8fa-44f4-8fa1-2502510738fa)


![Screenshot 2024-06-22 135918](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/9f1a1fd6-0eaf-467c-ad15-aac8425e2ca9)
![Screenshot 2024-06-22 140137](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/585fd59a-d3ce-4b30-83c7-d7a4ed7df03d)
![Screenshot 2024-06-22 142501](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/5ca1248a-7584-48ab-8506-d57db989a761)
![Screenshot 2024-06-22 143424](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/14fc2fb0-9381-4b6b-8d7a-b91fde09fba5)

![Screenshot 2024-06-22 143900](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/464dc91f-7608-4329-b005-a58281c69af6)



![Screenshot 2024-06-22 150318](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/74f79a88-566a-4002-bd33-a9599bf0d7e1)


![Screenshot 2024-06-22 150336](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/64c7ace3-f7db-4440-acba-9a24481a7899)

![Screenshot 2024-06-22 150408](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/60394eed-ff7f-4a04-8197-3e4b9dbc1c9f)

![Screenshot 2024-06-22 150738](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/50da70e0-e9ef-477e-9e7b-6c2ad23c99f4)

![Screenshot 2024-06-22 151041](https://github.com/GaneshkrishnaL/Using-AWS-EMR-to-do-Apache-Spark-Processing/assets/92093823/5a224c24-c4ab-4e9e-b07d-02277db56540)





































