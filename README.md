# nginx-deployment

Deployment and Service yaml files for nginx

## Starting deployment

Clone this repository to the master node and run the following commands

```bash
cd nginx-deployment

kubectl apply -f nginx-deployment.yaml
kubectl apply -f nginx-service.yaml
```

## Status

To see the nodes in the cluster

```bash
kubectl get nodes
```

To see the pods

```bash
kubectl get pods -o wide
```

To see all the deployments

```bash
kubectl get deploy -o wide
```

To see all the services

```bash
kubectl get svc -o wide
```

## URL

To see the nginx welcome page

```bash
curl http://(slave-node-public-ip):30004
```
