# K8S-tuto
fichier tuto K8S

 pour les le secret il faut  mettre les mot  en base63 
echo -n 'admin' | base64


 on peut mettre le  deployment et le service dans le même fichier .yaml 

## Integration du fichier du ConfigMap

kubectl apply -f mongo-config.yaml

## Integration du fichier du Secret

kubectl apply -f mongo-config.yaml

## Integration du fichier du deployment

kubectl apply -f mongo.yaml


minikube ip 

kubectl get all
la partie mongo doit etre dans un statefulset 

## Pour palier   au  bug quand  l'image n'arrive pas a se lancer 
minikube ssh docker pull