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
- Data Science [datascience-1.0]: Data Science is a Conda image with the most commonly used Python packages and libraries, such as NumPy and SciKit 
- Learn.
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



# terraform 
- airflow, glue, and sagemaker, notebook.. 
- what actual python code are manainged over terraforme and running ? 
- how it can be control over terrafome ? or sort of source code ? how it runs, modify and update in terrafrome or outside of terraform.



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




1. raw data -> data anaysis (null? empty? visulaised, manupliate )-> feature enginnering (missing data from other ML)-> ML input data (traning set, validate set, test set)
ML input data depends on potencial traning algorithm. 

2. ML input data -> hyperparameter tunu -> traning -> reuslt with perfoamce matrix (recall, F1, presicion...)

repeat. 2, or 1->2 if other alothgirems use. (experiment)

3. model -> deploy -> endpoint -> perfoamce monitoring. -> data stored for retraining.

retraining.

Freedom to Data scienet upto 2, restiection on deploy model for 3. 
monriting, resource creation, uesage, are cirital to use expensive resources. 
(IAM remove sagemaker.deploy role? is it possbile ?)

(?) sagemaker with airflow ? what is airflow ? 
https://sagemaker.readthedocs.io/en/stable/v2.html
https://sagemaker.readthedocs.io/en/stable/workflows/airflow/sagemaker.workflow.airflow.html



EXPERIMENT : code level 
very afrid of data scientist capabilty, program , bau 





invlove program for 
- asking right question, 
- BAU dashboard
- BAU alerting, monitoring
- BAU acitivices, (user adding, user to do what, resource control, lifecycle)
- new beast never seen before. 
- do not blame because bau did not ask, program shoudl pro-active to provide more details before bau asked. 

sagemaker autopilot deploy give option, to save requert, save response.
what is normal way to save request, response ?


internet access : it may requried to install packages (i.e. sagemaker-experiements)

# new MLOps.
- Sagemaker studio notebook, 
- powerful when user knows programming, data engeering, data scient (algoritm, hypterparameter) and AWS (S3, instance type .... ) and sagemaker sdk (experiments, trial, Tracker...)
- Dagerous when user does not eunugh know any single fields. single notebook can do everything.
- it will kick off compute resources out side of VPC, deploy to model.
- how it can be used ? in IMF Data scieent 
- if know enough then, it will be great tool, but it looks difficult to use to me , :(


# Azure ML
- Azure ML designer, (stuido) : tool for data scientist using with drag and drop
- BAU is not drag and drop -> same as Sagemaker.
- what BAU allows to user (data scientist and other engineer) to access AWS console or Azure portal

# BAU challenage.
more complex services and more advanced featuere are adding on cloud service.
it is no longer terraform only support cloud as code. 
user access, runntime change, apply . 
need to think in the future of cloud mataticty. 


