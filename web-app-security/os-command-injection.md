# 💻 OS Command Injection

## Visão Geral & Conceito (AppSec)
Ocorre quando a aplicação passa dados fornecidos pelo usuário para um comando do sistema operacional sem a devida sanitização ou isolamento. Isso permite que instruções adicionais
do sistema sejam interpretadas pelo terminal do servidor.

## Detecção & Monitoramento (SecOps)
- **Análise de Logs:** Buscar por metacaracteres de shell em parâmetros de requisições HTTP (como `;`, `|`, `&&`, `` ` ``).
- **Monitoramento de Processos:** Criar alertas para o surgimento de processos filhos inesperados (ex: `bash`, `sh`, `cmd.exe`) disparados pelo processo da aplicação web.
