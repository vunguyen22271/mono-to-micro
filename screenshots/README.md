# Screenshots

## Deployment Pipeline
* DockerHub showing containers that I have pushed
![Alt text](image.png)
* GitHub repository’s settings showing my GitHub Action CI
Feed CI
![Alt text](image-1.png)

* GitHub Action showing a successful build and deploy job - 
Feed CI build successfully
![Alt text](image-2.png)

- Note: I device to 4 build for case that when I have small change in 1 service, GitHub Action will only build that service.
![Alt text](image-3.png)

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
![Alt text](image-4.png)
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![Alt text](image-6.png)
![Alt text](image-5.png)

* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![Alt text](image-8.png)
![Alt text](image-7.png)
* To verify that you have set up logging with a backend application
```bash
kubectl logs backend-user-855f8bd9c7-f846s 
```
![Alt text](image-9.png)
![Alt text](image-10.png)

Frontend URL: http://a9727382fff2f46329967d369c07d47e-1271900169.us-east-1.elb.amazonaws.com/
![Alt text](image-12.png)

Backend URL: http://a6542bfe502154f7cbcd98c48ce30cbf-1892719817.us-east-1.elb.amazonaws.com:8080/api/v0/feed
![Alt text](image-11.png)
