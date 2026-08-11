# 📂 Path Traversal (Directory Traversal)

## Visão Geral & Conceito (AppSec)
Vulnerabilidade que ocorre quando a aplicação utiliza entradas do usuário para construir caminhos de arquivos no sistema operacional sem a devida validação. Permite que um agente malicioso 
navegue pelo sistema de arquivos do servidor e leia informações sensíveis.

## Detecção & Monitoramento (SecOps)
- **Análise de Logs:** Monitorar requisições HTTP contendo padrões de navegação de diretório, como `../` ou suas formas codificadas em URL (`%2e%2e%2f`).
- **Defesa Perimetral:** Configuração de regras no WAF para identificar e bloquear a presença de caracteres de travessia de diretório em parâmetros de requisição.
