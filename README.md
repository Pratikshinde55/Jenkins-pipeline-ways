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
  
 create jobA , JobB, JobC 'freestyle'

For JobA:--- ( Here we can create JobB downstream for jobA )

 ![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/1ad9d607-37db-4c39-9f83-18fff27b39ad)

For JobB:--- ( Here we can create JobC downstream for jobB )

![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/b24b9c7e-6526-467e-b16c-64b6c86c01d8)

Now we can create 'New view' file jenkins Dashboard :

![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/ebbc47bf-edb4-4b30-b3d3-528af72aa4a9)


1. Now create by Build pipeline view :

 This is option only come when we install Build pipeline plugin

 we can add multiple feature and button and also we add different jobs, 

 Only need to give Initial Job 

 ![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/520cb0b5-b6e9-41dc-9943-ab1aeaa42235)

 see pipeline :
 ![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/17758cef-2aa3-442e-a7cb-84aabeb3472e)


2. Now create by Delivery pipeline view:

This pipeline plugin give visual view.
we can add multiple features and buttons.

 


    
