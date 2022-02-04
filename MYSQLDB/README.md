
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
  git clone 

Go to session_1 directory
  cd ./kubernetes/MYSQLDB/
  
 





     
 

