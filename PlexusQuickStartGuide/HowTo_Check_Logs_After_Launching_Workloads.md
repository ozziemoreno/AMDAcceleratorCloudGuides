***

# HowTo_Check_Logs_After_Launching_Workloads

***

 **1**. Login to **https://aac.amd.com/**.
  
   ![image](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/d0ec09a6-d268-4ae8-9479-51a0a7e99f11)
   
 **2**. Click on **Workloads**.
 
   ![Workloads](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/d7a4f29c-c075-40bd-9cd5-42fef486580f)
   
 **3**. Select workload for which logs need to be checked. In the following image **Gromacs 2022_3-1690169305484** is selected.
 
   ![Workloads_any](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/7ad05cd1-8887-4641-9c2a-d17e5dff9ffd)
   
 **4**. Click on **SYSLOG** and scroll down for **Show historical logs** option.

   ![syslog](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/0b6c4555-d754-4676-bd98-23c39f24cc5d)

 **5**. Click on **Show historical logs**, press **download** button to download the logs (ex: 20230721.log).
 
   ![historical logs](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/a93b33b7-3381-4a9a-9572-eae0815688bd)
   <br/>
   <br/>
   ![download](https://github.com/amddcgpuce/AMDAcceleratorCloudGuides/assets/137781570/a19e1d5d-696f-4f29-9fbe-891c3ef55118)


 **6**. Click on **CLOSE**, select **STDOUT** option to check the output of any launched application (for ex: Throughput or Images/sec..etc).
 
   ![close](https://github.com/amddcgpuce/AMDAcceleratorCloudGuides/assets/137781570/ed1ee232-86cb-4f00-b7fd-b01f3cce5ee2)
  <br/>
  <br/>
   ![stdout](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/99138c6a-c4d7-4088-b1ff-abee00a7570f)
 
 **7**. Select the **download** option to download **STDOUT** logs (ex: job-8872-logs.tar).
 
   ![stdout_downloadlogs](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/04f6799f-793a-4f76-a952-2462b6462fc0)
  
 **8**. Click on **STDERR** to find errors of any application.
 
   ![stderror](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/90d2e259-52c9-403b-bf77-b502f98fb788)

  **STDERR:** It stands for standard error. It is invoked whenever a command faces an error, then that error message will be displayed in the STDERR tab.
  
  **STDOUT:** It stands for standard output, and it is used to display output of any command in the STDOUT tab.













