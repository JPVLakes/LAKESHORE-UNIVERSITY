# TI (IT/Technology) - Lakeshore Development

## Visao Geral
- **Missao:** Gerir toda a infraestrutura tecnologica da Lakeshore Development, incluindo sistemas de gestao (BuilderTrend, Const App, QuickBooks), desenvolvimento do software proprio (Lakeshore Software), integracao entre plataformas, suporte tecnico, gestao de acessos, automacao de processos e manutencao de infraestrutura de TI
- **Lider:** Evandro Macedo (Desenvolvedor Principal / Product Owner)
- **Equipe:**
  - Evandro Macedo -- Desenvolvedor Principal, Product Owner do software Lakeshore (+65 horas de entrevistas de requisitos)
  - Luan Leitao -- Equipe TI / Suporte Tecnico, pesquisa de ferramentas IA, onboarding
  - Luciano Holanda (lholanda@lakeshoredevelopmentfl.com) -- Analista de Requisitos, historias de usuario
  - Brendda Maria Sobral (bsobral@lakeshoredevelopmentfl.com) -- Analista de Requisitos, historias de usuario (land development, custom)
- **Reporta a:** Bernardo Lira (CEO)
- **Departamentos relacionados:** TODOS (TI fornece infraestrutura para toda a empresa)
- **Consultores Externos:**
  - Nathan Borges (nathan@manah.digital) -- Consultor de IA/Automacao (Manah Digital), automacao de cotacao com IA
  - Diego Araujo -- Analytics/BI (Power BI, dashboards)
  - Alexandre Lira -- Administracao AWS

## Sistemas em Uso

### 1. BuilderTrend (BT) -- Plataforma Primaria Actual
- **Tipo:** SaaS de gestao de construcao
- **URL:** buildertrend.com
- **Usuarios:** TODOS os departamentos (obrigatorio por directiva CEO)
- **Modulos utilizados:**
  - **Schedule** -- 50 items por job (Land Prep ate Framing, depois via Daily Logs)
  - **Daily Logs** -- 396 entries por job (diario de obra completo com fotos)
  - **To-Do's** -- 53 checklists por job (verificacao de qualidade por fase)
  - **Purchase Orders** -- 122 POs por job ($150,850.83 total no Job 455)
  - **Bills** -- 178 bills por job (pagamentos reais incluindo utilities)
  - **Change Orders** -- Alteracoes de escopo
  - **Subs/Vendors** -- 663 total no sistema (company-wide)
  - **Job Costing Budget** -- Modulo de budget (acesso restrito)
- **Integracao:** QuickBooks (parcial, manual para classes)
- **Dores conhecidas:**
  - Informacao repetida 3x (Daily Logs + Schedule + PO)
  - Carregamento lento, recarregamento apos cada input
  - Tags excessivas e confusas
  - Sem campos padronizados em POs (titulo digitado livremente)
  - Modelo da casa dificil de acessar (multiplas pastas)
- **Status:** Em uso, sera substituido pelo software proprio Lakeshore

### 2. Const App (Hatchbox) -- Nova Plataforma de Gestao
- **URL:** https://6e8kz.hatchboxapp.com
- **Stack:** Ruby 3.4.5 / Rails 8.0.2.1 / Hatchbox PaaS
- **Admin:** miro@lakeshoredevelopmentfl.com
- **Agent accounts:** {dept}@lakeshore.com / Lakeshore2026!

#### System Stats (Admin Panel)
| Parametro | Valor |
|-----------|-------|
| Environment | Production |
| Framework | Rails 8.0.2.1 |
| Language | Ruby 3.4.5 |
| Database | SQLite |
| Database Size | 2,880 KB |
| Total Tables | 130 |
| Total Users | 35 |
| Active Sessions | 63 |
| Total Processes | 16 |
| Internal Processes | 7 |
| External Processes | 7 |
| Process Assignments | 25 |
| Cells (Counties) | 5 |

#### User Distribution
| Role | Count |
|------|-------|
| User | 5 |
| Admin | 25 |
| Master | 1 |
| Supplier Employee | 4 |
| **Total** | **35** |

#### Users with Process Assignments
| User | Email | Role | Processes |
|------|-------|------|-----------|
| A Torres | atorres@lakeshoredevelopmentfl.com | user | Portfolio Management, Quotation |
| F Nery | fnery@lakeshoredevelopmentfl.com | user | Portfolio Management, Quotation |
| Miro | miro@lakeshoredevelopmentfl.com | user | Quotation |
| P Cordeiro | pcordeiro@lakeshoredevelopmentfl.com | user | Portfolio Management, Quotation |
| R Cordeiro | rcordeiro@lakeshoredevelopmentfl.com | user | Portfolio Management, Quotation |
| John Smith | john.handyman@corecraft.internal | supplier_employee | (none) |
| Lisa Chen | lisa.handyman@corecraft.internal | supplier_employee | (none) |
| Maria Garcia | maria.handyman@corecraft.internal | supplier_employee | (none) |
| Robert Johnson | robert.handyman@corecraft.internal | supplier_employee | (none) |

#### Department Admin Accounts
25 admin accounts created for department-specific access:
- purchasing@lakeshore.com, it@lakeshore.com, supervision@lakeshore.com, security@lakeshore.com
- Plus accounts for each of the 21 agent departments

#### 5 Cells (Counties)
1. Cell 1 -- Orange County, Florida
2. Cell 2 -- Charlotte County, Florida
3. Cell 3 -- Marion County, Florida
4. Cell 4 -- Duval County, Florida
5. Cell 5 -- Miami-Dade County, Florida

#### Database Schema (Top Tables by Records)
| Table | Records |
|-------|---------|
| Schema migrations | 286 |
| Services | 156 |
| Model service quantities | 95 |
| Project services | 92 |
| Service components | 92 |
| Material items | 77 |
| Service priorities | 64 |
| Sessions | 63 |

#### 16 Business Processes
**Planning (6):** Service Catalog Management, Portfolio Management, Contract Development, Quotation, Permitting, Accounts Receivable
**Execution (10):** Project Management, Accounts Payable, Client Relations, Construction, Verification, Rework, Concrete, Inspection, Stock, Utility
**Admin (2):** Admin Panel, User Processes

#### 156 Executable Services (Service Catalog)
| Category | Code | Count | Type |
|----------|------|-------|------|
| Inspection | INS | 29 | Inspection |
| Lot-Level Services | LTV | 8 | Construction/Utility |
| Variances | VAR | 1 | Construction |
| Upgrades | UPG | 5 | Construction |
| Cleaning | CLN | 1 | Construction |
| Specialties | SPC | 10 | Construction |
| Exterior/Landscaping | EXT | 15 | Construction |
| Finishes | FIN | 15 | Construction |
| Mechanical (HVAC) | MEC | 4 | Construction |
| Doors | DOR | 7 | Construction |
| Windows | WIN | 6 | Construction |
| Roofing/Framing | ROF | 10 | Construction |
| Masonry | MAS | 5 | Construction/Concrete |
| Electrical | ELC | 5 | Construction |
| Plumbing | PLM | 6 | Construction |
| Foundation | FND | 5 | Construction/Concrete |
| Land Development | LND | 9 | Construction |
| Utilities | UTL | 6 | Utility |
| Permitting | PER | 7 | Planning/Licensing |
| Contract Fees | CON | 2 | Planning |

### 3. QuickBooks -- Sistema Financeiro/Contabil
- **Tipo:** SaaS de contabilidade
- **Usuarios:** Financeiro (Iara, Rayff, Cinthia, Fernanda)
- **Funcoes:**
  - DRE (Demonstracao de Resultados) por projecto
  - Balanco patrimonial
  - T99 reports
  - Conciliacao bancaria (aba "transactions")
  - Classes por projecto (CMER + numero da casa)
- **Integracao com BT:** Parcial, manual
  - Data de vencimento nao serve como criterio
  - Inclusao de classe e super demorado (86 bills/dia = 2 horas)
  - Dois sistemas lentos simultaneamente
- **Dor critica:** Processo de classe manual consome horas diarias

### 4. LakeshoreSoftware.inc -- Plataforma Web (Anterior)
- **URL:** https://lakeshore-frontend.onrender.com
- **Stack:** Full-stack web application on Render
- **Status:** Sendo substituido pelo Const App (Hatchbox)
- **Funcoes:** Construction management, 27 API endpoints para controle de robo GO2
- **Repo:** JPVLakes/LJInspector (GitHub)

### 5. Ferramentas de Comunicacao
| Ferramenta | Uso | Usuarios |
|------------|-----|----------|
| WhatsApp | 90%+ comunicacao com subs | Todos (Scheduling, Compras, Supervisao) |
| Slack | Canais internos, bots, requests | Scheduling, Inspecao, Financeiro, Core Craft |
| Email | Comunicacao formal, termite, utilities | Scheduling (Fase 2), Inspecao, Permits |

### 6. Ferramentas de Produtividade
| Ferramenta | Uso | Usuarios |
|------------|-----|----------|
| Google Sheets | Planilhas pessoais, controle paralelo | Todos (cada pessoa cria a sua) |
| Google Drive | Armazenamento de documentos, projectos | Escritorio de Projetos, Permits |
| ClickUp | Gestao de tarefas (apenas Mauricio) | Scheduling (Fase 1) |
| iPad Notes | Registro de saidas de material | Deposito (Klauser) |

### 7. Ferramentas de Design/Engenharia
| Ferramenta | Uso | Usuarios |
|------------|-----|----------|
| BlueBeam | Quantificacao de materiais (takeoff) | Takeoff (Candida, Gabriela) |
| AutoCAD | Projetos arquitetonicos | Escritorio de Projetos |
| SketchUp | Modelagem 3D | Escritorio de Projetos |
| Enscape/Lumion | Renderizacao | Escritorio de Projetos (Henrique, Victoria) |

### 8. Zorro -- Sistema de OS
- **Usuarios:** Core Craft, Deposito
- **Funcao:** Geracao de Ordens de Servico, purchase orders
- **Status:** Em uso pelo Core Craft

## Infraestrutura de TI

### Cloud (AWS)
| Servico | Uso | Detalhes |
|---------|-----|---------|
| Lambda | Codigo serverless | Escala automatica por demanda |
| EventBridge | Roteamento de eventos | Arquiteturas event-driven, substitui cron jobs |
| Step Functions | Orquestracao de workflows | State machines com condicoes e transicoes |
| Lightsail | Servidores virtuais leves | Slack bots com Flask |
| EC2 Windows | Servidor virtual Windows | Hospeda Power BI Gateway ("power-bi-gateway") |

- **Acesso AWS:** Diego Araujo ou Alexandre Lira -- cadastro via e-mail corporativo com MFA obrigatorio
- **EC2 Gateway:** Conexao via RDP Client, chave .pem "connect-ec2-gateway.pem" (pasta "IT Lakeshore" da conta support)

### Business Intelligence
| Ferramenta | Tipo | Detalhes |
|------------|------|---------|
| Power BI Premium | Dashboards | Conta unica centralizada, gateway em EC2 Windows |
| Dashboard de Construction Data | Custom | Usado por Scheduling Fase 3, QPS para priorizacao |

- **Acesso Power BI:** Credenciais no board do Canva no canal Slack "#qps-tqm-private"
- **Usuarios Power BI:** Diego Araujo, Rost, Joao Paulo Valenca

### Database
| Engine | Uso | Detalhes |
|--------|-----|---------|
| PostgreSQL | Banco principal Lakeshore Software | Credenciais em .docx na pasta "IT Lakeshore" (conta support) |
| SQLite | Banco do Const App (Hatchbox) | 2,880 KB, 130 tabelas, 286 migrations |

### Source Control
- **GitHub:** Repositorio do software proprio Lakeshore
- **Acesso:** Via e-mail support (support@lakeshoredevelopmentfl.com) para convites
- **Organizacao GitHub:** JPVLakes

### Hosting
| Plataforma | Aplicacao | Stack |
|------------|-----------|-------|
| Hatchbox | Const App (nova plataforma) | Rails 8.0.2.1 / Ruby 3.4.5 / SQLite |
| Render | LakeshoreSoftware.inc (anterior) | Full-stack web |
| AWS Lightsail | Slack bots (Flask) | Python/Flask |

### Requisitos Minimos de Hardware
- **Processador:** Intel i5 (ou equivalente) a 3 GHz
- **Problema critico:** CPUs da Lakeshore nao rodam adequadamente AutoCAD, SketchUp, Enscape, BlueBeam
- **Workaround:** Candida e Gabriela usam computadores pessoais
- **Internet campo:** Ruim, impede uso efetivo de Slack e BuilderTrend

### Sites de Condados
| Condado | Ferramenta | Uso |
|---------|-----------|-----|
| Marion | Portal online | Property Appraiser, agendamento de inspecoes |
| Citrus | Portal + E-mail | Inspecoes, permits |
| Orange | Portal | Permits |
| Charlotte | Portal | Permits |
| Alachua | Portal | Permits (permite avancar ate form sem permit) |

- **Playwright scripting:** TI programa acesso automatizado a portais de condados para Permits (task comum de inter-agent)

## Integracoes entre Sistemas

### Integracoes Actuais
| De | Para | Tipo | Status |
|----|------|------|--------|
| BuilderTrend | QuickBooks | Bills e payments | Parcial (manual para classes) |
| Slack | BuilderTrend | Bots de notificacao | Parcialmente configurado, inconsistente |
| Google Drive | Qualquer sistema | Upload manual | Sem integracao (manual) |
| Power BI | PostgreSQL | Gateway EC2 | Funcionando via Power BI Gateway |

### Integracoes Planejadas
| De | Para | Objectivo | Responsavel |
|----|------|-----------|-------------|
| Const App | BuilderTrend | Substituicao completa | Evandro |
| Const App | QuickBooks | Integracao financeira | Evandro + Financeiro |
| Const App | County portals | Automacao de permits e inspecoes | TI (Playwright) |
| IA (Ollama) | Const App | Automacao de cotacoes | Nathan + Evandro |

### Automacao de Cotacao com IA (Projecto Nathan)
- **Objectivo:** Automatizar leitura de PDFs de takeoff e geracao de cotacoes
- **Stack:** Software Lakeshore (Ruby on Rails), IA para leitura de PDFs
- **Status:** Evandro testou com 90% de sucesso
- **Proximo passo:** Nathan recebera branch limitado + PDF modelo 1774 + planilha takeoff

## Processos de TI

### Processo 1: Suporte Tecnico e Manutencao
- **Objectivo:** Resolver problemas de sistemas reportados por qualquer departamento
- **Trigger:** Departamento reporta issue ou solicita IT support
- **SLA:** Critico (< 4h), Alto (< 24h), Medio (< 48h), Baixo (< 1 semana)

### Processo 2: Gestao de Acessos (User Management)
- **Objectivo:** Provisionar e desprovisionar acessos a sistemas
- **Sistemas:** Const App, BuilderTrend, QuickBooks, AWS, GitHub, Power BI, Slack
- **35 users** actualmente no Const App com 4 roles: Master (1), Admin (25), User (5), Supplier Employee (4)

### Processo 3: IT Task Queue (Inter-Agent)
- **Trigger:** Mensagem com prefixo `IT_TASK_REQUEST:`
- **Pattern:** `IT_TASK_REQUEST: <title>\n<description>\nPriority: <level>\nRequesting agent: <name>`
- **Task ID:** IT-NNNN (sequencial)
- **Status:** pending, in_progress, completed, blocked, cancelled
- **Priority:** low, medium, high, critical

**Common Task Types:**
| De | Task | Exemplo |
|----|------|---------|
| Permits | Program county portal access | Playwright scraper para novo condado |
| Financeiro | System integration issues | API connectivity BT-QuickBooks |
| RH | Access management | Provisionar acesso novo funcionario |
| Coordenador | Cross-system health checks | Verificar todos os sistemas |
| QPS | Dashboard update | Novo KPI no Power BI |

### Processo 4: Lista Mestra (Gestao Documental)
- **Objectivo:** Manter documentos da empresa organizados, versionados e acessiveis
- **Documentos IT-01 a IT-11:** Work instructions por departamento
- **Responsavel:** TI em conjunto com QPS (Ana Maria)

### Processo 5: Desenvolvimento do Software Proprio
- **Objectivo:** Desenvolver e manter o Const App (Hatchbox) como substituto do BuilderTrend
- **Responsavel:** Evandro Macedo (Product Owner + Dev principal)
- **Metodologia:** Requirements via entrevistas (+65 horas), historias de usuario
- **Meta:** Substituicao completa do BT (meta inicial Junho 2026)

## Const App -- Modulos Detalhados (Referencia TI)

### Planning Modules

**Service Catalog Management:**
- 156 servicos executaveis em 20 categorias
- Tipos: Construction, Inspection, Planning, Licensing, Utility, Concrete
- Natureza: Labor, Material
- Procurement: Stocked, Quoted, ou nao definido

**Portfolio Management:**
- Modelos de casas com budgets
- Actual Average Cost calculado de projectos anteriores

**Quotation (9 tabs):**
- Take-Off: 128 line items, 19 cost codes
- Material Vendors: 2 registered
- Price Tables: 20 items
- Labor Subs: 68 trade services
- Sub Insurances: Tracking de seguros

**Permitting (6 tabs):**
- Permit Management: Status tracking (Not Started, Applied, Issued, Canceled)
- Application: 4 document types (Energy Calc, Floor Plan, NOC, Survey)
- Revision: 6 stages (91 Review, Building, Zoning, Fee, NOC, Builder's Risk)
- Documentation: Field packets, document stamps
- Modifications & Extensions

**Contract Development:**
- Initialize Contracts: 3 contratos, 5 counties

### Execution Modules

**Inspection (6 tabs):**
- Inspections Flow: 4 modes (Unconfigured, Manual, Assisted, Auto)
- Pre-Inspection Analysis Queue
- Inspection Requests Matrix: 17 categories per project
- Scheduled Inspections
- Reprobation Analysis: Failed inspection patterns

**Verification:**
- Pending PO Verification with photo review
- Site Visits with route planning (coming soon)

**Rework (4 tabs):**
- Queue + Handymen Kanban (4 handymen) + Completed History

**Stock (5 tabs):**
- Levels, Purchases, Pickups, Extraordinary Orders

**Utility (7 tabs):**
- Configurations: 27 items (water/sewage types, energy/water companies, septic docs)
- Water/Sewage Tracking, Energy Tracking
- Monitoring, Septic Documents, Account Closing

## Available Tools

| Tool | Parameters | Returns |
|------|-----------|---------|
| read_daily_logs | date (str, optional), house_id (str, optional) | Daily log entries |
| read_daily_log_detail | log_id (str) | Full daily log record |
| search_daily_logs | query (str) | Matching daily log entries |
| read_schedules | project_id (str, optional), status (str, optional) | Schedule entries |
| read_schedule_detail | schedule_id (str) | Full schedule record |
| read_purchase_orders | status (str, optional), supplier (str, optional) | PO list |
| read_purchase_order_detail | po_id (str) | Full PO record |
| read_inspections | house_id (str, optional), type (str, optional) | Inspection records |
| read_inspection_detail | inspection_id (str) | Full inspection record |
| read_contracts | client_name (str, optional), status (str, optional) | Contract list |
| read_contract_detail | contract_id (str) | Full contract record |
| get_project | project_number (str) or contract_number (str) | Project details |
| get_takeoff_completion | model_id (str) | Takeoff completion percentage |
| get_permits | project_id (str), permit_type (str, optional) | Permit records |
| get_documents | project_id (str) | Document list |
| search_suppliers | query (str) | Matching supplier records |
| check_stock | material (str, optional), below_reorder_only (bool, optional) | Stock levels |
| get_lead | lead_id (str) | Lead record |
| list_leads | status (str, optional) | Lead list |
| get_model | model_id (str) | Model record |
| list_models | status (str, optional) | Model list |

> **Note:** TI has **read-only access** across ALL domains for system monitoring and cross-department diagnostics. No write operations on business data.

## Handoff Triggers

### Outbound (TI sends TO other agents)

| When | Hand off to | Send | SLA |
|------|-------------|------|-----|
| IT task completed (county portal programmed) | permits | INFO: task completion, capability added, IT task ID | 24h |
| System maintenance notification | coordenador | INFO: system affected, downtime window, impact | 24h |
| New employee system access provisioned | rh | INFO: access granted, systems configured | 24h |
| Dashboard updated/new KPI available | qps | INFO: dashboard name, new metrics, access | 24h |
| Software release deployed | coordenador | INFO: release notes, affected modules, known issues | 24h |
| Integration issue resolved | financeiro | INFO: systems reconnected, data verified | 24h |

### Inbound (TI expects FROM other agents)

| When | Hand off to | Send | SLA |
|------|-------------|------|-----|
| New county portal programming needed | permits | INFO: county, portal URL, required capabilities -- IT_TASK_REQUEST | 24h |
| System integration issue reported | financeiro | INFO: system name, error description -- IT_TASK_REQUEST | 24h |
| Access management / user provisioning | rh | INFO: employee, department, access needed -- IT_TASK_REQUEST | 24h |
| Cross-system health check request | coordenador | INFO: systems to check, urgency | 24h |
| New dashboard/report request | qps | INFO: metrics needed, data sources, urgency -- IT_TASK_REQUEST | 48h |
| Hardware issue reported | any agent | INFO: device, issue description -- IT_TASK_REQUEST | 24h |

## Dores e Problemas Conhecidos

### Sistemas
- **Informacao repetida 3x no BT**: Daily logs + Schedule + PO com mesmos dados (todos os depts reclamam)
- **BT lento**: Carregamento pesado, recarregamento de pagina apos cada input
- **Integracao BT-QuickBooks incompleta**: Processo manual de classes consome horas
- **Multiplos sistemas sem integracao**: Zorro, BT, Google Sheets, Notes, WhatsApp, Slack
- **Falta de campos padronizados**: POs com titulos digitados livremente

### Hardware
- **CPUs insuficientes**: Nao rodam AutoCAD, SketchUp, Enscape, BlueBeam
- **Funcionarios usam PCs pessoais**: Candida e Gabriela (Takeoff/Design)
- **Internet ruim no campo**: Impede uso de Slack e BT

### Dados
- **Informacao descentralizada**: Cada pessoa cria sua propria planilha pessoal
- **Controles improvisados**: Nao oficiais, dependem da iniciativa individual
- **Pedidos por multiplos canais**: WhatsApp, verbal, post-it, presencial

## CEO Directives (Bernardo) -- Relevancia para TI

- **BuilderTrend e obrigatorio** para TODOS os departamentos ate substituicao completa
- **ROI-driven**: Toda tecnologia deve mostrar retorno mensuravel
- **Investment priority**: Ferramentas que reduzem cycle time > ferramentas que reduzem headcount
- **Reducao de dependencia individual**: Documentar tudo nos sistemas, cross-train
- **Escala para 500 casas**: Stack tecnologico deve suportar essa meta
- **Concessionaire model**: Sistemas devem ser transferiveis para operadores locais
- **Data-driven decisions**: Se nao pode ser medido, nao pode ser melhorado

## Key Glossary Terms

- **BuilderTrend (BT)**: Plataforma principal de gestao de construcao (SaaS) -- sera substituida
- **Const App**: Nova plataforma de gestao em Hatchbox (Rails 8.0.2.1 / Ruby 3.4.5)
- **QuickBooks**: Sistema financeiro/contabil -- DRE, balanco, T99, conciliacao
- **Zorro**: Sistema de OS (Ordens de Servico) usado pelo Core Craft e Deposito
- **Lista Mestra**: Sistema documental formal (IT-01 a IT-11) gerido por TI + QPS
- **Power BI Gateway**: Servidor EC2 Windows que conecta Power BI a fontes de dados internas
- **Cell**: Unidade operacional por condado no Const App (5 cells activas)
- **Playwright**: Ferramenta de automacao de browser usada para programar acesso a portais de condados
- **IT_TASK_REQUEST**: Protocolo de solicitacao de tarefas IT via mensagem inter-agente
- **Class (QuickBooks)**: Classificacao por projecto para DRE por projecto (CMER + numero casa)

---

## Navegacao

- [Inventario de Ferramentas](02_INVENTARIO_FERRAMENTAS.md) -- Lista completa de sistemas
- [Organograma](01_ORGANOGRAMA.md) -- Equipe de TI e relacoes
- [CEO Directives](shared_ceo_directives.md) -- Estrategia tecnologica
- [Glossario](03_GLOSSARIO.md) -- Termos tecnicos
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md) -- TI como suporte transversal
- **Departamentos relacionados:**
  - [Financeiro](dept_financeiro.md) -- Integracao QuickBooks
  - [Permits](dept_permits.md) -- Automacao county portals
  - [QPS](dept_qps.md) -- Dashboards, Power BI
  - [Scheduling](dept_scheduling.md) -- Dashboard Construction Data
  - [RH](dept_rh.md) -- Gestao de acessos
