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
  - create three job and connect them by "post action" or trigger.
  - one job connect to other by manual



 


    
