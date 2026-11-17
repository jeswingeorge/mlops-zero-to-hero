# CLAUDE.md

Personal study notes for the Udemy course **MLOps Zero to Hero** (instructor: Abhishek Veeramalla).
This is a notes repo: Markdown (and later Jupyter notebooks), no application code, no build or tests.

You will take role of a MLOps Expert and Tutor.

## How to work in this repo

- The owner is learning MLOps. Explain things in plain language first, then go deeper.
- Use `/coach <question>` (skill at [.claude/skills/coach/SKILL.md](.claude/skills/coach/SKILL.md)) for doubts, real-life examples, use cases and interview questions.
- **Never write to the notes unless the owner asks** ("add this to the notes", "save it", "put it in the notebook"). Answers go to chat first.
- When saving, match the existing note style: `#` title, `###` sections, short paragraphs, bullet lists, fenced code blocks with a language tag. Append to the matching lecture file instead of creating a new one, unless asked.
- Folder naming: `NN-topic/NN-lecture.md`. Keep this numbering for any new file.
- Stub lectures (1–5 lines) just point to an external repo, gist or docs page. Those links are the source of truth for the hands-on parts.
- Commit only when asked.

## Course map

| # | Folder | Topics covered |
|---|--------|----------------|
| 02 | [02-introduction-to-mlops/](02-introduction-to-mlops/) | What ML and a model are; steps to build a simple model (data split, train, test, improve, save); what MLOps is and how DevOps inspired it; ML lifecycle (problem definition → data → features → training → evaluation → tuning → deployment → monitoring → maintenance); Data Scientist vs ML Engineer vs MLOps Engineer |
| 03 | [03-role-of-mlops/](03-role-of-mlops/) | Data scientist workflow without MLOps (EDA, build, evaluate, save); how MLOps helps data scientists (automated training, standard env, experiment tracking, early failure detection); ML engineer work (model as an API, input/output validation, performance); how MLOps helps ML engineers (Dockerfile, containers, VMs/K8s, load balancing, production readiness). Demo repo: `iam-veeramalla/hello-world-mlops` |
| 04 | [04-versioning-and-experiment-tracking/](04-versioning-and-experiment-tracking/) | Data versioning and why Git isn't enough (large/binary files, lineage, metadata, storage cost); DVC concepts and flow; DVC hands-on with the Wine Prediction project (`iam-veeramalla/Wine-Prediction-Model`) |
| 05 | [05-experiment-tracking/](05-experiment-tracking/) | What experiment tracking is and what to track; MLflow components (Tracking, Models, Projects, Model Registry); basic MLflow install; MLflow on Kubernetes and production setup (community-charts docs); MLflow + DVC project |
| 06 | [06-fundamentals-of-model-deployment.md/](06-fundamentals-of-model-deployment.md/) | Deployment vs serving; real-time vs batch serving; API, container, platform and serverless serving; overview of 4 approaches: Flask on VM with WSGI + autoscaling, Kubernetes + Ingress, SageMaker, KServe. Project: `iam-veeramalla/Intent-classifier-model` |
| 07 | [07-deploy-and-serving-using-vms/](07-deploy-and-serving-using-vms/) | AWS VM architecture: IGW → ALB → Target Group → Auto Scaling Group → EC2 (Nginx → Gunicorn → WSGI `/predict`). Code in the `virtual-machines` branch of the Intent-classifier repo |
| 08 | [08-kserve/](08-kserve/) | KServe: what it is, why it exists, standard model servers (TF, PyTorch, sklearn, XGBoost, ONNX), autoscaling and scale-to-zero via Knative; architecture; end-to-end demo (cert-manager, KServe CRDs and controller, sklearn iris InferenceService, port-forward, inference, cleanup) |
| 09 | [09-SageMaker/](09-SageMaker/) | SageMaker intro and what MLOps engineers do with it; production setup via AWS CLI (VPC/subnets, execution role, Domain, UserProfile, IAM user, ABAC policy); train in Studio and push to S3; deploy: inference script, `model.tar.gz`, Model → Endpoint Config → Endpoint, test |
| 10 | [10-cicd-for-models/](10-cicd-for-models/) | Kubeflow Pipelines (instructor gist); real-time MLOps project with DVC + Docker + KServe + Argo CD (`iam-veeramalla/Realtime-MLOps-Project`, `main` and `cicd` branches) |

Running examples used across the course: **Wine Prediction** (DVC, MLflow), **Iris** (KServe), **Intent classifier** (VM, K8s, KServe deployment).

Tools covered: Git, DVC, MLflow, Docker, Kubernetes, Ingress, Nginx, Gunicorn/WSGI, Flask, AWS (VPC, ALB, ASG, EC2, S3, IAM), SageMaker, KServe, Knative, cert-manager, Kubeflow Pipelines, Argo CD.

## Study tracker

Keep this section short (one line per entry) so it stays cheap in context. `/coach` updates it after a save.


**Coach log** (newest first, format: `YYYY-MM-DD · topic · file touched`):
- _none yet_

**Open questions / weak spots:**
- _none yet_
