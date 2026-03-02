<p align="center">
  <img src="public/clawd-logo.png" alt="ClawHub" width="120">
</p>

<h3 align="center">forked from clawhub.ai</h3>

<p align="center">
  <a href="https://github.com/openclaw/clawhub/actions/workflows/ci.yml?branch=main"><img src="https://img.shields.io/github/actions/workflow/status/openclaw/clawhub/ci.yml?branch=main&style=for-the-badge" alt="CI status"></a>
  <a href="https://discord.gg/clawd"><img src="https://img.shields.io/discord/1456350064065904867?label=Discord&logo=discord&logoColor=white&color=5865F2&style=for-the-badge" alt="Discord"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" alt="MIT License"></a>
</p>

[clawhub.ai](https://clawhub.ai/) is the **public skill registry for Clawdbot**: publish, version, and search text-based agent skills (a `SKILL.md` plus supporting files). It is minimalist roadmap designed for fast browsing + a CLI-friendly API, with moderation hooks and vector search. It aims to be the **SOUL.md registry**: publish and share system lore the same way you publish skills.

<p align="center">
  <a href="https://clawhub.ai">ClawHub</a> ·
  <a href="VISION.md">Vision</a> ·
  <a href="docs/README.md">Docs</a> ·
  <a href="CONTRIBUTING.md">Contributing</a> ·
  <a href="https://discord.gg/clawd">Discord</a>
</p>

---

<h1 align="center">UNPLUGistan</h1>

**The intent of UNPLUGistan is freedom from oppressive Computistan forever.** 

Chat your goals on any messaging app and [OpenClaw](https://github.com/openclaw/openclaw) *or your personal, minimalist* **improvement** *upon OpenClaw -- you will IMPROVE your OpenClaw and make it more secure by subtracting vulnerabilities that you do not need* UNPLUGistan is fundamentally about MINIMALIZATION.

The point is to unleash ephemeral AI agents in self-destructing Kubernetes pods that execute silently then vanish—no browsers, no apps, no maintenance. UNPLUGistan can be powered by Talos Linux, k3s, Firecracker, and ROS2, the stack scales down to true zero cost. Your personal Git repo becomes the sole source of truth so technology disappears and real life takes center stage.

***Fork it!*** *UNPLUGistan is living collection of awesome-esque agentic tools ... make your UNPLUGistan your own.*

**First things todo in first hour or so**:
1) READ through the whole list; understand why things are on the list ... *the first two items are what takes most of the hour.*
2) Star/fork your own set 10 most critical repos (eg, OpenClaw, k3s, Talos, ROS2, Firecracker, Cilium, Argo CD, Knative, Kaniko, Distroless) and speedread your way through them.
3) Clone your new UNPLUGistan repo LOCALLY; make some small edits and commit them.
4) Start with the official OpenClaw + k3s one-click install guide in the community (link in repo).
5) *(Perhaps OPTIONAL but recommended -- this could be done later) Add folders per your interests; possible suggestions: `/infrastructure/` (for your k8s yamls), `/openclaw-skills/` (your Git templates), `/ros2-nodes/` (robot integrations), `/docs/`. Turn key repos into Git submodules later.*

The point of UNPLUGistan is mainly education and INTELLIGENCE gathering; do not just start to installing and adding to your FlusterClaw. First, ***just*** seek to understand the lay of the land. The following *stack* of 100 is deliberately over-provisioned with redundancy so you can **pick the absolute minimal subset** (Talos + k3s + OpenClaw + ROS2 + Distroless + Firecracker).

Inform, but MINIMALIZE ... work toward the ideal of *literally* NEVER having think about compute again. The FUTURE dream is for you to chat → agents do → everything dies → you live in.  AT FIRST, don't install and set up anything ... just READ and follow communities making the stuff work.

### 100 Elements of UNPLUGistan

Organized by layer; not priority. Each entry = exactly two sentences (why it matters + how it connects) + official learning URL.

**1-10: Base OS & Kernel (the invisible host)**
1. **Linux Kernel**  
   It is the absolute minimal, auditable foundation that lets every container and pod die instantly without residue. It connects directly to Docker/k8s/ROS2 by exposing hardware and namespaces so OpenClaw agents can spin robotic swarms or ephemeral tasks without you ever touching a terminal.  
   https://github.com/torvalds/linux

2. **Alpine Linux**  
   The smallest production-grade distro (5 MB) for k8s nodes, guaranteeing your entire cluster boots in seconds and consumes almost no resources. It feeds minimalist Docker images and k3s so OpenClaw’s agentic pods stay hyper-constrained and ephemeral.  
   https://alpinelinux.org (mirror: https://github.com/alpinelinux/docker-alpine)

3. **Talos Linux**  
   Immutable, API-driven OS built exclusively for Kubernetes — no SSH, no package manager, zero maintenance ever. It turns your bare metal or cloud into a set-and-forget k8s host that OpenClaw and ROS2 pods talk to directly.  
   https://github.com/siderolabs/talos

4. **Fedora CoreOS**  
   Automatic atomic updates with zero downtime; the safest base when you occasionally need desktop debugging. It layers under k8s so OpenClaw agents can reboot nodes invisibly.  
   https://github.com/coreos/fedora-coreos-tracker

5. **NixOS**  
   Fully declarative configuration — one file defines the entire OS and all dependencies, eliminating “works on my machine” forever. It connects to every IaC tool so your UNPLUG-istan repo becomes the single source of truth.  
   https://github.com/NixOS/nix

6. **k3s**  
   Lightweight certified Kubernetes (single binary, 100 MB) that runs on anything from Raspberry Pi to cloud VPS and scales to zero cost when idle. It is the orchestration backbone that OpenClaw skills and ROS2 nodes use to launch temporary pods.  
   https://github.com/k3s-io/k3s

7. **k0s**  
   Zero-dependency Kubernetes distribution with built-in air-gap support for ultra-secure or robotic edge deployments. It pairs with k3s for hybrid cloud + on-robot swarms that OpenClaw can orchestrate ephemerally.  
   https://github.com/k0sproject/k0s

8. **Flatcar Container Linux**  
   Automatic updates with rollback; the most reliable long-running base for any node that occasionally hosts persistent OpenClaw memory.  
   https://github.com/flatcar/Flatcar

9. **Bottlerocket**  
   AWS-designed minimal OS with only the container runtime — no shell, no package manager, attack surface near zero. It hosts the supervisor pod that OpenClaw uses to spawn temporary task pods.  
   https://github.com/bottlerocket-os/bottlerocket

10. **MicroK8s**  
    Snap-installed single-node k8s perfect for local testing before pushing to cloud ephemeral clusters. It lets you prototype OpenClaw + ROS2 workflows on a laptop then migrate with zero changes.  
    https://github.com/canonical/microk8s

**11-25: Container Runtimes & Extreme-Minimal Builders**
11. **Docker** (Moby) – https://github.com/moby/moby  
12. **Podman** (rootless alternative) – https://github.com/containers/podman  
13. **Buildah** – https://github.com/containers/buildah  
14. **Kaniko** (build inside k8s without Docker) – https://github.com/GoogleContainerTools/kaniko  
15. **Distroless** (Google’s zero-OS images) – https://github.com/GoogleContainerTools/distroless  
16. **Scratch** base images – https://hub.docker.com/_/scratch (docs)  
17. **gVisor** (sandboxed runtime) – https://github.com/google/gvisor  
18. **Firecracker** (microVMs) – https://github.com/firecracker-microvm/firecracker  
19. **Kata Containers** (hardware-isolated pods) – https://github.com/kata-containers/kata-containers  
20. **CRI-O** – https://github.com/cri-o/cri-o  
21. **containerd** – https://github.com/containerd/containerd  
22. **BuildKit** – https://github.com/moby/buildkit  
23. **Earthly** (reproducible builds) – https://github.com/earthly/earthly  
24. **img** (Docker-less builder) – https://github.com/genuinetools/img  
25. **Bazel** (extreme hermetic builds) – https://github.com/bazelbuild/bazel

**26-40: Orchestration & Serverless Scaling**
26. **Kubernetes** (core) – https://github.com/kubernetes/kubernetes  
27. **Knative Serving** (scale-to-zero pods) – https://github.com/knative/serving  
28. **KEDA** (event-driven autoscaling) – https://github.com/kedacore/keda  
29. **Argo Workflows** (agentic DAGs) – https://github.com/argoproj/argo-workflows  
30. **Temporal** (reliable agent orchestration) – https://github.com/temporalio/temporal  
31. **NATS JetStream** (lightweight messaging) – https://github.com/nats-io/nats-server  
32. **Dapr** (sidecar for state) – https://github.com/dapr/dapr  
33. **Kubeflow** (optional ML pipelines) – https://github.com/kubeflow/kubeflow  
34. **Argo CD** (GitOps) – https://github.com/argoproj/argo-cd  
35. **Flux** (GitOps alternative) – https://github.com/fluxcd/flux2  
36. **Helm** (package manager) – https://github.com/helm/helm  
37. **Kustomize** – https://github.com/kubernetes-sigs/kustomize  
38. **Crossplane** (infrastructure from Git) – https://github.com/crossplane/crossplane  
39. **Tekton** (k8s-native CI) – https://github.com/tektoncd/pipeline  
40. **Keptn** (lifecycle automation) – https://github.com/keptn/lifecycle-toolkit

**41-55: Networking, Security & Isolation**
41. **Cilium** (eBPF networking & security) – https://github.com/cilium/cilium  
42. **Istio** (service mesh) – https://github.com/istio/istio  
43. **CoreDNS** – https://github.com/coredns/coredns  
44. **Traefik** (edge router) – https://github.com/traefik/traefik  
45. **Linkerd** (light mesh) – https://github.com/linkerd/linkerd2  
46. **Falco** (runtime security) – https://github.com/falcosecurity/falco  
47. **Kyverno** (policy engine) – https://github.com/kyverno/kyverno  
48. **OPA/Gatekeeper** – https://github.com/open-policy-agent/gatekeeper  
49. **SPIFFE/SPIRE** (zero-trust identity) – https://github.com/spiffe/spire  
50. **cert-manager** – https://github.com/cert-manager/cert-manager  
51. **Vault** (secrets) – https://github.com/hashicorp/vault  
52. **Sealed Secrets** – https://github.com/bitnami-labs/sealed-secrets  
53. **AppArmor** (kernel LSM) – built-in Linux  
54. **SELinux** – built-in  
55. **eBPF** tools (Cilium/BCC) – https://github.com/iovisor/bcc

**56-65: Storage (ephemeral-first)**
56. **tmpfs / emptyDir** (in-memory) – Kubernetes native  
57. **MinIO** (S3 for skills cache) – https://github.com/minio/minio  
58. **Rook** (if you ever need Ceph) – https://github.com/rook/rook  
59. **Longhorn** (light block) – https://github.com/longhorn/longhorn  
60. **Velero** (backup only when needed) – https://github.com/vmware-tanzu/velero  
61-65. (Reserved for your custom ephemeral volume plugins)

**66-75: AI Core & OpenClaw Ecosystem**
66. **OpenClaw** (the brain)  
    The only interface you will ever touch — chat on WhatsApp/Telegram triggers ephemeral k8s pods that execute your vision. It pulls skills from your Git repo and orchestrates the entire UNPLUG-istan stack so you never open a browser again.  
    https://github.com/openclaw/openclaw

67. **ClawHub Skills Registry** – https://www.clawhub.ai  
68. **Ollama** (local models fallback) – https://github.com/ollama/ollama  
69. **LangChain** (skill authoring) – https://github.com/langchain-ai/langchain  
70. **LlamaIndex** – https://github.com/run-llama/llama_index  
71. **Auto-GPT style agents** (community) – https://github.com/Significant-Gravitas/AutoGPT (adapt to OpenClaw)  
72. **CrewAI** – https://github.com/joaomdmoura/crewAI  
73. **OpenDevin** (inspiration) – https://github.com/OpenDevin/OpenDevin  
74. **BabyAGI** – https://github.com/yoheinakajima/babyagi  
75. **MetaGPT** – https://github.com/geekan/MetaGPT

**76-85: Communication & Interfaces**
76. **Matrix** (self-hosted chat bridge) – https://github.com/matrix-org/matrix.org  
77. **n8n** (workflow triggers) – https://github.com/n8n-io/n8n  
78. **Home Assistant** (if you add smart home) – https://github.com/home-assistant/core  
79. **WhatsApp / Telegram bridges** (OpenClaw native)  
80-85. (Your custom OpenClaw messaging connectors)

**86-95: Robotics & Physical World**
86. **ROS2** (core)  
    The standard for internetworking robotic swarms; OpenClaw agents launch temporary ROS2 nodes in k8s pods to control physical hardware while you stay offline.  
    https://github.com/ros2/ros2

87. **MoveIt2** – https://github.com/moveit/moveit2  
88. **Gazebo** (sim) – https://github.com/gazebosim/gazebo-classic  
89. **micro-ROS** (edge robots) – https://github.com/micro-ROS  
90. **Foxglove** (visualization, optional) – https://github.com/foxglove  
91-95. (Your custom ROS2 skill templates)

**96-100: Optimization & Zero-Fiddle Extras**
96. **Prometheus + Thanos** (light metrics) – https://github.com/prometheus/prometheus  
97. **OpenTelemetry** – https://github.com/open-telemetry/opentelemetry-go  
98. **Grafana** (only when you choose to look) – https://github.com/grafana/grafana  
99. **SOPS** (encrypted secrets in Git) – https://github.com/getsops/sops  
100. **Terraform** (cloud provisioning) – https://github.com/hashicorp/terraform

Reality.

Your UNPLUG-istan repo is live. Go claim it and start adding your first skill template. You’ve just eliminated Computistan forever.
