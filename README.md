# README – Lab Microsoft Azure: Localizando Serviços por Categoria

## Introdução

Este documento resume os aprendizados do laboratório sobre como localizar e entender serviços no portal Microsoft Azure, além de tópicos relacionados como SLA, alta disponibilidade, armazenamento, segurança, custos e monitoramento.

---

## Serviços e Categorias

O Azure oferece uma ampla gama de serviços organizados em categorias específicas. Por exemplo, na categoria **Análise**, encontramos serviços como:
- Analysis Services
- HDInsight Clusters
- Data Factories
- Data Lake Analytics
- Data Lake Storage Gen1
- Azure Databricks
- Microsoft Graph Data Connect
- Azure HDInsight em clusters AKS

Essa estrutura facilita encontrar rapidamente o que você precisa no portal Azure.

---

## SLA e Alta Disponibilidade

O SLA (Service Level Agreement) representa o compromisso de disponibilidade do serviço:
- **99%** → até 1,68h de indisponibilidade/semana (~7,2h/mês)
- **99,9%** → até 10min de indisponibilidade/semana (~43min/mês)

Máquinas virtuais podem ser configuradas com redundância entre regiões para garantir resiliência e melhorar o desempenho, mas isso pode impactar os custos.

---

## Criação de Máquinas Virtuais

Na criação de uma VM, configuramos:
- Nome
- Região
- Zona de disponibilidade
- Sistema operacional
- Tamanho
- Tipo de segurança e autenticação (usuário administrador)

Outros ajustes incluem disco, rede, gerenciamento, monitoramento e desktop remoto.

**Nota:** Todos os recursos precisam estar associados a um **grupo de recursos**.

---

## Data Centers

O site [datacenters.microsoft.com/globe/explore](https://datacenters.microsoft.com/globe/explore) oferece um mapa 2D/3D interativo com a localização global dos datacenters Azure.

---

## Armazenamento

Principais configurações:
- Nome único da conta
- Região (considerando latência e custo)
- Desempenho: Standard ou Premium
- Redundância: LRS, GRS, ZRS ou GZRS

Tipos disponíveis:
- Containers (pastas com opção de backup)
- Compartilhamento de arquivos (conexão SMB)
- Filas (mensageria)
- Tabelas (armazenamento estruturado)

---

## Migração de Dados

Ferramentas disponíveis:
- **AzCopy**: linha de comando para transferência rápida.
- **Azure Data Box**:
    - Data Box → até 80TB
    - Data Box Disk → até 35TB
    - Data Box Heavy → até 800TB
    - Data Box Job → até 1TB

---

## Identidade e Segurança

O **Entra ID** gerencia usuários, grupos e permissões, diferente do RBAC (controle baseado em funções).  
Recursos adicionais:
- **Entra Connect**: sincroniza usuários locais para a nuvem.
- Recuperação de contas deletadas: até 30 dias.

---

## Defender for Cloud

Ferramenta nativa para monitoramento e recomendações de segurança no ambiente Azure.

---

## Calculadoras de Custos

Duas calculadoras disponíveis:
- Estimativa de preços dos recursos.
- **TCO (Total Cost of Ownership)**: cálculo de economia na migração on-premises → Azure.

---

## Portal de Confiança

Ferramentas e normas de auditoria para garantir compliance, além de recursos como bloqueio de recursos e Purview.

---

## Ferramentas de Implantação

- **Cloud Shell**: execução de comandos PowerShell ou Bash (requer storage account).
- **Bicep**: automação na criação de recursos.
- **Azure Arc**: gerenciamento de servidores externos ao Azure.

---

## Monitoramento

- **Azure Monitor**: insights detalhados da infraestrutura.
- **Service Health**: status e manutenções.
- **Advisor**: recomendações para otimização.

---

## Conclusão

O laboratório permitiu explorar os serviços do Azure, entender como localizá-los por categoria, configurar recursos de forma eficiente e usar ferramentas de gerenciamento, segurança e monitoramento, garantindo alta disponibilidade e controle de custos.
