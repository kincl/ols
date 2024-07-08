# OLS Demo

OpenShift Lightspeed demo with local LLM hosting

## Get it working

```
oc create -k ols
oc create -k vllm  # or look at vllm-awq using a quantized model
helm upgrade -i lightspeed-console-plugin charts/openshift-console-plugin -n openshift-lightspeed --set plugin.image=quay.io/openshift/lightspeed-console-plugin:latest
```

## Attribution

| dir | url |
| --- | --- | 
| ols/ | https://github.com/openshift/lightspeed-service |
| vllm/ | https://github.com/rh-aiservices-bu/llm-on-openshift/tree/3330f0313555d6dce43c992bb91ca7315ca4f027/llm-servers/vllm/gitops |
| charts/openshift-console-plugin | https://github.com/openshift/lightspeed-console |
