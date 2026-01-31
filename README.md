# Infrastructure as Code (IaC)

This repository demonstrates **production-ready Infrastructure as Code (IaC)** practices using Kubernetes, Docker, and CI/CD pipelines. It is designed to showcase how modern backend and platform infrastructure is structured, automated, and maintained in real-world engineering teams.

The goal of this repository is to provide recruiters and hiring managers with a **clear, practical view of my DevOps and cloud-native skills**, rather than isolated demos.

---

## 🔧 Technologies & Tools

- **Kubernetes (K8s)** – container orchestration
- **Docker** – containerization
- **CI/CD Pipelines** – GitHub Actions, Azure DevOps, GitLab CI
- **Monitoring & Observability** – Prometheus, Grafana
- **Code Quality** – SonarQube
- **Databases** – PostgreSQL, MongoDB


---

## 📁 Repository Structure

```text
infrastructure-as-code/
│
├── k8s/                           # Kubernetes manifests
│   ├── monitoring/                # Prometheus & Grafana manifests
│   ├── namespace.yaml
│   │   ├── prometheus
│   │   │   ├── deployment.yaml
│   │   │   ├── service.yaml
│   │   │   └── configmap.yaml
│   │   │   └── instructions.md
│   │   └── grafana
│   │   │   ├── deployment.yaml
│   │   │   ├── service.yaml
│   │   │   └── configmap.yaml
│   │   │   └── instructions.md
│   │   └── jaeger/
│   │   │   ├── deployment.yaml
│   │   │   ├── service.yaml
│   │   │   └── configmap.yaml
│   │   │   └── instructions.md
│   ├── databases/                 # Database manifests
│   │   ├── mongodb/
│   │   │   ├── namespace.yaml
│   │   │   ├── deployment.yaml
│   │   │   ├── service.yaml
│   │   │   └── configmap.yaml
│   │   │   └── instructions.md
│   │   ├── postgres/
│   │   │   ├── namespace.yaml
│   │   │   ├── deployment.yaml
│   │   │   ├── service.yaml
│   │   │   └── configmap.yaml
│   │   │   └── instructions.md
│   │   └── redis/
│   │   │   ├── deployment.yaml
│   │   │   ├── service.yaml
│   │   │   └── configmap.yaml
│   │   │   └── instructions.md
│   │   └── sonarqube/      # SonarQube + PostgreSQL manifests
│   │       ├── deployment.yaml
│   │       ├── service.yaml
│   │       └── configmap.yaml
│   │       └── instructions.md
│
├── docker/                        # I am working on this will include soon
│   ├── sonar/                     # I am working on this will include soon
│   └── other-services/            # Any other custom container images
│
├── pipelines/                     # CI/CD pipeline definitions
│   ├── github-actions/            # GitHub Actions workflows coming soon
│   ├── azure-devops/              # Azure DevOps pipelines coming soon
│   └── gitlab-ci/                 # GitLab CI configuration coming soon
│
├── environments/                  # Environment-specific configs
│   ├── dev/
│   ├── staging/
│   └── prod/
│
├── scripts/                       # Helper scripts
│   ├── deploy.sh
│   └── cleanup.sh
│
├── README.md
└── .gitignore

