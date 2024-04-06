# nlw-unite-devops

https://hub.docker.com/

docker build -t passin:v1 .
docker image ls
docker run -p 3001:3333 -d passin:v1
docker ps
docker ps -a
docker logs <id_container>
docker stop <id_container>
docker rm <id_container>

docker-compose up --build -d
docker-compose down
docker-compose up

k3d cluster create nlw-unite --servers 2

kubectl config use-context k3d-nlw-unite
kubectl cluster-info
kubectl
kubectl get node
kubectl get pods
kubectl get ns
kubectl get pods -n kube-system

kubectl create ns test
kubectl apply -f k8s/deployment.yaml -n test

helm create deploy

kubeclt create ns nlw-helm
helm upgrade --install passin ./deploy -n nlw-helm

https://argoproj.github.io/cd/

kubectl delete ns test
