
 Install the MYSQL database on kubernetes using kubernetes artifact files  i.e. 
 
    mysql-deployment.yaml 

    mysql-configmap.yaml

    mysql-service.yaml

    mysql-secret.yaml 
   
Before going deep dive into deployment architecture let's first understand this concepts.

    Deployment :-
      Deployments represent a set of multiple, identical Pods with no unique identities. 

    Service :-
      Services are use to group pods together using labels & selectors. 

    Secret :- 
      Secrets are used to store confidential attributes such as password, API key etc.

    ConfigMap :- 
      ConfigMaps are used to store configuration parameters such hostname, port etc.
      
SEPTS :- 
 
Clone github repository

       git clone https://github.com/PatilDurga/Kubernetes.git

Go to session_1 directory

     cd ./kubernetes/MYSQLDB/

Create demo namespace

    kubectl create namespace demo
  
Set current namespace to demo

     kubectl config set-context --current --namespace=demo
   
Create secret 

      kubectl create -f mysql-secret.yaml 
    
Create configmap

     kubectl create -f mysql-configmap.yaml
     
Create deployment for MySQL

     kubectl create -f mysql-deployment.yaml

     kubectl get pods --watch

Exit when pod goes into running state
  
Create service for MySQL

      kubectl create -f mysql-service.yaml
      
      
Store MySQL root password in secret File.
AND 
Store host & port in configmap File . 

      





     
 

