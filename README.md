# nginx-k8s-example

                               +------------------+
                               |                  |
                               |  Internet        |
                               |                  |
                               +------------------+
                                      |
                                      | (Access Denied)
                                      |
                                      v
              +--------------------------------------------------+
              |                                                  |
              |    Kubernetes Cluster (Namespace: <namespace>)   |
              |                                                  |
              |    +---------------------------------------+     |
              |    |                                       |     |
              |    |    +----------------------+           |     |
              |    |    |                      |           |     |
              |    |    |  NGINX Pod (app: nginx)|           |     |
              |    |    |                      |           |     |
              |    |    +----------------------+           |     |
              |    |    |                                       |     |
              |    |                                       |     |
              |    |                                       |     |
              |    |    +----------------------+           |     |
              |    |    |                      |           |     |
              |    |    |  Debug Pod (Access Denied)|       |     |
              |    |    |                      |           |     |
              |    |    +----------------------+           |     |
              |    |                                       |     |
              |    +---------------------------------------+     |
              |                                                  |
              |                                                  |
              +--------------------------------------------------+



