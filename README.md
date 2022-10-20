# config-sync-template-repo

## KCC Template

Replace env vars here with actual values.

```
export GKE_NAME=gke-acm-demo-cluster
export GKE_SA=gke-primary-pool
export GKE_LOCATION=us-central1
export GKE_CONFIGS_REPO_URL="https://github.com/mbychkowski/gcp-acm-workshop-gke-configs"
export TENANT_PROJECT_ID=qwiklabs-gcp-01-613722232c89
export TENANT_PROJECT_NUMBER=247510278585
export TENANT_PROJECT_SA_EMAIL=qwiklabs-gcp-01-613722232c89@qwiklabs-gcp-01-613722232c89.iam.gserviceaccount.com
```

```
sed -i 's/${GKE_NAME}/'"$GKE_NAME"'/g' ./*.yaml
sed -i 's/${GKE_SA}/'"$GKE_SA"'/g' ./*.yaml
sed -i 's/${GKE_LOCATION}/'"$GKE_LOCATION"'/g' ./*.yaml
sed -i 's/${GKE_CONFIGS_REPO_URL}/'"$GKE_CONFIGS_REPO_URL"'/g' ./*.yaml
sed -i 's/${TENANT_PROJECT_ID}/'"$TENANT_PROJECT_ID"'/g' ./*.yaml
sed -i 's/${TENANT_PROJECT_NUMBER}/'"$TENANT_PROJECT_NUMBER"'/g' ./*.yaml
sed -i 's/${TENANT_PROJECT_SA_EMAIL}/'"$TENANT_PROJECT_SA_EMAIL"'/g' ./*.yaml
```

