# Helm Conditional Dependency
 - Conditions should be added to any dependencies that are optional.
 - These are added at in the `chart.yaml` under the dependency 
   e.g
   Where `apidocs` is the chart name of the dependency.

  ```
  apiVersion: v2
  name: myapplication
  description: A Helm chart for Kubernetes
  type: application
  version: 0.1.0
  appVersion: 1.0
  dependencies:
   - name: apidocs
     condition: apidocs.enabled
  ```
- [Stackoverflow](https://stackoverflow.com/questions/54032974/helm-conditionally-install-subchart)



