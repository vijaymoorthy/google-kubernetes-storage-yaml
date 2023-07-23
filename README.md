# Initial setup 
![image](https://github.com/vijaymoorthy/google-kubernetes-storage-yaml/assets/5792365/efcccef7-2b7d-488d-96ea-a11bac5c889d)
# Persistance Volume claim from pvc-demo.yaml 
## kubectl get persistentvolumeclaim
In order to access persistence volume , we use PVC claim. it is created as given below
![image](https://github.com/vijaymoorthy/google-kubernetes-storage-yaml/assets/5792365/1a113d3a-5b75-4e32-a1dd-2a1efe1ca50c)

# to creat the POD that access the volume using claim
![image](https://github.com/vijaymoorthy/google-kubernetes-storage-yaml/assets/5792365/e0695167-4e6b-4598-b579-97b884745d22)
## To verify that the POC can access volume
### get into the pod
### write the HTML
### try to access the HTML
![image](https://github.com/vijaymoorthy/google-kubernetes-storage-yaml/assets/5792365/38788f2b-84b3-4448-85fd-53d540b342c6)

## to test , if the above pod is realy persistence
![image](https://github.com/vijaymoorthy/google-kubernetes-storage-yaml/assets/5792365/e0de96be-8e50-4aa7-946a-2268e7e7bf35)

# Stateful pod
### creates a StatefulSet that includes a LoadBalancer service and three replicas of a Pod containing an nginx container and a volumeClaimTemplate for 30 gigabyte PVCs with the name hello-web-disk. The nginx containers mount the PVC called hello-web-disk at /var/www/html as in the previous task.

![image](https://github.com/vijaymoorthy/google-kubernetes-storage-yaml/assets/5792365/efe7353a-8dfa-4bd6-a152-69d96833cb0c)


