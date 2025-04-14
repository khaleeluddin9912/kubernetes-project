<<<<<<< HEAD
# kubernetes-project
=======
# 🚀 Node.js App Deployment on Kubernetes

## 👨‍💻 Author
**Mohammed Khaleel Uddin**

## 📋 What I Did:

### 1. **Set Up Kubernetes Cluster** 🌐
   - Installed Minikube and started the cluster:
     ```bash
     minikube start
     ```

### 2. **Created Docker Image for Node.js App** 🐳
   - Wrote a `Dockerfile` for the Node.js app to build the image.
   - Built the image with:
     ```bash
     docker build -t mohammedkhaleel/my-node-app:v2 .
     ```
   - Pushed the image to Docker Hub:
     ```bash
     docker push mohammedkhaleel/my-node-app:v2
     ```

### 3. **Create Kubernetes Deployment** 📦
   - Wrote a `deployment.yaml` file to deploy the app on Kubernetes.
   - Applied the deployment with:
     ```bash
     kubectl apply -f deployment.yaml
     ```

### 4. **Expose the App** 🌍
   - Created a `service.yaml` file to expose the app outside the cluster.
   - Applied the service configuration:
     ```bash
     kubectl apply -f service.yaml
     ```

### 5. **Scale the Deployment** 📈
   - Scaled the app to 3 replicas to ensure high availability:
     ```bash
     kubectl scale deployment my-node-app --replicas=3
     ```

### 6. **Check the Deployment** 🔍
   - Checked the status of pods and deployments:
     ```bash
     kubectl get pods
     kubectl get deployments
     kubectl get services
     ```

### 7. **Access the App** 🌐
   - Retrieved the URL for the app running on Minikube:
     ```bash
     minikube service my-node-service --url
     ```
   - Opened the URL in the browser to verify the app is running. 🖥️

### 8. **Logs and Debugging** 🛠️
   - Checked the logs for any errors using:
     ```bash
     kubectl logs <pod_name>
     ```

---

## 🏁 Conclusion

We successfully deployed a **Node.js app** on **Kubernetes** using **Minikube**. The app was:
- Containerized with **Docker** 🐳
- Deployed on **Kubernetes** 📦
- Exposed with a **NodePort** service 🌍
- Scaled for high availability 📈

Everything is running smoothly! 🎉
>>>>>>> 86ccfa9 (Kubernetes project with deployment, services, screenshots, and README)
