# Guardrails da organização — validação isolada

A migração altera somente o workflow guardrails e esta documentação. Preserva os
triggers pull_request e push(main/master), job/check guardrails, contents:read e
as mesmas verificações de CODEOWNERS, Dependabot e refs flutuantes proibidas.

Checkout7.0.1 fixado por SHA, SOURCE_SHA40 explícito (head do PR ou github.sha),
ref exato, persist-credentials:false e conferência git rev-parse. Runner exclusivo
`org-guardrails-run-${{ github.run_id }}`, prazo10min. Exige LinuxARM64 e marcador
/opt/isolation-base-ready; nega9p/virtiofs, SSH_AUTH_SOCK e variáveis de artifacts.
Usa python3 já presente no guest, sem novas dependências ou artifacts/secrets/cloud.

O controlador candidato admite somente este repo/workflow/job após contrato explícito
por SHA40+blob/branch. PR exige same-repo, base main exata, prova GraphQL do workflow
executado e ancestralidade, com freshness/revogação imediatamente antes do token.
Triggers preservados não concedem admissão automática; snapshots novos estão vazios.
Não há publicação, produção, ativação de runner ou alteração de política GitHub.

Teste local do validador e fixtures de preflight não substituem aceite da VM real.
Revisão independente e posterior CI no SHA publicado são pré-condições de uso.
