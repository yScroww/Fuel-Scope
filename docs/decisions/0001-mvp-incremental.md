# ADR 0001 — MVP incremental

Status: proposto, pendente de validação da fonte.

## Contexto

O projeto deve demonstrar engenharia de dados explicável e ser implementado pelo autor em pequenas entregas.

## Decisão

Começar com um estado e um combustível, Pandas, PostgreSQL e Streamlit. A ingestão inicial será manual por comando Python. Separar raw, staging e analytics e manter rastreabilidade até o arquivo de origem.

## Consequências

Menor custo de operação e foco em contratos, idempotência e métricas. API, agendamento, modelos e deploy ficam para fases posteriores. O recorte será revisto se a cobertura dos dados for insuficiente.
