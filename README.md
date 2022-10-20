# config-sync-template-repo

## KCC Template

Replace env vars here with actual values.

```
export GKE_NAME=gke-acm-demo-cluster
export GKE_SA=gke-primary-pool
export GKE_LOCATION=us-central1
export GKE_CONFIGS_REPO_URL="https://github.com/mbychkowski/gcp-acm-workshop-gke-configs"
export TENANT_PROJECT_ID=qwiklabs-gcp-04-24351b679a98
```

```
sed -i 's/${GKE_NAME}/'"$GKE_NAME"'/g' ./*
sed -i 's/${GKE_SA}/'"$GKE_SA"'/g' ./*
sed -i 's/${GKE_LOCATION}/'"$GKE_LOCATION"'/g' ./*
sed -i 's/${GKE_CONFIGS_REPO_URL}/'"$GKE_CONFIGS_REPO_URL"'/g' ./*
sed -i 's/${TENANT_PROJECT_ID}/'"$TENANT_PROJECT_ID"'/g' ./*
```

