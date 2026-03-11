# Tharlesson Platform

Este espaco centraliza os projetos de plataforma, SRE, DevOps e GitOps que construimos juntos.

## Projetos

| Pasta local | Projeto | Resumo | Repositorio |
| --- | --- | --- | --- |
| `ArgoCD-gitops` | Plataforma GitOps para AWS EKS | Argo CD + Argo Rollouts + Terraform + promocao `dev -> stage -> prod`. | [tharlesson/argocd](https://github.com/tharlesson/argocd) |
| `Atlantis` | Stack Atlantis + GitHub + AWS | Execucao centralizada de IaC com Atlantis em ECS Fargate. | [tharlesson/atlantis](https://github.com/tharlesson/atlantis) |
| `automacoes` | AWS SRE Automation Platform | Plataforma de automacoes SRE em Terraform (governanca, operacao e custos). | [tharlesson/sre-automations](https://github.com/tharlesson/sre-automations) |
| `Jenkins` | Monorepo da Plataforma Jenkins | Controller + agents + JCasC + seed jobs versionados. | [tharlesson/jenkins](https://github.com/tharlesson/jenkins) |
| `observabilidade` | Plataforma de Observabilidade AWS | Observabilidade para EC2/ECS/EKS com OpenTelemetry e metricas. | [tharlesson/observabilidade](https://github.com/tharlesson/observabilidade) |
| `porfolio` | Portfolio em React + Vite | Portfolio pessoal com publicacao via GitHub Pages. | [tharlesson/portfolio](https://github.com/tharlesson/portfolio) |
| `sre-automations` | Automacao Lambda Start/Stop | Automacao de janelas de operacao com AWS Lambda + Scheduler. | [tharlesson/sre-automations](https://github.com/tharlesson/sre-automations) |
| `terraform-import` | Terraform Import (workspace local) | Estrutura de importacao de recursos AWS para Terraform por modulos. | _Sem remoto configurado neste workspace_ |
| `terraform-import-sync-20260310230730` | Terraform Import (sync) | Copia sincronizada do fluxo de importacao para Terraform. | [tharlesson/terraform-import](https://github.com/tharlesson/terraform-import) |
| `terraform-modules` | Terraform AWS Platform Blueprint | Modulos reutilizaveis e stacks multi-conta/multi-ambiente. | [tharlesson/terraform-modules](https://github.com/tharlesson/terraform-modules) |

## Observacoes

- As pastas `automacoes` e `sre-automations` apontam para o mesmo repositorio remoto (`tharlesson/sre-automations`).
- Este README e mantido no repositorio da organizacao `.github` para servir como pagina de perfil.
