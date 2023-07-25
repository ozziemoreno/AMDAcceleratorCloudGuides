***

# How_To_Launch_Jammy(SSH)_Application.

***

 **1. Login to https://aac.amd.com/.**
    
   ![image](https://github.com/amddcgpuce/AMDAcceleratorCloudGuides/assets/137475062/d62dc96e-e37a-42b3-9b0e-72445014a621)

 **2. Click on Applications. Select Jammy (SSH) .**

   ![Jammy_app](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/81a8e243-ecc7-47de-abb0-0611398c77a3)

 **3. Click on 'New Workload' button available in the top right corner.**

   ![New_workload](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/99cef9af-060a-43ab-a4fa-f3a56b6be130)


 **4. Click on Next button available in the right corner.**

   ![Next](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/649cc131-bfd6-48ef-9e82-9f787ad1433d)

 **7. Select the allowed run time. The number of GPUs should be 8. Here, we have selected the run time as 1 hour, number of GPU’s as 8 and telemetry is enabled and Click on Next button.**

   ![8 GPUS](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/b48a0fb9-36c6-47d6-abfc-87a7bb4f55c9)

 **8. Select the cluster with desired queue to run the job. In this case 1CN128C8G1H_4RoCE_MI250_Ubuntu22 (gpu:mi250:8(S:0-1)) is selected and Click on Next.**
  
   ![queue](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/35ca8cc3-9bb8-45a8-83cd-925da07e1d5d)

 **9. Review all the configurations selected and click on Run Workload.**

   ![run1](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/192d4b5f-e4ff-4bc7-b47d-21b2a4426571)
   ![run2](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/28dda06f-356b-4d30-a18f-a58233c9cbbd)
   ![run3](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/2afdfebc-e830-4a3f-a712-197377636a0f)
   ![run4](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/06d5b0a8-15d6-4542-8ea0-de66714ae229)

 **10. Once the application execution is started then the status gets changed into 'Preparing','Pending','Sent','Running' state. The user has to wait to see the INTERACTIVE ENDPOINTS to access the interactive shell. get the username and password from the STDOUT tab and click on Connect.**
 
   ![username and password](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/1a4447d2-3b33-4f9e-ab8e-5f4eea0fce66)

   ![Connect](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/dc067924-f138-4565-a667-650abe89b1db)

   
 **11. Click on "Copy Shell Command" button, Open command prompt or Windows PowerShell and enter username and password.
  here username is aac and password is irRSFzt7WoCpwoCKD5P58qWhv0sCPQ5Y.**

   ![copy](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/c8df9813-3326-40b2-9cb4-769ce7fd8e73)
   ![username](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/c9f2c01a-cd8c-4984-a4d9-f50dfec5b0f6)



 **12. Once interactive shell access is verified Click on "FINISH WORKLOAD" button and click on Yes to complete the workload**
   
   ![finish](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/5b70eb8d-553b-4742-965f-de40ce3ae7e8)
   ![yes](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/e309714c-63b4-4358-849e-54d9b65b7a16)


   

   







   
