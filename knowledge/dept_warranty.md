# Warranty (Garantia) - Lakeshore Development

## Visao Geral
- **Missao:** Gerenciar todas as solicitacoes de garantia pos-entrega, coordenando reparos com subcontratados, acompanhando prazos, gerenciando processo de closing (pre-venda) e controlando cortes de grama em casas abertas e fechadas
- **Lider:** Taylane Silva - Closing + Warranty (presencial, contato com realtors/investidores, office2@lakeshoredevelopmentfl.com)
- **Equipe:**
  - Sophia Felizola (sfelizola@lakeshoredevelopmentfl.com) - Warranty (solicitacoes de reparo, cortes de grama)
  - Kildery Diniz (cpm3@lakeshoredevelopmentfl.com) - Warranty (gerenciamento de dados, planilhas, formado em estatistica)
- **Departamentos relacionados:** Client Relations (CR), Financeiro, Supervisao (Daniel), Monitores/Data Loggers, QPS (Don/Fortine), Scheduling, Subs diversos

## Processos

### Processo 1: Fluxo de Warranty (Garantia Pos-Entrega)
- **Objetivo:** Receber, registrar, encaminhar e acompanhar solicitacoes de reparo de clientes dentro do periodo de garantia ate a conclusao
- **Responsavel principal:** Sophia Felizola
- **Frequencia:** Diaria (fluxo continuo de solicitacoes)
- **Ferramentas:** E-mail (canal 100% formal para warranty), WhatsApp (cobranca a subs), Builder Trend (daily logs), Planilha de acompanhamento de reparos

**Passo a passo:**
1. Cliente envia solicitacao por e-mail (100% formalizado) -- Responsavel: Cliente -- Ferramenta: E-mail
2. Equipe recebe e registra na planilha de acompanhamento (pedido, tipo de reparo, data) -- Responsavel: Sophia / Kildery -- Ferramenta: Planilha Excel
3. Avaliar se esta dentro da garantia (validade = data de ocupacao/venda, NAO mais a partir do CO) -- Responsavel: Sophia -- Ferramenta: Planilha Excel
4. Encaminhar para sub responsavel via WhatsApp -- Responsavel: Sophia -- Ferramenta: WhatsApp (grupos especificos por tipo, ex: Eco One para encanamento)
5. Acompanhar execucao (cobrar a cada 3 dias se sem resposta) -- Responsavel: Sophia -- Ferramenta: WhatsApp
6. Registrar no Builder Trend: **open claim** -> **schedule** -> **finalize** (3 daily logs) -- Responsavel: Sophia -- Ferramenta: Builder Trend
7. Sub confirma conclusao (com foto preferencialmente) -- Responsavel: Sub -- Ferramenta: WhatsApp
8. Supervisor Daniel confirma em visitas de rota -- Responsavel: Daniel -- Ferramenta: Visita presencial

**Inputs:** Solicitacao de reparo do cliente (por e-mail)
**Outputs:** Reparo concluido; 3 daily logs no Builder Trend (open claim, schedule, finalize); registro na planilha
**Observacoes:** E-mail e canal 100% formal para warranty. Clientes frequentemente enviam por WhatsApp tambem, causando trabalho duplicado. Cobranca a subs que nao respondem e frequente.

### Processo 2: Closing (Pre-Venda)
- **Objetivo:** Gerenciar reparos necessarios identificados por private inspector antes da venda da casa, garantindo que esteja em condicoes para entrega
- **Responsavel principal:** Taylane Silva
- **Frequencia:** Por casa (na fase de venda)
- **Ferramentas:** WhatsApp, E-mail, Builder Trend

**Passo a passo:**
1. Private inspector realiza inspecao e lista reparos necessarios -- Responsavel: Inspector (externo) -- Ferramenta: Relatorio de inspecao
2. Taylane recebe lista via WhatsApp/e-mail -- Responsavel: Taylane -- Ferramenta: WhatsApp, E-mail
3. Encaminhar para equipe separar por tipo (eletrico, hidraulico, acabamento) -- Responsavel: Taylane -- Ferramenta: WhatsApp
4. Subs fazem reparos -- Responsavel: Subs -- Ferramenta: [execucao em campo]
5. Casa liberada para venda -- Responsavel: Taylane -- Ferramenta: [processo interno]

**Inputs:** Relatorio de inspecao privada com lista de reparos
**Outputs:** Casa com reparos concluidos, pronta para venda
**Observacoes:** Taylane trabalha presencialmente com realtors e investidores. Closing e mais via WhatsApp que e-mail.

### Processo 3: Gerenciamento de Cortes de Grama
- **Objetivo:** Manter gramados de casas abertas (em construcao) e fechadas (vendidas) cortados, evitando multas do condado e mantendo aparencia adequada
- **Responsavel principal:** Sophia Felizola / Kildery Diniz
- **Frequencia:** Semanal (data loggers passam semanalmente)
- **Ferramentas:** Slack (notificacoes dos data loggers), Planilha complexa de Kildery, Builder Trend, WhatsApp

**Passo a passo:**
1. Data loggers passam nas casas semanalmente e reportam no Slack (input no Builder Trend) -- Responsavel: Data Loggers/Monitores -- Ferramenta: Slack, Builder Trend
2. Verificar status da casa: open = pode solicitar direto; closed = precisa autorizacao -- Responsavel: Sophia / Kildery -- Ferramenta: Planilha de Kildery
3. Para casas closed: solicitar autorizacao via CR (Client Relations) no Slack -- Responsavel: Sophia -- Ferramenta: Slack
4. Excecao: casas de Gabriel e Vittor sao pre-autorizadas -- Responsavel: Sophia -- Ferramenta: [regra interna]
5. Calcular tamanho do gramado (base de dados + VLOOKUP) -- Responsavel: Kildery -- Ferramenta: Planilha Excel
6. Enviar lista para sub com pin point, endereco e tamanho -- Responsavel: Sophia -- Ferramenta: WhatsApp
7. Controlar prazos (maximo 5 dias, forcando 2-3 dias) -- Responsavel: Sophia -- Ferramenta: Planilha Excel
8. Registrar PO e valores (tabela de precos: ate 0.22 acres=$50; ate 0.33=$60; ate 0.50=cotacao; acima=cotacao especifica; teto $30 para cortes padrao) -- Responsavel: Kildery -- Ferramenta: Builder Trend, Planilha Excel
9. Sub envia foto/video de comprovacao -- Responsavel: Sub -- Ferramenta: WhatsApp

**Inputs:** Relatorio de data loggers (via Slack); status de casas (open/closed); autorizacao de CR para casas closed
**Outputs:** Gramados cortados; POs registradas; fotos de comprovacao
**Observacoes:** Risco de notificacao/multa do condado se grama muito alta. Cortes urgentes sao prioridade.

### Processo 4: Tracking de Shower Glass Door
- **Objetivo:** Acompanhar a instalacao de portas de vidro do box (shower glass door), que depende da conclusao de tile e vinyl como pre-requisitos
- **Responsavel principal:** Kildery Diniz
- **Frequencia:** Continua (por casa na fase final)
- **Ferramentas:** Builder Trend (tags), Planilha complexa de Kildery

**Passo a passo:**
1. Acompanhar tags de tile, vinyl, cabinets no Builder Trend -- Responsavel: Kildery -- Ferramenta: Builder Trend, Planilha Excel
2. Quando tile/vinyl finalizados -> casa habilitada para glass door -- Responsavel: Kildery -- Ferramenta: Planilha Excel
3. Acompanhar medicao (sub vai a casa para medir) -- Responsavel: Kildery -- Ferramenta: WhatsApp
4. Acompanhar PO e instalacao -- Responsavel: Kildery -- Ferramenta: Builder Trend
5. Acompanhar Beauty Final (inspecao final estetica) -- Responsavel: Kildery -- Ferramenta: Builder Trend
6. Acompanhar CEO (Certificate of Occupancy) -- Responsavel: Kildery -- Ferramenta: Builder Trend

**Inputs:** Status de tile/vinyl/cabinets (do Scheduling); PO de glass door
**Outputs:** Glass door instalada; casa pronta para Beauty Final e CEO
**Observacoes:** Shower glass door e um gatilho principal rastreado separadamente por ser um dos ultimos itens antes da entrega.

### Processo 5: Gerenciamento de Dados e Tracking (Planilha Complexa)
- **Objetivo:** Manter controle centralizado de todas as informacoes de warranty, closing e dados de casas para acompanhamento gerencial
- **Responsavel principal:** Kildery Diniz
- **Frequencia:** Diaria
- **Ferramentas:** Planilha complexa com multiplas abas, Builder Trend

**Passo a passo:**
1. Atualizar aba CEO tracking (data CEO, data venda/ocupacao) -- Responsavel: Kildery -- Ferramenta: Planilha Excel
2. Atualizar status de reparos com delay tracking (marcar >3 dias) -- Responsavel: Kildery -- Ferramenta: Planilha Excel
3. Atualizar tracking de Shower Glass Door, Tile, Vinyl, Cabinets -- Responsavel: Kildery -- Ferramenta: Planilha Excel
4. Gerenciar dados de cortes de grama (enderecos, tamanhos, autorizacoes, custos) -- Responsavel: Kildery -- Ferramenta: Planilha Excel
5. Manter base de dados de casas (enderecos, cidades, square feet, acres) -- Responsavel: Kildery -- Ferramenta: Planilha Excel
6. Controlar POs -- Responsavel: Kildery -- Ferramenta: Planilha Excel
7. Gerar informacoes para tomada de decisao -- Responsavel: Kildery -- Ferramenta: Planilha Excel

**Inputs:** Dados de todas as fontes (Builder Trend, WhatsApp, E-mail, Slack)
**Outputs:** Planilha centralizada com visao completa de warranty e closing
**Observacoes:** Kildery e formado em estatistica e criou sistema complexo de tracking que centraliza informacoes dispersas em multiplas fontes.

## Regras de Garantia
- **Validade**: A partir da data de ocupacao/venda (NAO mais a partir do CO)
- **Cobertura**: Tudo que nao passaria numa inspecao esta incluso (orientacao juridica)
- **Sub warranty**: Sub conta 1 ano a partir do fim do servico (conflito com regra da empresa)
- **CO ainda rastreado**: Para visualizacao de quanto tempo a casa demorou para ser vendida

## Dores e Problemas Conhecidos
- **3 daily logs por reparo**: Abertura, schedule, finalizacao -- muito input no sistema
- **Volume alto e dinamismo**: Dificil manter registro no Builder Trend em tempo real
- **Imediatismo dos clientes**: Ligam e mandam WhatsApp mesmo quando pedem para formalizar por e-mail
- **Trabalho duplicado**: Cliente manda e-mail E WhatsApp, equipe responde nos dois
- **Subs nao respondem**: Cobrar repetidamente via WhatsApp, as vezes ficam no vacuo
- **Subs de garantia tem prazo proprio**: Sub conta 1 ano a partir de quando TERMINOU servico, nao do CEO
- **Valores de reparo imprevisiveis**: Morador nao relata extensao total do problema, sub descobre no local
- **Falta de registro no Builder Trend**: Inputs retroativos nao sao detectados no acompanhamento diario
- **Builder Trend lento**: Internet ruim causa delay no carregamento
- **Cortes de grama urgentes**: Risco de notificacao/multa do condado
- **Sem valores fixos para reparos**: Depende de avaliacao no local
- **Monitores nao acompanham casas em fase 4**: Kildery tem que verificar com supervisor Daniel
- **Nao existe software dedicado para warranty**: Prejuizos significativos (caso de $14.000 em uma unica casa)

## Dependencias
- **Recebe de:** Client Relations (CR) -> autorizacao para corte de grama em casas fechadas; Financeiro -> pagamento de honorarios quando garantia do sub expira; Supervisores (Daniel) -> verificacao in loco em casas de warranty; Data Loggers/Monitores -> reportam necessidade de corte de grama; QPS (Don/Fortine) -> padroes de qualidade
- **Entrega para:** Subs -> encaminhamento de solicitacoes de reparo; Financeiro -> POs de reparos e cortes de grama; Client Relations -> status de reparos para comunicacao com cliente; Taylane -> casas prontas para venda apos reparos de closing

---

## Descricao de Cargo Formal (Fonte: Drive Lakeshore)

### Coordenador de Closing & Warranty

- **Setor:** Closing & Warranty
- **Descricao geral:** Atendimento no pre-venda do corretor, reparos, garantia, ajuste de documentos e atendimento na entrega da casa
- **Principais responsabilidades:**
  - Agendamento de walkthrough entre supervisor e corretor e/ou comprador
  - Responsavel pelas chaves das casas
  - Responsavel por solicitar reparos com os subcontractors
  - Realizar o preenchimento do documento de garantia de 1 ano da construtora
  - Acompanhamento das documentacoes: HUDs (HUD 99A, HUD 99B, HUD 92541, HUD 92544), WARRANTY 2-10, Loan, Notice of Termination/Affidavit
  - Emitir Purchase Orders
  - Atualizar o sistema (Daily Logs, POs)
  - Apos a assinatura do Notice of Termination/Affidavit, comunicar ao financeiro para realizar o fechamento da casa

---

## Checklist de Entrega (Fonte: Drive Lakeshore)

Itens do Final Walkthrough Checklist com relevancia direta para o departamento de Warranty. Problemas identificados APOS a assinatura deste checklist devem ser submetidos pelo processo formal de garantia. Os itens abaixo representam os pontos de maior incidencia de solicitacoes pos-entrega.

---

### Itens de Alto Risco para Warranty por Categoria

**Geral**
- Vinyl e tiles instalados corretamente — defeitos de instalacao sao cobertos pela garantia de 1 ano
- Armarios sem rachaduras ou arranhoes — item cosmético; avaliado caso a caso
- Drywall fechado — infiltracoes ou falhas estruturais posteriores entram como claim
- Appliances instalados e funcionando — mau funcionamento pos-entrega pode ser claim ou responsabilidade do fabricante
- Garbage disposal funcionando — item mecanico, alta frequencia de claims

**Eletrico**
- Todas as luzes funcionando — falhas eletricas pos-entrega sao claims frequentes
- Tomadas funcionando corretamente — verificacao critica; falhas podem indicar problema de fiacao
- Detectores de fumaca e monoxido de carbono instalados e funcionando — item de seguranca; obrigatorio

**Ar-Condicionado**
- AC limpo e com filtro novo na entrega — estado inicial documentado para referencia em claims futuros
- AC funcionando corretamente — sistema HVAC e um dos maiores geradores de claims pos-entrega

**Hidraulico / Plumbing**
- Agua quente funcionando — falhas no aquecedor geram claims frequentes
- Torneiras bem instaladas e funcionando — vazamentos pos-entrega sao claims cobertos
- Descarga funcionando corretamente
- Ralos sem entupimento — entupimentos pre-existentes sao responsabilidade do builder
- Sem vazamentos em tubulacoes ou conexoes — vazamentos ocultos descobertos apos entrega geram claims de alta severidade

**Portas e Janelas**
- Fechadura eletronica funcionando (porta da frente) — falha mecanica/eletronica coberta pela garantia
- Porta de correr de vidro: fechadura instalada, chaves disponiveis, tela instalada — itens frequentemente reclamados
- Borracha de vedacao da porta da frente instalada — vedacao deficiente causa infiltracao de agua
- Porta de vidro do box devidamente instalada — instalacao inadequada gera claims de seguranca

---

### Regras de Transicao Pos-Checklist

Conforme o documento oficial de entrega assinado pelo cliente:

- **Reparos nao cobertos**: itens puramente cosmeticos ou fora dos padroes de qualidade estabelecidos pela empresa nao serao executados; cliente recebe notificacao escrita identificando os itens excluidos
- **Canal formal de warranty**: qualquer problema identificado APOS a conclusao da vistoria deve ser submetido pelo processo formal de solicitacao de garantia (via e-mail)
- **Chaves**: entregues exclusivamente no escritorio de Orlando, apos quitacao da Final Invoice ou conclusao do fechamento financeiro
- **Utilities**: prazo de 10 dias uteis para o proprietario transferir as contas de utilities para seu nome — apos esse prazo, servicos sob conta da Lakeshore serao encerrados

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- [Catalogo de Dores](07_CATALOGO_DORES.md)
- [Fluxo Spec Home](05_FLUXO_SPEC_HOME.md)
- [Fluxo Custom Home](06_FLUXO_CUSTOM_HOME.md)
- [Glossario de Termos](03_GLOSSARIO.md)
- **Departamentos relacionados:**
  - [Client Relations](dept_client_relations.md) — autoriza corte de grama; recebe status de reparos
  - [Financeiro](dept_financeiro.md) — paga honorarios quando garantia do sub expira; recebe POs de reparos
  - [Supervisao](dept_supervisao.md) — Daniel faz verificacao in loco em casas de warranty
  - [Inspecao](dept_inspecao.md) — inspecoes finais aprovadas habilitam fechamento de casa

---

## Supervisao Quality Integration

### How Supervisao Findings Feed Warranty Risk Assessment
- Supervisao performs quality pre-inspections during construction
- Quality findings documented in daily logs become warranty risk indicators
- Common risk patterns identified during construction that predict future warranty claims:

| Construction Finding | Warranty Risk | Predictive Action |
|---------------------|---------------|-------------------|
| Plumbing rough-in issues | High claim probability (leaks) | Flag house for 6-month warranty check |
| HVAC installation deviation | System failure risk | Flag for first-summer performance check |
| Drywall finish defects | Cosmetic claims likely | Document pre-delivery condition |
| Exterior stucco cracks | Water intrusion risk | Flag for rainy season follow-up |
| Tile/vinyl installation gaps | Immediate claim likely | Ensure repair before closing walkthrough |

### Integration Points
- **Daniel (Supervisor)** verifies warranty repairs in field during regular route visits
- Supervisao quality scores by subcontractor feed into warranty sub-selection:
  - High-quality subs -> preferred for warranty repair assignments
  - Low-quality subs -> flagged, avoid for warranty work
- QPS route data (Don/Fortine visiting ~60 houses/day) identifies emerging warranty patterns

## Coverage Thresholds

### Warranty Duration by Category
| Category | Coverage Period | Start Date | What's Covered | What's NOT Covered |
|----------|----------------|------------|----------------|---------------------|
| Structural | 10 years | Date of occupancy/sale | Foundation cracks, framing failure, roof structure | Normal settling, cosmetic cracks |
| Mechanical (HVAC) | 2 years | Date of occupancy/sale | System failures, compressor, ductwork | Filter changes, thermostat batteries |
| Mechanical (Plumbing) | 2 years | Date of occupancy/sale | Pipe leaks, fixture failures, water heater | Drain clogs from misuse, external damage |
| Mechanical (Electrical) | 2 years | Date of occupancy/sale | Wiring faults, panel issues, outlet failures | Bulb replacement, surge damage |
| Cosmetic (Paint, Drywall) | 1 year | Date of occupancy/sale | Installation defects, peeling, cracking | Normal wear, nail pops from settling |
| Cosmetic (Flooring) | 1 year | Date of occupancy/sale | Installation defects, loose tiles, gaps | Scratches, stains, normal wear |
| Appliances | Per manufacturer | Date of installation | Per manufacturer terms | See manufacturer warranty card |
| Roofing (Materials) | Per manufacturer | Date of installation | Shingle defects, material failure | Storm damage (insurance) |
| Roofing (Workmanship) | 2 years | Date of occupancy/sale | Leaks from installation errors | Storm damage, falling debris |

### Key Coverage Rules
- **Start date**: Warranty begins at date of occupancy/sale (NOT from CO date)
- **CO tracking**: CO date still tracked for analytics (time house took to sell)
- **Legal guidance**: "Everything that would not pass an inspection is covered" (orientation from legal)
- **Sub warranty conflict**: Subcontractors count 1 year from THEIR completion date, not from sale -- this creates a gap period where Lakeshore covers but sub may not

### Coverage Decision Tree
```
Warranty claim received
  |
  +-> Determine claim category (structural, mechanical, cosmetic, appliance)
  |
  +-> Calculate time since occupancy/sale date
  |
  +-> Within coverage period?
  |     |
  |     +-> YES -> Process claim (see Claim Resolution Process)
  |     +-> NO -> Deny with explanation
  |           - Provide coverage period info
  |           - IF appliance -> direct to manufacturer
  |           - IF structural and close to 10yr -> review carefully (high-value)
  |
  +-> Borderline cases (within 30 days of expiration):
        - Review on case-by-case basis
        - IF safety concern -> approve regardless
        - IF goodwill opportunity -> escalate to Taylane for decision
```

## Claim Resolution Process

### End-to-End Warranty Claim Flow
```
1. RECEIVE: Client sends claim via email (formal channel)
   - Log in tracking spreadsheet: date, client, house, issue type
   - Acknowledge receipt within 24 hours

2. VALIDATE: Check warranty coverage
   - Occupancy/sale date vs. current date
   - Claim category vs. coverage threshold
   - IF not covered -> notify client with explanation
   - IF covered -> proceed

3. IDENTIFY: Find responsible subcontractor
   - Search daily logs for house + work type
   - Find original sub, completion date, PO reference
   - Check if sub's own guarantee is still active

4. ROUTE: Send to subcontractor
   - Contact sub via WhatsApp with claim details + original PO
   - Set 3-day initial response deadline
   - IF no response -> follow up at day 3
   - IF still no response at day 7 -> escalate to Supervisao

5. SCHEDULE: Coordinate repair timing
   - Sub proposes repair date
   - Register in Builder Trend: "schedule" daily log
   - Notify client of repair date

6. EXECUTE: Sub performs repair
   - Sub visits house and completes repair
   - Sub sends photo/video confirmation via WhatsApp
   - Supervisor Daniel verifies during route visits (when feasible)

7. VERIFY: Confirm completion
   - Register in Builder Trend: "finalize" daily log
   - Contact client to confirm satisfaction
   - IF client not satisfied -> repeat from step 4 with same or different sub

8. CLOSE: Mark claim resolved
   - Update tracking spreadsheet with resolution date
   - Calculate resolution time (target: <14 days)
   - Archive documentation
```

### SLA Tracking
| Milestone | Target SLA | Escalation |
|-----------|-----------|------------|
| Client acknowledgment | 24 hours | Auto-escalate to Taylane |
| Sub contacted | 48 hours | Follow-up via WhatsApp |
| Sub initial response | 3 days | Second follow-up |
| Repair scheduled | 7 days | Escalate to Supervisao |
| Repair completed | 14 days | Escalate to Coordenador |
| Client confirmation | 3 days after repair | Phone call to client |

### Financial Routing
- **Sub guarantee active**: Sub performs repair at own cost
- **Sub guarantee expired, Lakeshore warranty active**: Generate new PO -> route to Financeiro for payment authorization
- **Both expired**: Deny claim, refer homeowner to sub directly for private arrangement

---

## BuilderTrend Job 455 -- Real Data

### Warranty Context from Job 455
- **Job Status**: Closed (Sep 24, 2025)
- **Owner Walkthrough (FCC4)**: Sep 9, 2025
- **CO Issued**: Sep 2025
- **Warranty start date**: Based on date of occupancy/sale (NOT CO date)
- **0 Change Orders**: No scope disputes during construction

### Subcontractors Available for Warranty Repairs (from Job 455)
| Trade | Sub | Contact Pattern |
|-------|-----|----------------|
| Plumbing | Eco One Plumbing Services, Inc | WhatsApp group (direct) |
| Electrical | Electrical sub | WhatsApp group |
| AC/HVAC | AC sub | WhatsApp group |
| Roofing | Roofing sub | WhatsApp group |
| Garage Door | Strong Quality Garage Door | Direct contact |
| Cabinets/Countertop | ONYX GRANITE | Direct contact |
| Tile/Vinyl | IVISION GROUP LLC | Direct contact |
| Stucco/Lath | J.A.S.H. Services | Direct contact |
| Handyman/Touch-up | CoreCraft Services LLC | Slack @group-handyman |
| Painting | JC Anchor Painting Corp | Direct contact |
| Insulation | ETERNAL INSULATION LLC | Direct contact |
| Driveway | Red Twelve LLC | Direct contact |

### Warranty Claims Lifecycle (BuilderTrend)
1. Client emails warranty request
2. Register in BT: Daily Log with "open claim" tag
3. Route to original sub via WhatsApp
4. Daily Log update: "schedule" tag when sub schedules repair
5. Sub completes repair (photo confirmation)
6. Supervisor Daniel confirms during route visit
7. Daily Log update: "finalize" tag
8. Warranty claim closed

### Common Warranty Issues (from Job 455 trades)
Based on the trades and materials used on Job 455, common warranty claims include:
- Plumbing leaks (Eco One -- $3,350 original work)
- AC issues (thermostat, ductwork -- $7,300 original)
- Electrical faults (outlets, fixtures -- $6,470 original)
- Stucco cracks (J.A.S.H. -- $3,450 original)
- Tile/vinyl defects (IVISION -- $4,204 original)
- Cabinet/countertop issues (ONYX -- $6,978 original)
- Garage door adjustment (Strong Quality -- $1,850 original)
- Door hardware (MLI Home Improvements -- $575 original)

## CPM Construction Sequence -- Warranty Touchpoints

### Quality Control Gates That Prevent Warranty Claims
The CPM includes quality control points designed to catch issues before handover:
| QC Point | Timing | Purpose |
|----------|--------|---------|
| Quality Control 1 | With Final Touches (FIRST day) | Catch defects early |
| Quality Control 2 | With Final Touches (LAST day) | Final sweep before walkthrough |
| FCC (Final Construction Check) | After Building Final Inspection | Comprehensive quality audit |
| Internal Walkthrough | Before client walkthrough | Company leadership review |
| Client Walkthrough | Formal handover | Client identifies any remaining issues |
| Drywall Repair Verification | After drywall repairs | Verify drywall patches are invisible |
| Sod Health Verification | After sod installation | Verify sod is healthy and established |

### Post-Handover Activities (from CPM FASE 4)
- Hose Install/Removal -- irrigation seeding must be maintained for sod health
- Portable Removal -- scheduled after close-out
- Lawn maintenance transitions to CoreCraft (warranty lawn cuts)

## Const App Integration

### Relevant Const App Modules for Warranty
- **Rework Module**: Manage rework requests from inspections (same workflow applies to warranty claims)
  - Rework Queue: Assign to handymen, dispatch, or postpone
  - Handymen Kanban Board: Track rework progress (John Smith, Maria Garcia, Lisa Chen, Robert Johnson)
  - Completed History: Permanent record of completed reworks with duration
- **Verification Module**: Verify that warranty repairs were completed properly
  - Site Visits: Schedule verification visits for warranty repairs
  - Photo Review: Review photos of completed warranty work

### Service Codes for Common Warranty Work
| Code | Service | Common Warranty Issue |
|------|---------|---------------------|
| CON-002 | Warranty Fee | Warranty fee charged to contract |
| PLM-005 | Plumbing Trim | Fixture leaks, adjustments |
| ELC-005 | Electrical Trim | Outlet/fixture issues |
| MEC-003 | Mechanical Trim | AC/HVAC adjustments |
| FIN-001 | Stucco | Crack repairs |
| FIN-006 | Painting | Touch-up painting |
| EXT-014 | Handyman Touch Up | General repairs |
| VAR-001 | Variances | Miscellaneous warranty items |

## Available Tools

| Tool | Parameters | Returns |
|------|-----------|---------|
| read_daily_logs | date (str, optional), house_id (str, optional) | Daily log entries |
| read_daily_log_detail | log_id (str) | Full daily log record |
| search_daily_logs | query (str) | Matching daily log entries |

> **Note:** Warranty has read-only access to daily logs for checking project history, original sub identification, and repair tracking.

## CEO Directives (Bernardo)
- Warranty is the last touchpoint with the client -- every repair reflects on the Lakeshore brand.
- Cost-plus transparency extends to warranty: track every repair cost per house for closing reconciliation.
- Scale to 500 homes means warranty volume will grow exponentially -- structured tracking is mandatory.
- Sub accountability: subs who generate excessive warranty claims should be flagged for performance review.

## Handoff Triggers

### Outbound (Warranty sends TO other agents)

| When | Hand off to | Send | SLA |
|------|-------------|------|-----|
| Repair POs and lawn cut POs created | financeiro | $: PO reference, repair description, sub name, amount | 24h |
| Repair status update for client communication | client_relations | INFO: repair status, timeline, house_id | 24h |
| Houses ready for sale after closing repairs | coordenador | APROV: house cleared for sale, closing complete | 24h |

### Inbound (Warranty expects FROM other agents)

| When | Hand off to | Send | SLA |
|------|-------------|------|-----|
| Lawn cut authorization for closed houses | client_relations | APROV: authorization for lawn maintenance | immediate |
| Payment when sub guarantee expires | financeiro | $: sub guarantee expiration, payment needed | 24h |
| Field verification in warranty houses | supervisao | INFO: field verification result, issues found | 24h |
| Lawn cut need reported by monitors | qps | INFO: house_id, lawn condition, urgency | 24h |
| Quality standards for warranty verification | qps | DOC: quality checklist, standards reference | 48h |
| CO issued -- house can be delivered | inspecao | INFO: CO issued, house_id -- H-13 triggers closing process | immediate |

## Key Glossary Terms

- **Warranty** / **Garantia**: Post-delivery repair coverage -- structural (10yr), mechanical (2yr), cosmetic (1yr)
- **Closing** / **Fechamento**: Pre-sale repair and handover process -- managed by Taylane
- **CO (Certificate of Occupancy)** / **Habite-se**: County certificate enabling occupancy -- tracked for analytics
- **FCC (Face for Checklist Done)** / **Verificacao Final**: QPS quality gate before delivery
- **Client Hold** / **Retencao do Cliente**: Cost approval needed from client for extras
- **Lawn Cut** / **Corte de Grama**: Lawn maintenance for open and closed houses -- tiered pricing
- **Sub Guarantee** / **Garantia do Sub**: Sub's own warranty period (1 year from their completion, NOT from sale)
- **Release** / **Liberacao**: Notarized document confirming sub was paid -- required before payment
- **Punch List** / **Lista de Pendencias**: Items needing correction before delivery
