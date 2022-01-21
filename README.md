# Anthos Configuration Management Directory

This is the root directory for Anthos Configuration Management.

See [our documentation](https://cloud.google.com/anthos-config-management/docs/repo) for how to use each subdirectory.
# Anthos Demo

This repo contains the [GCP microservices demo](https://github.com/GoogleCloudPlatform/microservices-demo). You can apply it to your anthos configuration by running the following commands to enable Anthos Configuration Management. This will syncronise this repo with your cluster(s)

# To activate this repo in your anthos cluster
```
export CLUSTER_NAME=[enter cluster name]
export PROJECT_ID=[enter GCP project ID]
gcloud beta container hub config-management apply --membership=$CLUSTER_NAME --config=./apply-spec.yaml --project=$PROJECT_ID
```



