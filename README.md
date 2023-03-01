Kubernetes deployment steps for GCP
https://www.udemy.com/course/docker-and-kubernetes-the-complete-guide/learn/lecture/25408376#questions/17305086

gcloud config set project [PROJECT_ID]
gcloud config set compute/zone asia-south1-a
gcloud container clusters get-credentials [CLUSTER_NAME]

kubectl create secret generic pgpassword --from-literal PGPASSWORD=[POSTGRES_DATABSE_PASSWORD]

Run following command in cloud console:
curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3
chmod 700 get_helm.sh
./get_helm.sh
helm repo add ingress-nginx https://kubernetes.github.io/ingress-nginx
helm install my-release ingress-nginx/ingress-nginx
(https://www.udemy.com/course/docker-and-kubernetes-the-complete-guide/learn/lecture/17417508#notes)
