Issues with managing kubernetes control plane:
Why API server went down? certificate expiry on a server, scheduler might not be working.
EKS- Managed control plane (Highly available kube clusters)
We can create EC2 instances for worker nodes or go with faragate 

Ingress controller watches all the ingress resources and it will configure the LB, external user's request come to LB then to service and then to pod with this.

*******************************************************************************************************************************
This command creates a eks cluster ,vpc, subnets
eksctl create cluster --name demo -region us-east-1 --fargate
*******************************************************************************************************************************
we can attach a autheticator etc too


*******************************************************************************************************************************
if you are usinh faragte, you can use fargate profile to create a new namepsace for your appl to run on
eksctl create fargateprofile --cluster demo --region us-east-1 --name sample-app --namespace game2048

*******************************************************************************************************************************
