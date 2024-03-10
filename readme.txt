

https://kubernetes.io/docs/tutorials/stateful-application/zookeeper/

https://kazoo.readthedocs.io/en/latest/api.html

    for i in 0 1 2; do echo "=== k-$i ==="; k exec zk-$i --  zkServer.sh status; done

    kubectl exec zk-0 -- zkCli.sh create /hello world

    kubectl exec zk-1 -- zkCli.sh get /hello
