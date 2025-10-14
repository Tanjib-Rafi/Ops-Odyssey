# Bind least privilege (use built-in edit role) — namespace scoped

```
kubectl -n ci-cd create rolebinding ci-cd-sa-edit \
  --clusterrole=edit \
  --serviceaccount=ci-cd:ci-cd-sa
```

- `edit` allows deploys, configmaps, secrets, replica sets, etc., but not cluster-wide resources (CRDs, clusterroles, nodes, etc.). Good for app deployment.
