***

# HowTo_Check_Logs_After_Launching_Workloads

***

 **1.Login to https://aac.amd.com/.**
  
   ![image](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/d0ec09a6-d268-4ae8-9479-51a0a7e99f11)
   
 **2.Click on Workloads.**
 
   ![Workloads](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/d7a4f29c-c075-40bd-9cd5-42fef486580f)
   
 **3.Select any workload from the list of completed workloads(for Ex: Gromacs 2022_3-1690169305484).**
 
   ![Workloads_any](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/7ad05cd1-8887-4641-9c2a-d17e5dff9ffd)
   
 **4.Click on Syslog and scroll down for "Show historical logs" option to download the daemon logs(ex: 20230721_D.log).**

   ![syslog](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/0b6c4555-d754-4676-bd98-23c39f24cc5d)
   ![historical logs](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/a93b33b7-3381-4a9a-9572-eae0815688bd)

 **5.Click on download option to download the daemon logs.**
 
   ![daemon_logs](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/fdca1818-8aff-44d2-a659-4e5e75c238de)

 **6.Click on CLOSE and select STDOUT option for the output of any launched application(for ex: Throughput or Images/sec..etc).**
 
   ![stdout](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/99138c6a-c4d7-4088-b1ff-abee00a7570f)
 
 **7.Select the download option for downloding STDOUT logs(example log file name: job-8872-logs.tar).**
 
   ![stdout_downloadlogs](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/04f6799f-793a-4f76-a952-2462b6462fc0)
  
 **8.Click on STDERR to find the errors of any application .**
 
   ![stderror](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/90d2e259-52c9-403b-bf77-b502f98fb788)

  **STDERR: It stands for standard error. It is invoked whenever a command faces an error, then that error message gets stored in this data stream.**
  
  **STDOUT: It stands for standard output, and is used to text output of any command , and then that output is stored in the stdout stream.**













