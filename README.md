# Certified Kubernetes Application Developer (CKAD) Exam Preparation

## Core Concepts

Create a namespace:

```bash
k create ns my-namespace
```

Create a pod using the `nginx` image and run a shell command in it.:

```bash
k run nginx --image nginx -- /bin/sh -c "while true; do echo hello; sleep 10; done"
```

Create the k8s manifest for a pod:

```bash
k run nginx --image nginx  --dry-run=client -o yaml > pod.yaml
```

Create a pod and expose traffic on port 80:

```bash
k run nginx --image nginx --port 80
```

Create a deployment using the `nginx` image and run a shell command in it.:

```bash
k create deploy nginx --image nginx -- /bin/sh -c "while true; do echo hello; sleep 10; done"
```

Create the k8s manifest for a deployment:

```bash
k create deploy nginx --image nginx --dry-run=client -o yaml > deploy.yaml
```

Create pod from a manifest file:

```bash
k create -f pod.yaml
```

Create deployment from a manifest file:

```bash
k create -f deploy.yaml
```

Get pods

```bash
k get pods
```

Get pods in all namespaces

```bash
k get pods --all-namespaces or k get pods -A
```

Get deployments

```bash
k get deploy
```

Change the image of a deployment/pod:

```bash
k set image pod/nginx nginx=nginx:1.24.0
```

Get IP address of a pod:

```bash
k get po -o wide
```

Get pods yaml:

```bash
k get po nginx -o yaml
```

Get information about a pod:

```bash
k describe po nginx
```

Get logs of a pod:

```bash
k logs nginx
```

If pod crashes, get the logs:

```bash
k logs nginx -p
```

Execute a command in a pod:

```bash
k exec -it nginx -- /bin/sh
```

Execute a simple command in a pod:

```bash
k run nginx --image nginx -it -- ls
```

Do the same but delete pod after command is executed:

```bash
k run nginx --image nginx --rm -it -- ls
```

Set env variable in a pod:

```bash
k run nginx --image nginx --env="VAR1=value1" --env="VAR2=value2"
```
