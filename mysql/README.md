helm-wordpress
*installed with helm v2

Commands:

helm version

sudo mv /usr/local/bin/helm /usr/local/bin/helm3

wget https://get.helm.sh/helm-v2.16.9-linux-amd64.tar.gz

tar -xf helm-v2.16.9-linux-amd64.tar.gz

mv linux-amd64/helm /usr/local/bin/helm

sudo mv linux-amd64/helm /usr/local/bin/helm

helm version

kubectl create sa -n kube-system tiller

kubectl create clusterrolebinding tiller-cluster-admin --clusterrole=cluster-admin --serviceaccount=kube-system:tiller

kubectl create sa -n kube-system | grep tiller

helm init --service-account tiller --upgrade

create chart named "examplefile"

go to the directory and execute that command

helm install --name example --values values.yaml .

if you want to use a repository with your pre-configured "values.yaml" file;


cd task3-k8-wp/
   
   
   git add .
  
  
  git commit -m "new file "
   
   
   git config --global user.email "example@gmail.com"
   
   git config --global user.name "eaxmple"
   
   git commit -m "new file "
   
   git push
   
   kubectl get pods
   
   kubectl get ns
   
   kubectl get pods -n wp-mysql
   
   
   kubectl get service -n wp-mysql
   
   kubect lget ingress
   
   kubectl get ingress -n wp-mysql
   
   kubectl get deploy n wp-mysql
   
   kubectl get deploy -n wp-mysql
   
   kubectl get pwc  -n wp-mysql
   
   kubectl get pvc  -n wp-mysql
   
   kubectl get pv  -n wp-mysql
   
   kubectl get secret  -n wp-mysql
   
   kubectl get StatefulSet  -n wp-mysql
   
   kubectl get pods  -n wp-mysql
   
   kubectl get node  -n wp-mysql
   
   kubectl get node  -n wp-mysql -o wide




Dont forget to change the namespace name in values file..
