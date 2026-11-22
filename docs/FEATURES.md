# Funcionalidades / Features

[Português](../README.md) · [English](../README.en.md)

As funcionalidades abaixo descrevem a V1 documentada e seus dados sintéticos. / The features below describe the documented V1 and its synthetic data.

| Área / Area | Português | English |
|---|---|---|
| Dashboard | Saúde sintética, contagens e atividade recente | Synthetic health, counts and recent activity |
| Infrastructure | Inventário DEMO, ambientes e filtros | DEMO inventory, environments and filters |
| Servers | Detalhes e histórico de métricas sintéticas | Details and synthetic metric history |
| Monitoring | Gráficos, dados tabulares e regras temporais | Charts, tabular data and time-based rules |
| Alerts | Severidade textual, estado e reconhecimento | Textual severity, status and acknowledgement |
| Incidents | Timeline, análise e causa provável heurística | Timeline, analysis and heuristic probable cause |
| Auto-Healing | Prévia, autorização e recuperação simulada | Preview, authorization and simulated recovery |
| Reports | Disponibilidade por amostras e exportações | Sample-based availability and exports |
| Audit | Histórico consultável de ações e resultados | Reviewable history of actions and outcomes |
| Settings | Perfil, tema claro/escuro e densidade | Profile, light/dark themes and density |

## Escolhas de engenharia / Engineering choices

**Português.** Regras consideram duração, banda de recuperação e cooldown, evitando tratar cada amostra como incidente independente. A recuperação não é uma ação silenciosa: existe uma etapa de prévia e uma autorização explícita. A resolução é associada à verificação do estado sintético. Controles locais de autenticação e acesso por papel são documentados, sem alegação de certificação de segurança.

**English.** Rules account for duration, recovery bands and cooldown rather than treating every sample as a separate incident. Recovery is not a silent action: it includes a preview and explicit authorization. Resolution is tied to verification of synthetic state. Local authentication and role-based controls are documented without claiming security certification.

## Cenários / Scenarios

Normal, CPU elevada, disco cheio e serviço indisponível. / Normal operation, high CPU, full disk and unavailable service.

As métricas e os efeitos são simulados; não representam medições nem alterações de infraestrutura real. / Metrics and effects are simulated; they are neither measurements nor changes to real infrastructure.
