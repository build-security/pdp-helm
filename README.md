# Deploy Build Security PDP via Helm

This project creates a sample PDP deployment to a Kubernetes cluster of your choice.

## Filling out the template file

Edit the values-tmpl.yaml file according to your specification:

* Insert the API key & secret that were generated in the build security console. (do not use quotes when setting these values)

* In case you wish the PDP to be initialized with a policy from a Git commit hash (SHA) set the commit SHA in the BUNDLE_COMMIT parameter.

* Set service type to the correct setting according to your deployment type.



## Installing with Helm

`helm install --name-template build-security-pdp ./build-security-pdp  -f values-tmpl.yaml`

* Please note the chart will be installed to your currently configured context.
## Uninstalling with Helm
 `helm uninstall  build-security-pdp`



