# Kubernetes


1. **kubectl create deployment httpenv --image=bretfisher/httpenv**:
   - Description: Creates a deployment named "httpenv" using the "bretfisher/httpenv" image.

2. **kubectl scale deploy/httpenv --replicas 5**:
   - Description: Scales the "httpenv" deployment to have 5 replicas.

3. **kubectl expose deployment/httpenv --port 8888**:
   - Description: Exposes the "httpenv" deployment on port 8888.

4. **kubectl get service**:
   - Description: Retrieves information about all services in the cluster.

5. **kubectl get services**:
   - Description: Retrieves information about all services in the cluster (alternative command).

6. **kubectl run tmp-shell --rm -it --image=bretfisher/netshoot --restart=Never -- /bin/bash**:
   - Description: Runs a temporary shell container named "tmp-shell" using the "bretfisher/netshoot" image, with interactive mode enabled.

7. **kubectl expose deployment httpenv --port 8888 --name httpenv-np --type NodePort**:
   - Description: Exposes the "httpenv" deployment on port 8888 with the name "httpenv-np" as a NodePort service.

8. **kubectl get services**:
   - Description: Retrieves information about all services in the cluster.

9. **curl localhost:31396**:
   - Description: Sends a GET request to the localhost on port 31396.

10. **kubectl expose deployment httpenv --port 8888 --name httpenv-lb --type LoadBalancer**:
    - Description: Exposes the "httpenv" deployment on port 8888 with the name "httpenv-lb" as a LoadBalancer service.

11. **kubectl delete service/httpenv-np**:
    - Description: Deletes the service named "httpenv-np".


12. **kubectl create job test --image nginx --dry-run=client -o yaml**:
   - Description: Creates a job named "test" using the "nginx" image, performing a dry run with client-side validation and outputting the YAML configuration.
