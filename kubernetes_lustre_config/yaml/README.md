### Demo steps for creating Lustre's MGS component on K8s

1. Create Persistent Volume for Lustre's MGS component
```
kubectl create -f pv-mgs.yaml
```

2. Create Persistent Volume Claim for Lustre's MGS component
```
kubectl create -f pvc-mgs.yaml
```

3. Create Lustre's MGS Virtual Machine
```
kubectl create -f centos7-lustre-mgs.yaml
```

4. Validate Lustre's MGS Virtual Machine is up and running
```
kubectl get vmis
```