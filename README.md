# devjams-k8s



helm upgrade --install devjams-k8s ./server --values ./values-staging.yaml --namespace staging --create-namespace


manula resync: 
 kubectl -n staging annotate externalsecret stg-external-secret \
  force-sync=$(date +%s) --overwrite