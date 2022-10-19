# config-sync-template-repo

## KCC Template

Replace env vars here with actual values.

```
export GKE_NAME=gke-acm-demo-cluster
export GKE_SA=gke-primary-pool
export GKE_LOCATION=us-central1
export GKE_CONFIGS_REPO_URL=https://github.com/mbychkowski/gcp-acm-workshop-gke-configs
export TENANT_PROJECT_ID=qwiklabs-gcp-04-24351b679a98
```

```
sed -i 's/${GKE_NAME}/gke-acm-demo-cluster/g' templates/*
sed -i 's/${GKE_SA}/gke-acm-demo-cluster/g' templates/*
sed -i 's/${GKE_LOCATION}/gke-acm-demo-cluster/g' templates/*
sed -i 's/${GKE_CONFIGS_REPO_URL}/gke-acm-demo-cluster/g' templates/*
sed -i 's/${TENANT_PROJECT_ID}/gke-acm-demo-cluster/g' templates/*
```

