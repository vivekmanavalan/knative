# knative
This repository has all the resources needed to run knative in kubernetes engine

create a free trial account in google cloud 

create a cluster in the gke

IN LOCAL:
install gcloud cli

install kubectl 
gcloud components install kubectl
kubectl version - to check version

open the cluster using the kubectl command 
gcloud container clusters get-credentials CLUSTER_NAME --zone ZONE_NAME

If the target cluster is not running in the default zone or region, or if you did not set a default zone or region, 
you need to supply the region (--region=REGION) or zone (--zone=ZONE) in the command.


To get pods
kubectl get pods

To get service running
kubectl get ksvc

T0 install knative 
goto to knative home page and select yaml installation

execute the serving commands and use kourier it's lightweight

To check logs in knative service
It has two parts in it user-container and queue proxy

kubectl get logs -f user-container
