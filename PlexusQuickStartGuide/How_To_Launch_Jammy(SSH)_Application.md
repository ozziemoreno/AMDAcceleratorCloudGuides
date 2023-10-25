***

# How_To_Launch_Jammy(SSH)_Application.

***

 **1**. Login to **https://aac.amd.com/**.
    
   ![image](https://github.com/amddcgpuce/AMDAcceleratorCloudGuides/assets/137475062/d62dc96e-e37a-42b3-9b0e-72445014a621)

 **2**. Click on **Applications**. Select **Jammy (SSH)**.

   ![Jammy_app](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/81a8e243-ecc7-47de-abb0-0611398c77a3)

 **3**. Click on **New Workload** button available in the top right corner.

   ![New_workload](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/99cef9af-060a-43ab-a4fa-f3a56b6be130)


 **4**.Select Input Files. Upload any input file(s) which application will need to run. Click **+ Upload files**, and then drag the files into AAC, or click **Browse files** to open the Open file dialog window. Here uploading files is not required, hence click **NEXT** to proceed.

   ![Next](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/649cc131-bfd6-48ef-9e82-9f787ad1433d)

 **5**. In the Resources page, Select the desired parameters. <br>
 **(i)** Under node parameters,by default the **queue oversubscribe** option is **disabled**.<br>
**(ii)** Under node parameters,by default the **telemetry** option is **enabled**. Enabling telemetry gives the performance values once the workload is finished. If not needed, the user can turn off the telemetry. <br>
**(iii)** Under time parameters, there is an option for **maximum allowed runtime**; by default, the value is set to **1 hour**. The user can give their desired runtime. The maximum allowed runtime is **30 days**.<br>
**(iv)** Select the number of GPU's required; by default, the number of GPU's is set to **8**.<br>
After selecting the required resources, click **NEXT** to proceed.  

   ![8 GPUS](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/b48a0fb9-36c6-47d6-abfc-87a7bb4f55c9)

 **6**. In the compute page,Select the cluster with desired queue to run the job. In the following image **1CN128C8G2H_2IB_MI210_SLES15 (Pre-emptible)** queue is selected and Click on **Next** to continue.
  
   ![image](https://github.com/amddcgpuce/AMDAcceleratorCloudGuides/assets/137475004/ca15d5df-df2f-4c31-83e8-efba29305fdc)

 **7**. Review all the configurations selected and click on **Run Workload**.

![image](https://github.com/amddcgpuce/AMDAcceleratorCloudGuides/assets/137475004/ba037494-0b4e-413e-80d7-e25abf72a880)
![image](https://github.com/amddcgpuce/AMDAcceleratorCloudGuides/assets/137475004/d6fa92d5-2284-442b-883a-d666b72def80)
![image](https://github.com/amddcgpuce/AMDAcceleratorCloudGuides/assets/137475004/4115d8e4-a3cc-4f64-8ccf-e0c5b9a2c771)
![image](https://github.com/amddcgpuce/AMDAcceleratorCloudGuides/assets/137475004/8b8edfa9-38ed-4b80-ad04-45a05cc3f6ca)


 **8**. Once the application execution is started then the status gets changed into **Preparing, Pending, Sent, Running** state. 
 The username and password can be found in **STDOUT**
   ![image](https://github.com/amddcgpuce/AMDAcceleratorCloudGuides/assets/137475004/2263059e-9d4b-4b42-bb32-0716c3151eb6)
 
 **9**.User has to wait for some time, refresh the page and scroll down to see the **INTERACTIVE ENDPOINTS** in the right corner. Click on **Connect**.
 ![image](https://github.com/amddcgpuce/AMDAcceleratorCloudGuides/assets/137475004/49cff85c-700b-499d-a90a-f98b180b76cf)

 **10**.To access the server CLI, copy the shell command and replace <USER> with given username and providing password. (username and password can be found in stdout tab). <br>
 Here the username is **aac** and the command is **ssh -p 7004 aac@aac1.amd.com**
 
![image](https://github.com/amddcgpuce/AMDAcceleratorCloudGuides/assets/137475004/fa5f5bd2-ef0e-4359-98f3-2042ed39fb9c)
<br>

 **11**. Once the work is done and to finish the workload Click on the **FINISH WORKLOAD** button and click on **Yes** to complete the workload.
   
   ![finish](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/5b70eb8d-553b-4742-965f-de40ce3ae7e8)
   <br/>
   <br/>
   ![yes](https://github.com/gurumohan123/AMDAcceleratorCloudGuides/assets/137781570/e309714c-63b4-4358-849e-54d9b65b7a16)



   

   







   
