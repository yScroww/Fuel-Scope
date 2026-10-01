# Contrato de dados — rascunho

**Status:** pendente de validação em um arquivo oficial. Este documento não é um esquema confirmado.

## Hipótese de grão

Uma observação por revenda, produto e data de coleta. Testar unicidade antes de definir constraints.

## Regras propostas

- CNPJ como texto; preservar zeros iniciais.
- Data de coleta como data; horário de ingestão separado.
- Preço decimal com unidade explícita, armazenado em `NUMERIC`.
- Preservar arquivo, checksum, lote e número da linha.
- Duplicatas exatas não multiplicam a fato; conflitos devem ficar rastreáveis.
- Linhas inválidas têm motivo de rejeição e permanecem auditáveis.
- Preços incomuns não são descartados automaticamente.
- Reprocessar o mesmo arquivo não aumenta a quantidade de observações.

## Preencher na atividade 02

Para cada campo: nome original, nome normalizado, tipo, obrigatoriedade, transformação, regra de validação e exemplo real. Documentar separador, encoding, formato de data e decimal após inspeção.
