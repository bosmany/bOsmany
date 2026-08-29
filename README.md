<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=180&section=header&text=Bilal&fontSize=56&fontColor=ffffff&fontAlignY=38&desc=DevOps%20%2F%20Platform%20Engineer%20%E2%80%94%20building%20toward%20AI%20infrastructure&descAlignY=58&descSize=18" width="100%" alt="Bilal" />

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=20&pause=1200&color=2C5364&center=true&vCenter=true&width=700&lines=Infrastructure+as+Code+%7C+Terraform+%2B+Ansible;Kubernetes+%2B+Observability+%28Prometheus%2FGrafana%29;CI%2FCD+Pipelines+%7C+GitHub+Actions;LLM+Agents+%2B+Multi-Agent+Orchestration;MLOps+%7C+Train+%E2%86%92+Serve+%E2%86%92+Monitor" alt="Typing SVG" />

</div>

<br/>

I design and automate the systems that ship and run software — infrastructure
as code, container orchestration, CI/CD pipelines — and increasingly, the
engineering underneath LLM applications: retrieval, tool-use, multi-agent
orchestration, and model fine-tuning.

> Every repo below states, in its own README, exactly which commands were run
> to validate it — `terraform validate`, `helm template | kubeconform`,
> `pytest`, a live `docker run` + `curl` against the running container. I'd
> rather ship a shorter list of things that demonstrably work than a longer
> list of things that might.

<br/>

<div align="center">

### Infrastructure & Cloud
<img src="https://skillicons.dev/icons?i=terraform,aws,ansible,linux,bash&perline=5" alt="Infrastructure stack" />

### Containers, Orchestration & CI/CD
<img src="https://skillicons.dev/icons?i=docker,kubernetes,githubactions,prometheus,grafana&perline=5" alt="Containers and CI/CD stack" />

### AI / ML
<img src="https://skillicons.dev/icons?i=python,pytorch,fastapi,git&perline=5" alt="AI/ML stack" />

</div>

<br/>

## Featured projects

<table>
<tr>
<td width="50%" valign="top">

**[terraform-aws-cicd-platform](https://github.com/bosmany/terraform-aws-cicd-platform)**

Modular Terraform (VPC / ECS Fargate / RDS) across dev & prod environments,
Ansible config management, and a GitHub Actions pipeline that lints,
validates, and security-scans (Checkov, tfsec, Trivy) on every PR.

![Terraform](https://img.shields.io/badge/Terraform-844FBA?logo=terraform&logoColor=white&style=flat-square)
![AWS](https://img.shields.io/badge/AWS-FF9900?logo=amazonaws&logoColor=white&style=flat-square)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?logo=ansible&logoColor=white&style=flat-square)

</td>
<td width="50%" valign="top">

**[k8s-observability-stack](https://github.com/bosmany/k8s-observability-stack)**

A hand-written Helm chart (HPA, PDB, NetworkPolicy, ServiceMonitor) for a
real instrumented service, plus a Prometheus/Grafana/Alertmanager layer with
custom dashboards and alert rules — validated with `helm lint`,
`kubeconform`, and `promtool`.

![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white&style=flat-square)
![Helm](https://img.shields.io/badge/Helm-0F1689?logo=helm&logoColor=white&style=flat-square)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white&style=flat-square)

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[multi-agent-orchestrator](https://github.com/bosmany/multi-agent-orchestrator)**

A DAG-based multi-agent framework on the Claude API: a Planner decomposes a
task into a dependency graph, specialist agents execute subtasks
concurrently where independent, and a Critic drives bounded revision loops
— shared structured state via a typed blackboard, not free-text scratchpad.

![Anthropic Claude](https://img.shields.io/badge/Claude%20API-d97757?logo=anthropic&logoColor=white&style=flat-square)
![Python](https://img.shields.io/badge/asyncio-3776AB?logo=python&logoColor=white&style=flat-square)
![Pytest](https://img.shields.io/badge/tested-pytest-0A9EDC?logo=pytest&logoColor=white&style=flat-square)

</td>
<td width="50%" valign="top">

**[llm-finetuning-lab](https://github.com/bosmany/llm-finetuning-lab)**

A real LoRA fine-tuning pipeline: PEFT adapter training on a small model,
before/after evaluation, post-training quantization — actual loss curves
and metrics generated and committed, not simulated.

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white&style=flat-square)
![HF Transformers](https://img.shields.io/badge/%F0%9F%A4%97%20Transformers-yellow?style=flat-square)
![PEFT/LoRA](https://img.shields.io/badge/PEFT-LoRA-8A2BE2?style=flat-square)

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[claude-rag-agent](https://github.com/bosmany/claude-rag-agent)**

A retrieval-augmented, tool-using agent on the Anthropic Messages API —
hand-rolled multi-turn tool-call loop, real chunking/retrieval pipeline, 57
passing tests with zero network calls.

![Anthropic Claude](https://img.shields.io/badge/Claude%20API-d97757?logo=anthropic&logoColor=white&style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white&style=flat-square)
![Pytest](https://img.shields.io/badge/tests-57%20passing-0A9EDC?logo=pytest&logoColor=white&style=flat-square)

</td>
<td width="50%" valign="top">

**[mlops-pipeline](https://github.com/bosmany/mlops-pipeline)**

An end-to-end ML pipeline: train → quality-gated evaluation → versioned
artifact → FastAPI serving, containerized so the model trains *during* the
Docker build and CI smoke-tests the live container.

![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white&style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white&style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white&style=flat-square)

</td>
</tr>
</table>

<br/>

## Get in touch

<div align="center">

[![Email](https://img.shields.io/badge/Email-osmanybilal%40gmail.com-2C5364?style=for-the-badge&logo=gmail&logoColor=white)](mailto:osmanybilal@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-%40bosmany-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bosmany)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=100&section=footer" width="100%" alt="" />

</div>
