# Camada de Fundação

## Introdução

### Objetivo do Documento
O objetivo deste documento é fornecer diretrizes e estruturas para estabelecer uma camada de fundação sobre a qual os bounded contexts possam construir. Isso inclui detalhes sobre serviços compartilhados, governança de dados, protocolos de comunicação e mais.

### Público-Alvo
Este documento é destinado a todos os membros da equipe envolvidos no projeto, desde desenvolvedores, arquitetos, designers de UX, até analistas de negócios e stakeholders. Ele também será útil para equipes de governança e operações.

### Como Utilizar este Documento
Este documento deve servir como um guia para entender e implementar a camada de fundação que suportará os diversos bounded contexts identificados. Cada seção aborda um aspecto específico que deve ser considerado e definido. O documento deve ser atualizado e revisado conforme o projeto evolui.

## 1. Serviços e Componentes Compartilhados
- **Serviços ou Componentes Comuns**: Quais são os serviços ou componentes comuns que vários bounded contexts utilizarão? (Ex: Um serviço de autenticação compartilhado)
- **Acesso aos Serviços**: Como esses serviços compartilhados serão acessados? (Ex: Via API RESTful com token de acesso)

## 2. Governança de Dados
- **Compartilhamento de Dados**: Como os dados serão compartilhados entre os bounded contexts, se for o caso? (Ex: Utilizar um Data Lake comum)
- **Regras de Propriedade de Dados**: Quais são as regras de propriedade de dados? (Ex: Cada bounded context é dono de seus próprios dados)

## 3. Protocolos de Comunicação
- **Comunicação entre Contextos**: Como os bounded contexts se comunicarão entre si? (Ex: APIs, filas de mensagens, eventos)
- **Padrões de Comunicação**: Quais são os padrões para esses métodos de comunicação? (Ex: JSON para APIs RESTful)

## 4. Protocolos de Segurança
- **Protocolos de Autenticação e Autorização**: Quais são os protocolos comuns para autenticação e autorização? (Ex: OAuth 2.0)
- **Gestão de Credenciais**: Como as credenciais de segurança serão gerenciadas e rotacionadas? (Ex: Utilizando um gerenciador de segredos)

## 5. Stack Tecnológica
- **Stack Tecnológica Comum**: Existe uma stack tecnológica comum que todos os bounded contexts devem seguir? (Ex: Backend em Java, Frontend em React)
- **Diretrizes para Desvios**: Quais são as diretrizes para desviar da stack comum, se necessário? (Ex: Aprovação do arquiteto-chefe)

## 6. DevOps e Implantação
- **Pipelines de CI/CD Comuns**: Quais são os pipelines comuns de CI/CD? (Ex: Jenkins para integração contínua)
- **Coordenação de Implantações**: Como as implantações serão coordenadas entre diferentes bounded contexts? (Ex: Comunicação via Slack ou e-mail)

## 7. Monitoramento e Registro
- **Ferramentas de Monitoramento e Registro**: Quais são as ferramentas compartilhadas para monitoramento e registro? (Ex: Grafana para monitoramento, ELK para registros)
- **Métricas Rastreadas**: Quais métricas devem ser comumente rastreadas? (Ex: Tempo de resposta da API, taxa de erro)

## 8. Documentação
- **Armazenamento de Documentação**: Onde a documentação compartilhada será armazenada? (Ex: Confluence ou Wiki interna)
- **Formato e Estrutura**: Qual é o formato e a estrutura da documentação? (Ex: Markdown, diagramas UML)

## 9. Governança e Conformidade
- **Políticas de Governança**: Quais são as políticas de governança relacionadas a serviços e componentes compartilhados? (Ex: Auditorias regulares)
- **Garantia de Conformidade**: Como será garantido o cumprimento de regulamentações legais e do setor? (Ex: Análise legal trimestral)

## 10. Versionamento e Compatibilidade Retroativa
- **Versionamento de Ativos**: Como as alterações em ativos compartilhados serão versionadas? (Ex: Semantic Versioning)
- **Compatibilidade Retroativa**: Qual é a política para manter a compatibilidade retroativa? (Ex: Manter versões anteriores por 6 meses)

## 11. Tratamento de Exceções e Failover
- **Procedimentos de Exceção**: Quais são os procedimentos padrão para tratamento de exceções? (Ex: Registros detalhados, alertas)
- **Failover e Balanceamento de Carga**: Como o failover e o balanceamento de carga serão gerenciados? (Ex: Uso de load balancers)

## 12. Custos e Faturamento
- **Alocação de Custos**: Como os custos de serviços e ativos compartilhados serão alocados para diferentes bounded contexts? (Ex: Baseado em uso)
- **Mecanismo de Faturamento**: Qual é o mecanismo de faturamento e rastreamento? (Ex: Relatórios mensais)
