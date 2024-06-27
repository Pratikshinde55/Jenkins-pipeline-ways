# Jenkins-pipeline-ways

We can create pipeline by two ways in Jenkins 
 1. Manual pipeline
 2. pipeline as code (automatic)

Upstream :

  If jobA run then after next automatic JobB run , it means JobA is upstream of JobB .

Downsteram:

  If jobA run then after next jobB automatic start then JobB is downstream job of jobA.
  


# Manual jenkins pipeline (jenkins WebUI):

For this jenkins give many plugins which give different view for pipeline .

for manual pipeline i install "Build pipeline plugin and Delivery pipeline plugin" and restart jenkins:

 Jenkins Dashboard -->> Manage jenkins -->> plugins 

 create manual pipeline:
  - create individual three job and connect them by "post action" or trigger.
  - one job connect to other by manual

 Step 1:
 create jobA , JobB, JobC 'freestyle'

For JobA:--- ( Here we can create JobB downstream for jobA )

 ![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/1ad9d607-37db-4c39-9f83-18fff27b39ad)

For JobB:--- ( Here we can create JobC downstream for jobB )

![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/80dfc8e0-92e4-4ade-b62f-d4d6f9f0c678)





 


    
