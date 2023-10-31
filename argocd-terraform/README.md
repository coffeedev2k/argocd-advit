# ArgoCD deployment by Terraform

* Deployment of ArgoCD HelmChart
* Deployment of ArgoCD ROOT Application

Copyleft (c) by Denis Astahov.


создать кластер в EKS

eksctl create cluster -f eks_cluster_dev.yaml

aws eks list-clusters

aws eks update-kubeconfig --name demo-dev --region us-west-2
aws eks list-clusters  --region us-west-2
  964  31/10/23 11:25:28 terraform init
  965  31/10/23 11:26:34 terraform apply
  966  31/10/23 11:28:07 head -n 50 main.tf
  967  31/10/23 11:34:37 terraform init
  968  31/10/23 11:34:59 k get namespace
  969  31/10/23 11:35:16 history
  970  31/10/23 11:35:26 aws eks update-kubeconfig --name demo-dev --region us-west-2
  971  31/10/23 11:35:30 k get namespace
  972  31/10/23 11:35:50 k get all
  973  31/10/23 11:37:45 awscli version
  974  31/10/23 11:37:49 aws-cli version
  975  31/10/23 11:37:56 aws version
  976  31/10/23 11:38:00 aws version --version
  977  31/10/23 11:38:13 aws help
  978  31/10/23 11:38:37 aws version
  979  31/10/23 11:39:10 sudo apt install awscli
  980  31/10/23 11:40:03 cd /tmp
  981  31/10/23 11:40:06 curl -LO https://storage.googleapis.com/kubernetes-release/release/v1.23.6/bin/linux/amd64/kubectl
  982  31/10/23 11:40:27 ls
  983  31/10/23 11:40:33 file kubectl
  984  31/10/23 11:40:51 mv kubectl kubectl1.23.6
  985  31/10/23 11:39:16 sudo apt update
  986  31/10/23 11:41:16 chmod +x kubectl1.23.6
  987  31/10/23 11:41:27 sudo apt install awscli
  988  31/10/23 11:41:52 kubectl1.23.6 get all
  989  31/10/23 11:42:46 kubectl1.23.6 get namespaces
  990  31/10/23 11:43:09 kubectl1.23.6 get all -n namespaces
  991  31/10/23 11:43:19 kubectl1.23.6 get all -n argocd
  992  31/10/23 11:43:46 kubectl1.23.6 get secrets -n argocd
  993  31/10/23 11:45:06 kubectl1.23.6 get secrets -n argocd argocd-initial-secret -o jsonpath=".data.password}" | base64 -d
  994  31/10/23 11:45:17 kubectl1.23.6 get secrets -n argocd argocd-initial-admin-secret -o jsonpath=".data.password}" | base64 -d
  995  31/10/23 11:45:22 kubectl1.23.6 get secrets -n argocd argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d
