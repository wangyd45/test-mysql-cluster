# test-mysql-cluster

## 高可用
参考：  
https://github.com/Yolean/kubernetes-mysql-cluster  
http://galeracluster.com/2016/11/introducing-the-safe-to-bootstrap-feature-in-galera-cluster/  
kubectl --namespace=mysql-galear-cluster1 exec -c init-config mariadb-0 -- sed -i "s/safe_to_bootstrap: 0/safe_to_bootstrap: 1/g" /data/db/grastate.dat  
kubectl --namespace=mysql-galear-cluster1 exec -c init-config mariadb-0 -- touch /tmp/confirm-new-cluster  

## m-s
https://www.troyying.xyz/index.php/k8s/3.html  
https://www.jianshu.com/p/509b65e9a4f5  
http://www.jumpbeandev.com/2017/06/01/mysqlcluster/  
https://github.com/jumpjumpbean/k8smysqlcluster  
