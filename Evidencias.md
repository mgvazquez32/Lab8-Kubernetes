Evidencias:

Hello World!popesan@popesan:~/lab8-kubernetes/app-template-kubectl get pods -n desafio8 -n desafio8
kubectl get svc -n desafio8
kubectl get pvc -n desafio8
kubectl logs deploy/app -n desafio8 --tail=100
curl -i http://$(minikube ip):30080/
NAME                     READY   STATUS    RESTARTS   AGE
app-6dc9ff5977-qdxkt     1/1     Running   0          41m
mongo-856b4b7d6d-5pz52   1/1     Running   0          41m
NAME        TYPE        CLUSTER-IP      EXTERNAL-IP   PORT(S)          AGE
app-svc     NodePort    10.97.55.238    <none>        3000:30080/TCP   44m
mongo-svc   ClusterIP   10.99.149.143   <none>        27017/TCP        44m
NAME        STATUS   VOLUME                                     CAPACITY   ACCESS MODES   STORAGECLASS   VOLUMEATTRIBUTESCLASS   AGE
mongo-pvc   Bound    pvc-ac41af32-ae21-4ae9-8e46-3a82ecdbb9d1   2Gi        RWO            standard       <unset>                 44m
[Nest] 1  - 09/01/2025, 11:21:29 PM     LOG [NestFactory] Starting Nest application...
[Nest] 1  - 09/01/2025, 11:21:29 PM     LOG [InstanceLoader] AppModule dependencies initialized +22ms
[Nest] 1  - 09/01/2025, 11:21:29 PM     LOG [RoutesResolver] AppController {/}: +10ms
[Nest] 1  - 09/01/2025, 11:21:29 PM     LOG [RouterExplorer] Mapped {/, GET} route +6ms
[Nest] 1  - 09/01/2025, 11:21:29 PM     LOG [NestApplication] Nest application successfully started +6ms
HTTP/1.1 200 OK
X-Powered-By: Express
Content-Type: text/html; charset=utf-8
Content-Length: 12
ETag: W/"c-Lve95gjOVATpfV8EL5X4nxwjKHE"
Date: Tue, 02 Sep 2025 00:03:22 GMT
Connection: keep-alive
Keep-Alive: timeout=5

Hello World!popesan@popesan:~/lab8-kubernetes/app-template-nestjs/k8s$ 

