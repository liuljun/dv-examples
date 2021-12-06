# dv-examples
This repository will contain examples on how to use IBM data virtualization service on Cloud Pak for Data (aaS)


1. Lakehouse using DV

Step 1: Add object store connection into DV.   
Video - https://github.com/liuljun/dv-examples/blob/main/1.%20Add%20IBM%20cloud%20object%20storage%20to%20Data%20Virtualization.mp4   
Note: for IBM cloud object storage, the service credential needs to enable "Include HMAC Credential" in the "Advanced options". Then you are able to find the "access_key_id" and "secret_access_key" in the service credential.  

Step 2: Virtualize object store files.  
Video - https://github.com/liuljun/dv-examples/blob/main/2.%20Virtualize%20object%20store%20files.mp4  
Note: each .csv file should be put in a different folder because of the restriction - https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=cvo-creating-virtualized-table-from-files-in-cloud-object-storage Besides, the column header should be removed from the .csv file if you don't want to keep it in the virtualized data.  

Step 3: Create a join view.  
Video - https://github.com/liuljun/dv-examples/blob/main/3.%20Create%20a%20join%20view.mp4  
Note: multi-table join is not supported yet. user needs to join them one by one or use SQL editor to create the view directly.  

Step 4: Assign virtualized data to projects.  
Video - https://github.com/liuljun/dv-examples/blob/main/4.%20Assign%20the%20join%20view%20to%20a%20analytics%20project.mp4  
Note: When preview the data in Project -> Assets, the personal credential needs to provide. On CP4D, user can use the platform username and password. On cloud, user needs to use the APIKEY.  

Step 5: Create data caches.  
Video - https://github.com/liuljun/dv-examples/blob/main/5.%20Create%20a%20data%20cache.mp4  
Note: Need to pay attention on the restrictions to use DV caches on more complex queries - https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=queries-restrictions-cache-entries
