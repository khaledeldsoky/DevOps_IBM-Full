## 🧭 Project Architecture Overview

```mermaid
flowchart LR
    User -->|Git| GitHubRepo[DevOps_IBM-Full Repo]

    GitHubRepo --> Linux[Linux Basics]
    GitHubRepo --> Git[Git & GitHub]
    GitHubRepo --> Docker[Docker & Containers]
    GitHubRepo --> K8s[Kubernetes]
    GitHubRepo --> CICD[CI/CD Pipelines]
    GitHubRepo --> IaC[Infrastructure as Code]
    GitHubRepo --> Monitoring[Monitoring & Logging]

    Docker --> K8s
    Git --> CICD
    CICD --> Docker
    IaC --> K8s
    K8s --> Monitoring
