# Backlog e Kanban

Quadro: [FuelScope — MVP](https://github.com/users/yScroww/projects/1).

Trabalhe na ordem abaixo, respeitando dependências. Limite de trabalho em andamento: **uma atividade**. Estados: Backlog → Ready → In progress → In review → Done (equivalentes a A fazer → Pronto → Em andamento → Em revisão → Concluído). No início, apenas a atividade 01 está pronta; as demais dependem das anteriores.

| Ordem | Atividade | Dependências |
|---|---|---|
| 01 | Validar cobertura e recorte da ANP | nenhuma |
| 02 | Definir contrato de dados e chave | 01 |
| 03 | Preparar ambiente Python e PostgreSQL | 02 |
| 04 | Preservar arquivo bruto e manifest de ingestão | 03 |
| 05 | Implementar leitor e normalização do CSV | 02, 04 |
| 06 | Implementar validação e quarentena | 05 |
| 07 | Carregar raw e staging com idempotência | 03, 06 |
| 08 | Construir dimensões e fato de preços | 07 |
| 09 | Criar métricas SQL semanais | 08 |
| 10 | Construir dashboard básico | 09 |
| 11 | Configurar CI e verificações de qualidade | 03, 06, 07 |
| 12 | Validar execução reproduzível e fechar demo do MVP | 10, 11 |

## Depois do MVP

- Fase 2: ingestão nacional incremental, revisão de arquivos alterados, agendamento, API FastAPI com documentação e testes.
- Fase 3: backtesting temporal contra persistência/média móvel, anomalias explicáveis, monitoramento e deploy.

Essas fases serão decompostas após a avaliação do MVP, para evitar tarefas prematuras. O fechamento exige evidência; criação de pastas não significa implementação concluída.

