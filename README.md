# test-mysql-cluster

## 高可用
参考：  
https://github.com/Yolean/kubernetes-mysql-cluster  
http://galeracluster.com/2016/11/introducing-the-safe-to-bootstrap-feature-in-galera-cluster/  
kubectl --namespace=mysql-galear-cluster1 exec -c init-config mariadb-0 -- sed -i "s/safe_to_bootstrap: 0/safe_to_bootstrap: 1/g" /data/db/grastate.dat  
kubectl --namespace=mysql-galear-cluster1 exec -c init-config mariadb-0 -- touch /tmp/confirm-new-cluster  
