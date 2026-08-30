<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=180&section=header&text=Bilal%20Osmany&fontSize=48&fontColor=ffffff&fontAlignY=38&desc=DevOps%20%2F%20Platform%20Engineer%20%E2%80%94%20building%20toward%20AI%20infrastructure&descAlignY=58&descSize=18" width="100%" alt="Bilal Osmany" />

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=20&pause=1200&color=2C5364&center=true&vCenter=true&width=700&lines=Infrastructure+as+Code+%7C+Terraform+%2B+Ansible;Kubernetes+%2B+Observability+%28Prometheus%2FGrafana%29;CI%2FCD+Pipelines+%7C+GitHub+Actions;Transformers+%2B+CNNs+%7C+Built+and+Trained+from+Scratch;LLM+Agents+%2B+Multi-Agent+Orchestration;LoRA+Fine-Tuning+%2B+Quantization+%2B+ONNX" alt="Typing SVG" />

</div>

<br/>

I design and automate the systems that ship and run software — infrastructure
as code, container orchestration, CI/CD pipelines — and I go deep on the
machine learning underneath them: implementing a Transformer's attention
math by hand, fine-tuning with LoRA, exporting to ONNX, and orchestrating
multiple LLM agents with real concurrency, not just calling an API.

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

### AI / ML engineering

<table>
<tr>
<td width="50%" valign="top">

**[transformer-from-scratch](https://github.com/bosmany/transformer-from-scratch)**

A GPT-style decoder-only Transformer built from raw PyTorch primitives — no
`nn.Transformer`, no HuggingFace. Hand-verified attention math against
by-hand-computed values, causal masking, weight tying, trained from random
init; beats a bigram baseline by 20% loss / roughly halved perplexity.

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white&style=flat-square)
![From scratch](https://img.shields.io/badge/attention-hand--verified-8A2BE2?style=flat-square)
![Pytest](https://img.shields.io/badge/tests-27%20passing-0A9EDC?logo=pytest&logoColor=white&style=flat-square)

</td>
<td width="50%" valign="top">

**[cv-transfer-learning-pipeline](https://github.com/bosmany/cv-transfer-learning-pipeline)**

ResNet18 transfer learning on FashionMNIST — real data augmentation, Grad-CAM
interpretability, ONNX export with verified numerical equivalence, and a
measured 2.07x PyTorch-vs-ONNX Runtime latency speedup.

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white&style=flat-square)
![ONNX](https://img.shields.io/badge/ONNX-005CED?logo=onnx&logoColor=white&style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white&style=flat-square)

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[llm-finetuning-lab](https://github.com/bosmany/llm-finetuning-lab)**

A real LoRA fine-tuning pipeline: PEFT adapter training on a small
transformer, before/after evaluation (F1 0.41 → 0.69), post-training
quantization — actual loss curves and metrics generated and committed, not
simulated.

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white&style=flat-square)
![HF Transformers](https://img.shields.io/badge/%F0%9F%A4%97%20Transformers-yellow?style=flat-square)
![PEFT/LoRA](https://img.shields.io/badge/PEFT-LoRA-8A2BE2?style=flat-square)

</td>
<td width="50%" valign="top">

**[multi-agent-orchestrator](https://github.com/bosmany/multi-agent-orchestrator)**

A DAG-based multi-agent framework on the Claude API: a Planner decomposes a
task into a dependency graph, specialists execute subtasks with real
`asyncio` concurrency (measured, not assumed), and a Critic drives bounded
revision loops over a typed shared blackboard.

![Anthropic Claude](https://img.shields.io/badge/Claude%20API-d97757?logo=anthropic&logoColor=white&style=flat-square)
![Python](https://img.shields.io/badge/asyncio-3776AB?logo=python&logoColor=white&style=flat-square)
![Pytest](https://img.shields.io/badge/tests-23%20passing-0A9EDC?logo=pytest&logoColor=white&style=flat-square)

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

### DevOps / platform engineering

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
</table>

<br/>

## Get in touch

<div align="center">

[![Email](https://img.shields.io/badge/Email-osmanybilal%40gmail.com-2C5364?style=for-the-badge&logo=gmail&logoColor=white)](mailto:osmanybilal@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-%40bosmany-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bosmany)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=100&section=footer" width="100%" alt="" />

</div>
