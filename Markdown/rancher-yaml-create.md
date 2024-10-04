@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces/Code (main) $ kubectl create -f rancher.yaml 
clusterrole.rbac.authorization.k8s.io/proxy-clusterrole-kubeapiserver created
clusterrolebinding.rbac.authorization.k8s.io/proxy-role-binding-kubernetes-master created
namespace/cattle-system created
serviceaccount/cattle created
clusterrolebinding.rbac.authorization.k8s.io/cattle-admin-binding created
secret/cattle-credentials-23341b8 created
clusterrole.rbac.authorization.k8s.io/cattle-admin created
Warning: spec.template.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms[0].matchExpressions[0].key: beta.kubernetes.io/os is deprecated since v1.14; use "kubernetes.io/os" instead
Warning: spec.template.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution[2].preference.matchExpressions[0].key: node-role.kubernetes.io/master is use "node-role.kubernetes.io/control-plane" instead
deployment.apps/cattle-cluster-agent created
service/cattle-cluster-agent created
@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces/Code (main) $ 