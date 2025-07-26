# ☁️ GCP Labs – Cloud Security

Laboratórios práticos focados em **segurança na nuvem com Google Cloud Platform**, com ênfase em boas práticas, IAM, rede, monitoramento e infraestrutura como código segura.

---

## 💡 Objetivo

Capacitar o profissional a:

- Criar e proteger ambientes na GCP
- Gerenciar permissões com IAM e políticas de segurança
- Proteger VPCs com regras de firewall e VPNs
- Auditar e monitorar atividades na nuvem
- Automatizar provisionamento com Terraform

---

## 🚀 Projetos disponíveis

| Projeto | Descrição | Tecnologias |
|---------|-----------|-------------|
| Infra segura GCP com Terraform | Criação de VPC, firewall, instâncias e IAM | Terraform, GCP Compute, IAM |
| Auditoria e Logging | Ativação e análise de Cloud Audit Logs | GCP Logging, Monitoring |
| IAM granular e seguro | Configuração de papéis mínimos para serviços | GCP IAM, Service Accounts |
| Scanner de vulnerabilidade | Deploy de scanner em instâncias GCE | Trivy, GCP VM, Shell Script |

---

## 🧰 Stack utilizada

- Google Cloud Console e SDK  
- GCP IAM, Compute Engine, VPC, Logging, Monitoring  
- Terraform, Trivy, Bash Script

---

## 🗂️ Estrutura do projeto

```bash
📁 gcp-labs-cloud-sec/
├── terraform-vpc-secure/
│   ├── main.tf
│   ├── variables.tf
├── iam-policy-lab/
│   ├── role_config.tf
│   ├── docs/
├── audit-logging/
│   ├── enable_logs.sh
│   ├── cloud_log_queries.md
├── vm-trivy-scan/
│   ├── deploy_trivy.sh
│   ├── result.json
```

---

## 🧠 Como rodar localmente

Instale o Google Cloud CLI e autentique:

```bash
gcloud init
gcloud auth application-default login
```

Clone o repositório e vá para um dos labs:

```bash
git clone https://github.com/AndreGoncallez/gcp-labs-cloud-sec.git
cd gcp-labs-cloud-sec/terraform-vpc-secure
```

Inicialize o Terraform e aplique:

```bash
terraform init
terraform plan
terraform apply
```

---

## 🧪 Em breve

- Integração com Cloud Armor e WAF
- Deploy com Cloud Run + identidade segura
- Centralização de logs com Pub/Sub + BigQuery
- Benchmark CIS automático via script
