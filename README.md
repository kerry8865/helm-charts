# Github Pages use

### 1. Helm chart repo address:
https://kerry8865.github.io/helm-charts/docs/

### 2. Add chart repo:
$ helm repo add github-pages https://kerry8865.github.io/helm-charts/docs/

### 3. Check add chart repo:
$ helm repo list | grep github-pages
NAME        	URL                                             
github-pages	https://kerry8865.github.io/helm-charts/docs/

### 4. Search chart package:
$ helm search mychart
NAME                	CHART VERSION	APP VERSION	DESCRIPTION                
github-pages/mychart	0.1.0        	1.0        	A Helm chart for Kubernetes

### 5. Download chart package:
$ helm fetch github-pages/mychart

### 6. Online install chart:
$ helm install --name=mychart-test --namespaces=default github-pages/mychart
