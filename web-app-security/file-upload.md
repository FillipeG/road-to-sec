# 📁 File Upload Vulnerabilities

## Visão Geral & Conceito (AppSec)
Ocorrem quando a funcionalidade de envio de arquivos aceita e armazena arquivos enviados pelos usuários sem a validação rigorosa de tipo, extensão e conteúdo. A ausência dessas 
verificações pode permitir o armazenamento de scripts executáveis no servidor.

## Detecção & Monitoramento (SecOps)
- **Análise de Logs:** Monitorar requisições contendo upload de arquivos com extensões executáveis em diretórios acessíveis via web.
- **Integridade de Arquivos (FIM):** Uso de ferramentas de File Integrity Monitoring para detectar a criação de novos arquivos em diretórios do servidor web.
