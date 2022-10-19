# config-sync-template-repo

## KCC Template

Replace env vars here with actual values.

```
export GKE_NAME=gke-acm-demo-cluster
export GKE_SA=
export GKE_LOCATION=us-central1
export GKE_CONFIGS_REPO_URL=https://github.com/mbychkowski/gcp-acm-workshop-gke-configs
export TENANT_PROJECT_ID=
```

```
sed -i 's/gke-acm-demo-cluster/${GKE_NAME}/g' templates/*
sed -i 's/${GKE_SA}/gke-acm-demo-cluster/g' templates/*
sed -i 's/${GKE_LOCATION}/gke-acm-demo-cluster/g' templates/*
sed -i 's/${GKE_CONFIGS_REPO_URL}/gke-acm-demo-cluster/g' templates/*
sed -i 's/${TENANT_PROJECT_ID}/gke-acm-demo-cluster/g' templates/*
```

