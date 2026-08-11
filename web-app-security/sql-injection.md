# 🗄️ SQL Injection (SQLi)

## Visão Geral & Conceito (AppSec)
Vulnerabilidade clássica que ocorre quando entradas do usuário não tratadas são concatenadas diretamente em instruções de banco de dados relacional. Permite interferir no comportamento das consultas originais, 
podendo levar à exposição ou manipulação inadvertida de dados.

## Detecção & Monitoramento (SecOps)
- **Análise de Logs:** Monitoramento de sintaxe SQL em parâmetros de entradas HTTP (como aspas simples `'`, comentários `--`, palavras-chave `UNION`, `SELECT`).
- **WAF:** Implementação de assinaturas de inspeção para bloquear padrões conhecidos de interpolação SQL em campos de entrada.
