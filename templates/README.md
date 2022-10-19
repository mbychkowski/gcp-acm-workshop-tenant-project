
# KCC Template

Replace env vars here with actual values.

```
export GKE_NAME
export GKE_SA
export GKE_LOCATION
export GKE_CONFIGS_REPO_URL
export TENANT_PROJECT_ID
```

sed -i 's/${GKE_NAME}/gke-acm-demo-cluster/g' templates/*