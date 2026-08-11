# 🔒 Broken Access Control

## Visão Geral & Conceito (AppSec)
Falha na aplicação de políticas de autorização, onde o sistema não verifica adequadamente se o usuário autenticado possui permissão para acessar determinado recurso ou executar uma ação. 
Envolve cenários de escalação de privilégios vertical (acesso a funções administrativas) e horizontal (acesso a dados de outros usuários).

## Detecção & Monitoramento (SecOps)
- **Análise de Logs:** Monitorar picos de respostas HTTP `403 Forbidden` ou `401 Unauthorized`, que podem indicar tentativas de varredura de endpoints restritos.
- **Auditoria:** Acompanhar alterações de identificadores (IDs de usuário, hashes) em parâmetros de URL ou corpo de requisição originados de uma mesma sessão.
