# OCI Identity: Gestão de Identidade Avançada e Recuperação de Desastres (DR) com Terraform ☁️🔐

Este projeto foi desenvolvido como aplicação prática dos meus estudos em **Gestão de Identidade e Acesso (IAM)** no Oracle Cloud Infrastructure (OCI). O repositório demonstra como provisionar e configurar **Domínios de Identidade (Identity Domains)** customizados, preparando a arquitetura para cenários críticos de **Recuperação de Desastres (DR) em regiões remotas**.

## 🎯 Cenário de Negócio Aplicado

Para atender a requisitos de conformidade e alta disponibilidade, foi estruturado um domínio de identidade dedicado para aplicações críticas:

* **Nome do Domínio:** `AA-Demo`
* **Descrição:** Domínio de demonstração para o Curso AA.
* **Tipo de Domínio:** `Oracle-apps-premium` (Habilita recursos avançados de segurança, integração com apps Oracle/SaaS e governança corporativa).
* **Foco em DR:** Configuração preparada para replicação e resiliência bi-regional (Recuperação de desastres em regiões remotas).

## 🏗️ Arquitetura do Repositório

O projeto utiliza **Terraform** para garantir que a infraestrutura de segurança seja replicável, auditável e tratada como código (IaC).

* `main.tf` - Provedor OCI e a declaração do Identity Domain Premium.
* `variables.tf` - Parâmetros customizáveis do domínio (Nome, descrição, tipo).
* `outputs.tf` - Exposição do ID do domínio criado para integrações com aplicações externas.

## 🛠️ Tecnologias Utilizadas
* **Oracle Cloud Infrastructure (OCI)**
* **Terraform (IaC)**
* **OCI Identity Domains (IAM)**

## 🚀 Como Executar Este Projeto

1. **Clonar o repositório:**
   ```bash
   git clone https://github.com
   cd oci-identity-domains-dr-automation
   ```
2. **Inicializar o Terraform e baixar o OCI Provider:**
   ```bash
   terraform init
   ```
3. **Planejar a execução (Gera a prévia do domínio `AA-Demo`):**
   ```bash
   terraform plan
   ```
4. **Aplicar a criação na Oracle Cloud:**
   ```bash
   terraform apply
   ```

---
📌 *Projeto desenvolvido focado em Segurança da Informação, Governança de Nuvem e Continuidade de Negócios (BC/DR).*
