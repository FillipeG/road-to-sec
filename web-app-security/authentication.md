# 🔑 Authentication Vulnerabilities

## Visão Geral & Conceito (AppSec)
Fragilidades nos mecanismos de validação da identidade do usuário. Incluem falhas na política de credenciais, vulnerabilidades a ataques de força bruta, possibilidade de enumeração de usuários por
respostas e inconsistências na implementação de autenticação multifator (2FA).

## Detecção & Monitoramento (SecOps)
- **Análise de Logs:** Monitorar volumes anômalos de tentativas de login malsucedidas originadas de um mesmo endereço IP ou direcionadas a uma conta específica.
- **Alertas SIEM:** Configuração de alertas para múltiplos erros de autenticação em janelas curtas de tempo e implementação de *rate-limiting* na camada de aplicação/WAF.
