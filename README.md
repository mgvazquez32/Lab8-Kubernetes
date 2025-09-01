# Desafío 8 - Kubernetes (NestJS + MongoDB)

Este repo contiene manifiestos de Kubernetes para desplegar la app **NestJS** del Desafío 5
junto a **MongoDB**, conectados entre sí dentro del Namespace `desafio8`.

## Pasos

minikube start
kubectl get nodes

minikube image build -t app-template-nestjs:local .

Evidencias:

kubectl get pods -n desafio8
kubectl get svc -n desafio8
kubectl get pvc -n desafio8
kubectl logs deploy/app -n desafio8 --tail=100
curl -i http://$(minikube ip):30080/
