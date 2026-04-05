# kissterra-images

kissterra-images to store images for later use them publicly

## Getting Started

### Example access image from public HTML:
```![Kissterra IDP|200](https://raw.githubusercontent.com/kissterra/kissterra-images/master/images/kissterra_idp.png)```

### Prerequisites

- Docker
- Make (optional)

### Local Development

```bash
# Clone the repository
git clone git@github.com:kissterra/kissterra-images.git
cd kissterra-images

# Build
docker build -t kissterra-images .

# Run
docker run -p 8080:8080 kissterra-images
```

### Running Tests

```bash
# Run unit tests
docker compose run --rm app test
```

## CI/CD

This repository uses GitHub Actions for CI/CD:

- **Build & Test** — Runs on every push and PR to `master`
- **Docker Build** — Builds and pushes Docker image to ECR

## Deployment

Deployments are managed via ArgoCD. See the [k8s-manifests](https://github.com/kissterra/k8s-manifests) repository.

## Team

**Owner:** Kissterra DevOps

## Links

- [ArgoCD](https://argocd.kissterra.com)
- [Port.io](https://app.port.io)
- [Jira Board](https://kissterra-tech.atlassian.net/jira/software/projects/KM/boards/68)
