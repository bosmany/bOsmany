# Bilal

DevOps / Platform Engineer building toward AI infrastructure — I design and
automate the systems that ship and run software: infrastructure as code,
container orchestration, CI/CD pipelines, and increasingly, the plumbing
around LLM applications (retrieval, tool-use, model serving).

I like projects that are small enough to review in one sitting and honest
about their own limitations — every repo below documents exactly what was
validated and how, not just what it claims to do.

## Stack

**Infrastructure & Cloud**
![Terraform](https://img.shields.io/badge/Terraform-844FBA?logo=terraform&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?logo=amazonaws&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?logo=ansible&logoColor=white)

**Containers & Orchestration**
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?logo=helm&logoColor=white)

**CI/CD & Observability**
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?logo=grafana&logoColor=white)

**AI / ML**
![Anthropic Claude](https://img.shields.io/badge/Claude%20API-d97757?logo=anthropic&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)

**Languages**
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?logo=gnubash&logoColor=white)
![HCL](https://img.shields.io/badge/HCL-844FBA?logo=terraform&logoColor=white)

## Featured projects

| Repo | What it demonstrates |
|---|---|
| [terraform-aws-cicd-platform](https://github.com/bosmany/terraform-aws-cicd-platform) | Modular Terraform (VPC / ECS Fargate / RDS) across dev & prod environments, Ansible config management, and a GitHub Actions pipeline that lints, validates, and security-scans (Checkov, tfsec, Trivy) on every PR. |
| [k8s-observability-stack](https://github.com/bosmany/k8s-observability-stack) | A hand-written Helm chart (HPA, PDB, NetworkPolicy, ServiceMonitor) for a real instrumented service, plus a Prometheus/Grafana/Alertmanager layer with custom dashboards and alert rules — validated with `helm lint`, `kubeconform`, and `promtool`. |
| [claude-rag-agent](https://github.com/bosmany/claude-rag-agent) | A retrieval-augmented, tool-using agent on the Anthropic Messages API — hand-rolled multi-turn tool-call loop, real chunking/retrieval pipeline, 57 passing tests with zero network calls. |
| [mlops-pipeline](https://github.com/bosmany/mlops-pipeline) | An end-to-end ML pipeline: train → quality-gated evaluation → versioned artifact → FastAPI serving, containerized so the model trains *during* the Docker build and CI smoke-tests the live container. |

Every repo above states plainly, in its own README, which commands were
actually run to validate it (`terraform validate`, `helm template | kubeconform`,
`pytest`, live `docker run` + `curl`) — I'd rather a shorter list of things
that demonstrably work than a longer list of things that might.

## GitHub stats

![Bilal's GitHub stats](https://github-readme-stats.vercel.app/api?username=bosmany&show_icons=true&theme=default&hide_border=true)
![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=bosmany&layout=compact&hide_border=true)

## Get in touch

- Email: [osmanybilal@gmail.com](mailto:osmanybilal@gmail.com)
- GitHub: [@bosmany](https://github.com/bosmany)
