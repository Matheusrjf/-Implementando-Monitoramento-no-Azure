#Implementando Monitoramento de Recursos no Microsoft Azure 🚨
📌 Sobre o Projeto

Este repositório foi criado como parte do desafio prático da DIO (Digital Innovation One) com o tema: Configuração e Gerenciamento de Monitoramento no Azure.
O objetivo é consolidar o conhecimento sobre as ferramentas de monitoramento do Azure, com foco na detecção de eventos críticos, como a exclusão de uma Máquina Virtual (VM).

🧑‍💻 Principais Tópicos Abordados
1. Por que Monitorar Recursos na Nuvem?
O monitoramento no Azure permite:

✅ Acompanhar o desempenho dos recursos.
✅ Detectar falhas, interrupções ou comportamentos inesperados.
✅ Criar alertas para eventos críticos (ex.: exclusão de VMs, picos de uso, falhas de conectividade).
✅ Gerar métricas e dashboards para análise contínua.

2. Principais Ferramentas de Monitoramento no Azure 🛠️
✅ Azure Monitor
Plataforma central de monitoramento do Azure.

Coleta métricas, logs, e permite criar alertas personalizados.

✅ Log Analytics
Armazena e permite consultas avançadas sobre logs de recursos.

Usa a linguagem de consulta Kusto Query Language (KQL).

✅ Azure Activity Log
Registra todas as operações realizadas em recursos do Azure.

Útil para rastrear exclusões, criações ou alterações de VMs.

✅ Azure Alerts
Permite configurar alertas automáticos com base em métricas ou logs.

Exemplo: Alertar quando uma VM for excluída.

✅ Azure Action Groups
Define as ações que devem acontecer quando um alerta é acionado.

Pode incluir: envio de e-mail, webhook, SMS, ITSM, etc.

3. Como Criar um Alerta de Exclusão de VM 🚦
Etapas no Portal Azure:
Acesse Monitor > Alerts > New alert rule.

Escolha o recurso: Subscription ou Resource Group onde estão as VMs.

Em Condition, selecione o Activity Log Signal.

Escolha o evento:
"Delete Virtual Machine (Microsoft.Compute/virtualMachines/delete)".

Configure um Action Group para definir como será a notificação (ex.: e-mail).

Defina o nome da regra de alerta.

Clique em Create Alert Rule.

4. Exemplos de Outras Situações de Monitoramento ✅
Monitoramento de CPU Alta: Alertas quando o uso de CPU da VM ultrapassa um limite.

Monitoramento de Falhas de Disco.

Monitoramento de Conexões de Rede.

Monitoramento de Disponibilidade de Aplicações (Application Insights).

5. Dicas Úteis ⚡
Sempre use Resource Tags para facilitar filtros nas consultas de logs.

Automatize o envio de relatórios periódicos.

Utilize dashboards customizados para acompanhar vários recursos ao mesmo tempo.

Teste os alertas simulando eventos (ex.: criar e excluir uma VM de teste).
