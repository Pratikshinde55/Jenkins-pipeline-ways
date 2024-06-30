# Jenkins-pipeline-ways

We can create pipeline by two ways in Jenkins :
 1. pipeline as code (automatic)
 2. Manual pipeline

  

# 1. Pipeline as Code:

  Pipeline as code can create by using "Groovy language". It is DSL ( Domain-Specific Language)

  Groovy Language also run on JVM (Java virtual machine).

 Ways of write Pipeline as code: 
  1. Scripted 
  2. Declarative  
   
ways of create pipeline as Code:
  1. Jenkinsfile (Create on local or gitHub and access by Jenkins WebUI)
  2. Direct create Declarative Script on Jenkins WebUI.


⚙️ For Pipeline as code following terms are use in Jenkinsfile or Jenkins WebUI:

  - stage : This is means job, consider we can create jobA, JobB, JobC that job is known as Stage.
  - steps : Tt is sub-block of stage. In every job we can do somethings that things in stage is known as steps.
  - stages : All Multiple Stage (Jobs) put in one block that is known as stages block {}.
  - pipeline : It is keyword which use for declare this pipeline as code. It is main block in which we put all stages, steps, agents, and so on.
  - agent : It is about on which node we want to run stage/job or pipeline, By Using "label" we specify that on which node we want execute pipeline.


Jenkinsfile : 

It is Standard name of the file in which pipeline as code store.


 - Now Create pipeline as Code: (Select 'pipeline' for create pipeline as code)
![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/d10af14c-a676-4538-aa90-916e157055d7)

![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/f3deea6b-8cbb-4906-99e6-cd4673ffc123)

![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/c46cb3f4-d735-4a32-8d5f-99c49e6a8de5)

![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/5176c8ee-2de6-4599-af8d-b9b11a8b32f5)

![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/e0e34b56-0b0f-44cb-8c66-eed4c6c95ed7)


# 2. Manual jenkins pipeline (jenkins WebUI):

- Upstream :

  If jobA run then after next automatic JobB run , it means JobA is upstream of JobB .

- Downsteram:

  If jobA run then after next jobB automatic start then JobB is downstream job of jobA.
  
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

Onlu need to initial job and also we can give final job of pipeline.

go to "My view"  -->> "new View" -->> "Delivery Pipeline View" 

![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/415cf65f-1b14-4a72-a074-b5b9ddc9b1c8)

we can get follow view :

![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/56b841f1-7e7c-4fad-8c1c-749170aedf6a)


 
- Note :
Also we can add new job which is run wehn other run, menas we can add upstream job for new JobD.

we can create by using "Build trigger" -->> "Build after other projects are built"

![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/bbd28d4a-3111-43fd-8cdd-b3e2fb241c23)

pipeline view by delivery plugin:

![image](https://github.com/Pratikshinde55/Jenkins-pipeline-ways/assets/145910708/286d7dce-3675-4526-82c4-b2b978ce6b06)


