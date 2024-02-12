# Steps to Reproduce

1. `kubectl apply -f setup/`   
2. Wait until provider kubernetes is ready.
3. `kubectl apply -f providerconfig.yaml`
4. `kubectl apply -f claim.yaml`
5. Bump the api version of the `Object` to `v1alpha2` in `setup/composition.yaml`.
6. `kubectl apply -f setup/composition.yaml` 
7. Check the composite, `kubectl describe composite` 