S3 Security with Tagging based policy : how it can be used access control from SageMaker and Data Engineering AWS Services?

S3 partition design and partition usage in Glue ??

Glue → Crawler → output Database for schema . how database is created? is it internal Glue or RDS ? is it managed by terra-form ?

Glue in details are created by terra-form, then how it can be operated and managed(changed) and save , running and so on?

ETL need Glue  catelog, how it created? 

Glue ETL running lanague ? spark python ? version ? how source code control with git ? 

glue ETL created by terraform,
initial trransform code generated, how it can stored in Git, pusing to Glue ETL?
how developer changes? over the console ? or over the Git ?
Console ? access console ? over whic account ? AD ? or AWS ?
Git ? push to target ETL ?


SageMaker Notebook (EC2 instance based)

AMI ?
Access by user ? how ?
SageMaker Notebook (Created by console)

AMI ?
Access by user? how ? console access with AD ?
Save the code into Repo . how ?


SageMaker Studio

TYPES OF AVAILABLE SAGEMAKER IMAGES 
what are they?
- Data Science [datascience-1.0]: Data Science is a Conda image with the most commonly used Python packages and libraries, such as NumPy and SciKit Learn.
MXNet, PyTorch, Tensorflow.


user access : listing users  : AD connect ?
              oepn brower over aws console ?  HOW?
              AMI
source code notebook git ?

SageMaker Traning

AMI ?
patch process ? 
BAU support process.
Where ? in PAT with PAT data ? or Prod Data?
Model save in PAT or PROD
S3 Access, later inference need Model
ECR, Docker for traning
ECR repo ?
access ?
approved by security


SageMaker Inference

AMI?
futher details ?
request Input API ? any transformation (ex string to numeric)
ECR Repo, access


=========

moniroing and alerting,
traning, billable , how ? and details ? dashboard ? spot instance (baiillabe getting down)  vs on-demand ? business demand ?
dashboard for Ops, Cost, for IMF , 
tagging, identify, cost related resources, 
- tranning done, resource stopped , 

- sagemaker stuido prcing : per suer ? user dashboard, usage, training billable tiem, data engineerting tiem ...

do not ask BAU creaet daahboard, each project need to buidl dashbord for bau, i have doen for my eniter project and 3pp as well.

BAU cost related dashboard.


inferrance stored result. 
busienes will ask claim #1234 why it calcualte bal bla. where is the evident ? bla bal..
BAU position ? IMF pposition ?


Notebook deploy model to prodction, ITSS approval ?
monriigg on-gloing performace, matrix prediction, 
IMF user ask BAU ?? what seniaro IMF will ask BAU ?


data scient user's view there capabilbity, using R only , sagemaker stuido support R ??
https://aws.amazon.com/blogs/machine-learning/bringing-your-own-r-environment-to-amazon-sagemaker-studio/
Docker, BAU maintaince ? 
what if new IMF data scient on-boaning, and need python other than R, what BAU support this ?


BAU user's view, what is supproitng ? user adding, in AD ? depends on access secuirty model.
tracking un-useal or high cumsompuion resource .. cost ..



Glue :data enginieering feature enginnering, 
glue is more data engineering tool no longer BAU working on adding feature and tranformation..

- TAG
- -sagemaker internal ec2 for traning or deploy , no tag no trigger, to prevent



claim triage, callficiation,
how recision, recall is important ? 
sagemaker studio, how it is easier to give performacne to data scietnet ?
what if sagemaker notebook, how hard to give permrance matrix provide? any code reuired build ?

![image](https://user-images.githubusercontent.com/24234662/128103176-85b094fb-62c3-4ab3-8f8d-4a4f60f845f8.png)

