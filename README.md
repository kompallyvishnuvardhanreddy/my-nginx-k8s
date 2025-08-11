# my-nginx-k8s

This project contains a custom Nginx Docker image and Kubernetes manifests to deploy it.
Requirements:
Docker
Kubernetes (Minikube or any cluster)
kubectl CLI

Dockerfile:
docker build -t my-custom-app:1.0 .

Push Image to Docker Hub:
docker tag my-custom-app:1.0 <your-dockerhub-username>/my-custom-app:1.0
docker push <your-dockerhub-username>/my-custom-app:1.0

Apply Kubernetes Manifests:
kubectl apply -f deployment.yml
kubectl apply -f service.yml

Check Resources:
kubectl get pods
kubectl get svc

Access the Application:
minikube service my-nginx-service

<img width="671" height="484" alt="Screenshot 2025-08-11 194119" src="https://github.com/user-attachments/assets/3691bf59-ab23-46f5-b7d6-c309f07f6c9d" />
<img width="752" height="422" alt="Screenshot 2025-08-11 194310" src="https://github.com/user-attachments/assets/655ddc59-9285-455f-828b-6c3cbfefa8a0" />
<img width="1761" height="520" alt="Screenshot 2025-08-11 194350" src="https://github.com/user-attachments/assets/6ea45ba2-e72e-420f-a7c6-cfc9d05ee076" />
