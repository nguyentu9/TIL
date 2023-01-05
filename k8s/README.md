### **Create dashboard**

https://github.com/kubernetes/dashboard/blob/master/docs/user/access-control/creating-sample-user.md

```
  kubectl apply -f dashboard-admin.yaml
```

- You should see a service account and a cluster role binding created.

```
  serviceaccount/admin-user created
  clusterrolebinding.rbac.authorization.k8s.io/admin-user created
```

- Get admin token

```
kubectl -n kubernetes-dashboard create token admin-user
```

### Access Dasboard

https://github.com/kubernetes/dashboard/blob/master/docs/user/accessing-dashboard/README.md
