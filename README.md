# END to END azure data engineering  adwenture works project 

![image](https://github.com/user-attachments/assets/4e5af451-3a4e-48f8-9c13-1ce7127c1cf6)

## services used in the projects
### azure data lake gen 2 storage
### azure data factory
### azure databricks
### azure synapse analytics
### powerBI desktop

![image](https://github.com/user-attachments/assets/a9817f9e-a6b6-4e94-99e1-5b0b876f0b4c)


## medalin architechture for data storage in adls gen 2
![image](https://github.com/user-attachments/assets/7228f5ac-0a99-4551-ae4b-cdd9d30de921)

## bronze layer raw data from copy activity data factory from github http data source
![image](https://github.com/user-attachments/assets/7fd4aad6-8a9e-40b3-82d8-12367d2c76d6)

## creattion of dynamic copy activity using lookup and for each activity to copy data from github to adls bronze conatianer
![image](https://github.com/user-attachments/assets/28213070-3c52-4560-aa99-70a59c693718)
##
parameters used in json format for dynamic copy value we get in lookup activity
![image](https://github.com/user-attachments/assets/1497cec3-455f-44f8-8be0-c27f0e778b92)

## link services
![image](https://github.com/user-attachments/assets/970418ed-ba19-44fd-9737-fe09ab921362)

## population of data after running the pipeline successfully
![image](https://github.com/user-attachments/assets/939456b0-2ac2-47ff-85ac-5b2e245a88af)

![image](https://github.com/user-attachments/assets/adbf1359-7ebf-40ac-b606-43951a588a26)

## creating permision to databricks for accesing read/write adls gen 2
    ***create app registration in azure entra id and giving rbac storage blog contributer role to this application from adls RBAC
    credential needed in databricks:-
    aplication /client id 
    directory(tenant)ID 
    secrete value from certificates and secrestes***
    
     

## data transformation silver layer using databricks pyspark
aw_silverlayer notebook in repo
![image](https://github.com/user-attachments/assets/2a7adf3a-ec0e-47c8-9c03-d8758880ea0d)
![image](https://github.com/user-attachments/assets/198b097b-b018-4c32-8633-243ba0b786ca)
![image](https://github.com/user-attachments/assets/f2468ee2-3e03-48dd-b957-6d1779389a19)
## writing all data one after another after tranformation in the dataframe
![image](https://github.com/user-attachments/assets/1e583aa2-db88-4e09-975d-336281fef1b5)
 ## using databricks visualtion 
![image](https://github.com/user-attachments/assets/7facfcd3-dcd9-45c6-a728-6eded7bfd8d1)

![image](https://github.com/user-attachments/assets/c5998b6f-40c2-4adf-b884-2b40e8eed1c9)

## silver layer data after tranformation
![image](https://github.com/user-attachments/assets/25a8ad95-8390-4fc7-8ab7-60c4a55b78f5)


## now in azure synapse analytics 
    created serverless sql pool for lakehouse feature
    created schema gold
    created views fr each table 
    created external table extsale in gold conatainer 
    ![image](https://github.com/user-attachments/assets/57ffc234-44cf-49f1-b8c6-7342650ac909)

    ![image](https://github.com/user-attachments/assets/3421ca41-0c16-4f66-ba96-09cd720d21a4)

## using sql serverless endpoint from synapse to load exttable in powerbI for bussiness intelligenge visualization
![image](https://github.com/user-attachments/assets/9901325b-e09e-4a4d-80f8-28478515f374)
