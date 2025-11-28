# Helm Charts Repository

This repository hosts Helm charts using GitHub Pages.

## Available Charts

### nginx
A sample Helm chart for deploying NGINX web server on Kubernetes.

## Usage

### Add the Helm repository

```bash
helm repo add my-helm-repo https://ravi-rafay.github.io/helm-charts-repo/
helm repo update
```

### Install the nginx chart

```bash
helm install my-nginx my-helm-repo/nginx
```

### Search for available charts

```bash
helm search repo my-helm-repo
```

## Chart Development

### Package a new chart

```bash
helm package charts/nginx -d .
```

### Update the repository index

```bash
helm repo index . --url https://ravi-rafay.github.io/helm-charts-repo/
```

### Commit and push changes

```bash
git add .
git commit -m "Update charts"
git push
```

GitHub Pages will automatically serve the updated repository.
