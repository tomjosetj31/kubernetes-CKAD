# Questions I faced during the CKAD exam

### 1. Create a pod in a namespace

### 2. There is a pod running and make traffic in and out of the pod from specific pods network policies are already there (np with different selectors)

### 3. Create a deployment with some replicas running in a namespace

### 4. Setup an ingress with with different paths

### 5. There is a dockerfile build the dockerfile and export the container as OCI image format.

### 6. Create a cronjob which run every 2 min should succeed, fail this much time should terminate in this much seconds. Create a job from that.

### 7. Create a deployment and use a service account in it

### 8. Create a secret and use it in a pod as env variable

### 9. Create deployment with security context and run as a specific user and enable the privilege escalation false

### 10. Fix a deployment (wrong api version and selector was not present)

### 11. Create a pod with readiness probe (httpget in the /healthz)

### 12. Expose a deployment as a service (Nodeport)

### 13. Canary deployment with max 10 pods traffic to the new deployment should be 20%

### 14. Create a service account and use it in a deployment

### 15. A service account exists but it does not have permission to create a pod in a namespace so provide the permission

### 16. Create deployment with resource request and limit limit should be the half of the actual limit setup in a namespace (Using LimitRange or ResourceQuota)
