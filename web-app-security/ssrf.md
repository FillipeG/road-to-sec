# 🌐 Server-Side Request Forgery (SSRF)

## Visão Geral & Conceito (AppSec)
Vulnerabilidade em que a aplicação web é induzida a realizar requisições HTTP para destinos não previstos. Permite interagir com serviços internos da rede, APIs privadas ou interfaces de
metadados do ambiente de hospedagem que não deveriam estar expostos externamente.

## Detecção & Monitoramento (SecOps)
- **Tráfego de Saída (Egress):** Monitorar conexões de rede originadas pelo servidor web com destino a endereços IP privados ou de loopback (`127.0.0.1`, `10.0.0.0/8`, `169.254.169.254`).
- **Segmentação de Rede:** Aplicação de regras estritas de firewall para limitar os destinos que o servidor da aplicação tem permissão de contatar na rede.
