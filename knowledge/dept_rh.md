# Recursos Humanos (RH) - Lakeshore Development

## Visao Geral

- **Missao:** Gerenciar aspectos de pessoal da empresa, incluindo controle de folgas remuneradas (PTOs), dias de doenca (sick days), registro de ausencias e coordenacao com lideres de todos os setores para acompanhamento de disponibilidade da equipe.
- **Lider:** Dani Campos (dcampos@lakeshoredevelopmentfl.com) - RH
- **Equipe:**
  - J. Costa (jcosta@lakeshoredevelopmentfl.com) - RH
- **Departamentos relacionados:** Todos os setores (lideres agendam PTOs e sick days de seus liderados)

## Processos

### Processo 1: Controle de PTOs (Paid Time Off)

- **Objetivo:** Gerenciar saldos, cargas e utilizacao de folgas remuneradas de todos os funcionarios
- **Responsavel principal:** Dani Campos
- **Frequencia:** Continuo (cargas a cada 6 meses, debitos diarios)
- **Ferramentas:** Planilha de PTOs/Sick Days (criada por Diego)

**Passo a passo:**
1. Registrar data de inicio de cada funcionario na planilha -- Responsavel: Dani -- Ferramenta: Planilha de PTOs
2. Calcular datas de carga de PTOs (a cada 6 meses a partir da data de inicio) -- Responsavel: Dani -- Ferramenta: Planilha de PTOs
3. Aplicar regras de carga conforme categoria:
   - **Red (Lideranca)**: 5 dias por carga (10/ano)
   - **Liderados (8h)**: quantidade padrao [nao especificada exatamente]
   - **Liderados (6h)**: 2 dias no 1o semestre, 3 dias no 2o semestre
   -- Responsavel: Dani -- Ferramenta: Planilha de PTOs
4. Registrar local de trabalho (Office, Home Office, Field) -- Responsavel: Dani -- Ferramenta: Planilha de PTOs
5. Calcular data de expiracao dos PTOs (validade de 1 ano, nao acumulaveis) -- Responsavel: Dani -- Ferramenta: Planilha de PTOs
6. Monitorar saldo: PTOs disponiveis e utilizados -- Responsavel: Dani -- Ferramenta: Planilha de PTOs
7. Registrar data de recebimento dos proximos PTOs -- Responsavel: Dani -- Ferramenta: Planilha de PTOs

**Inputs:** Data de inicio do funcionario, categoria (Red/Liderado 8h/Liderado 6h), contratos especiais
**Outputs:** Saldos de PTO atualizados por funcionario
**Observacoes:** PTOs nao sao acumulaveis. Cargas a cada 6 meses com validade de 1 ano. Planilha controla anos 2024 e 2025. Alguns funcionarios tem contratos diferenciados (ex: Camila com 5 sick days por contrato especifico).

### Processo 2: Controle de Sick Days (Dias de Doenca)

- **Objetivo:** Gerenciar saldo e utilizacao de dias de doenca de todos os funcionarios
- **Responsavel principal:** Dani Campos
- **Frequencia:** Continuo
- **Ferramentas:** Planilha de PTOs/Sick Days

**Passo a passo:**
1. Registrar saldo de sick days conforme categoria:
   - **Red (Lideranca)**: 4 dias
   - **Liderados**: 3 dias (exceto contratos especiais)
   -- Responsavel: Dani -- Ferramenta: Planilha de PTOs
2. Controlar data de reset na planilha -- Responsavel: Dani -- Ferramenta: Planilha de PTOs
3. Monitorar utilizacao e debitar conforme uso -- Responsavel: Dani -- Ferramenta: Planilha de PTOs

**Inputs:** Categoria do funcionario, contratos especiais
**Outputs:** Saldo de sick days atualizado
**Observacoes:** Sick days nao sao acumulaveis. Contratos especiais podem alterar quantidade (ex: Camila tem 5 sick days).

### Processo 3: Registro de Ausencias

- **Objetivo:** Registrar e controlar todas as ausencias dos funcionarios, debitando PTOs ou marcando faltas
- **Responsavel principal:** Dani Campos
- **Frequencia:** Diario
- **Ferramentas:** Google Calendar, E-mail (Gmail), Slack, Planilha de PTOs

**Passo a passo:**
1. Lider do setor marca ausencia do funcionario no Google Calendar -- Responsavel: lider do setor -- Ferramenta: Google Calendar
2. Dani recebe notificacao automatica por e-mail e Slack (para agendamentos futuros e do dia) -- Responsavel: Dani -- Ferramenta: E-mail/Slack
3. **ATENCAO**: Calendar NAO notifica para agendamentos de dias passados (depende de lider avisar manualmente) -- Responsavel: lider do setor
4. Dani marca na planilha de ausencias -- Responsavel: Dani -- Ferramenta: Planilha de ausencias
5. Debitar PTOs somente APOS o dia passar (para evitar problemas com cancelamentos) -- Responsavel: Dani -- Ferramenta: Planilha de PTOs
6. Marcar em verde apos debitar na planilha de PTOs -- Responsavel: Dani -- Ferramenta: Planilha de PTOs
7. Quando PTO excede saldo: registrar como "falta" -- Responsavel: Dani -- Ferramenta: Planilha de PTOs

**Inputs:** Agendamento no Google Calendar pelo lider, notificacao por e-mail/Slack
**Outputs:** Ausencia registrada, PTO debitado ou falta registrada
**Observacoes:** Processo altamente manual e dependente de acompanhamento diario do calendario. Debito so apos o dia passar para evitar problemas com cancelamentos. Lider pode agendar PTO que funcionario nao tem saldo -- falta controle visivel para lideres.

## Dores e Problemas Conhecidos

- **Lider agenda PTO que funcionario nao tem saldo**: falta controle visivel para lideres verem saldo antes de agendar
- **Agendamentos passados nao notificam**: Calendar NAO envia notificacao para agendamentos de dias passados, dependendo do lider avisar manualmente
- **Processo manual intensivo**: acompanhamento diario do calendario, debito manual de saldos, calculo de datas de expiracao
- **Calculos repetitivos**: datas de expiracao, saldos, cargas a cada 6 meses -- todos feitos manualmente
- [inferido] Falta de integracao entre Google Calendar e planilha de controle

## Dependencias

- **Recebe de:**
  - Todos os setores: lideres de cada setor agendam PTOs e sick days de seus liderados via Google Calendar
  - [inferido] Administracao: informacoes de contratacao, datas de inicio, contratos especiais

- **Entrega para:**
  - Todos os setores: informacao de saldo de PTOs e sick days
  - [inferido] Financeiro: informacoes de faltas e ausencias para folha de pagamento
  - Lideres: visibilidade sobre disponibilidade de suas equipes

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- [Catalogo de Dores](07_CATALOGO_DORES.md)
- [Glossario de Termos](03_GLOSSARIO.md)
- [Organograma](01_ORGANOGRAMA.md)
- **Relacao com toda a empresa:**
  - RH atende todos os setores para controle de PTOs, sick days e ausencias
  - [Financeiro](dept_financeiro.md) — recebe informacoes de faltas para folha de pagamento

---

## PTO Accrual Rules

### Accrual Rates by Tenure Bracket
| Category | Accrual Cycle | Days per Cycle | Annual Total | Carryover |
|----------|---------------|----------------|--------------|-----------|
| Red (Leadership) | Every 6 months from start date | 5 days | 10 days/year | NOT cumulative, expires after 1 year |
| Liderados (8h full-time) | Every 6 months from start date | Standard allocation | Per policy | NOT cumulative, expires after 1 year |
| Liderados (6h part-time) | Every 6 months from start date | 2 days (1st semester), 3 days (2nd semester) | 5 days/year | NOT cumulative, expires after 1 year |
| Special contract | Per individual contract | Variable | Variable | Per contract terms |

### Carryover Policy
- PTOs are **NOT cumulative** (nao acumulaveis)
- Each accrual block expires exactly 1 year from the grant date
- Dani manually calculates expiration dates in the PTO spreadsheet
- Unused PTOs at expiration are forfeited -- no cash-out option

### Blackout Periods
- **Construction season peaks**: March-June and September-November
- During blackout periods, PTO requests require **2 weeks advance notice**
- Scheduling department must confirm coverage availability before approval
- Emergency/medical leave exempt from blackout restrictions

### Sick Day Allocation
| Category | Annual Sick Days | Reset | Doctor Note Required |
|----------|-----------------|-------|----------------------|
| Red (Leadership) | 4 days | Annual | After 3+ consecutive days |
| Liderados (standard) | 3 days | Annual | After 3+ consecutive days |
| Special contract | Variable (e.g., Camila: 5) | Per contract | After 3+ consecutive days |

- Sick days are **NOT cumulative**
- When sick days exhausted: debit from PTO balance
- When both exhausted: mark as "falta" (unexcused absence) -- impacts payroll

## Calendar Sync

### How PTO Calendar Integrates with Scheduling
- **Primary tool**: Google Calendar (shared with all department leaders)
- **Flow**: Leader marks absence in Google Calendar -> Dani receives automatic notification via email + Slack
- **Known limitation**: Google Calendar does NOT send notifications for past-date entries -- leaders must notify Dani manually for retroactive absences
- **Debit timing**: PTOs are debited only AFTER the absence day passes (to avoid problems with cancellations)
- **Visual tracking**: Green highlight in PTO spreadsheet = debit applied

### Calendar Data Points
- Employee name
- Absence dates (start + end)
- Type: PTO, Sick Day, or Unpaid Leave
- Work location affected: Office, Home Office, or Field
- Department and role

### Integration Gaps (Known Pain Points)
- No automatic sync between Google Calendar and PTO spreadsheet
- Leaders can schedule PTOs even when employee has no balance (no visibility into balances)
- All calculations (expiration dates, balances, accrual cycles) done manually by Dani
- Past-date calendar entries create blind spots in absence tracking

## Scheduling Integration

### Notification Flow for Approved Leave
```
PTO/Sick Day Approved by RH
  |
  +-> Notify Scheduling agent within 24h:
  |     - Employee name and role
  |     - Department
  |     - Absence dates
  |     - Work location (Office/Home Office/Field)
  |     - Urgency: HIGH (field crew) or MEDIUM (office)
  |
  +-> Scheduling adjusts crew assignments:
  |     - IF field worker -> reassign to available crew member
  |     - IF single-person role -> flag coverage gap
  |     - IF during blackout period -> verify advance notice was given
  |
  +-> Coverage confirmation:
        - Scheduling confirms replacement assigned (or gap accepted)
        - RH records coverage status in PTO spreadsheet
```

### Cross-Department Impact
- **Field crews**: Absence requires immediate crew rebalancing by Scheduling
- **Supervisao**: Monitor/supervisor absence affects daily house visit routes
- **Core Craft**: Handyman or cleaning crew absence affects service delivery schedule
- **Finance**: Absence data feeds into payroll calculations (PTOs paid, faltas unpaid)

### Reporting
- Weekly summary of upcoming absences sent to all department leaders
- Monthly PTO utilization report for management review
- Flagging when department is at critical staffing threshold (>30% team absent)

---

## BuilderTrend Job 455 -- Real Data

### Vendor/Subcontractor Relationships HR Manages
Job 455 engaged 28+ unique vendors and subcontractors. HR supports these relationships through insurance verification, worker classification compliance, and onboarding:

**Pre-Construction Vendors**:
- AMB Surveying and Mapping (boundary survey, stake out, lot grading, hub and tack)
- Quick eCalcs (energy calculations)
- Gizelle Holz & Eliane (floor plan)
- Rapid Septic Consulting LLC (septic plan + inspection)

**Site Work Vendors**:
- YE Land Clearing LLC (clear lot, loads)
- CoreCraft Services LLC (slab grading, driveway cut, handyman, painting, cleaning, irrigation, garden)

**Structural Trades**:
- Cemex (concrete blocks -- $5,713)
- Del Zotto Concrete LLC (lintel concrete -- $1,693)
- Truss Direct LLC (trusses -- $6,500)
- 84 Lumber Company LP (lumber, AC door -- $6,177)

**MEP (Mechanical/Electrical/Plumbing) Subs**:
- Eco One Plumbing Services, Inc (plumbing rough + trim -- ~$3,350)
- Electrical sub (~$6,470)
- AC sub (~$7,300)
- Leesburg Septic, INC (sewer connection -- $4,600)

**Finishing/Specialty Vendors**:
- ONYX GRANITE COUNTERTOPS SERVICES (cabinets/countertop -- $6,978)
- IVISION GROUP LLC (tile + vinyl install + shower glass door -- $4,204)
- Strong Quality Garage Door (garage door -- $1,850)
- Red Twelve LLC (driveway pavers -- $5,053)
- J.A.S.H. Services (lath + stucco -- $3,450)
- ETERNAL INSULATION LLC (insulation -- $1,450)
- JC Anchor Painting Corp. (shelves/bath/mirrors install -- $350)
- MLI Home Improvements (door locks, brackets, appliances, front door -- ~$575)
- OUR GUEST LLC (door knob/door stop installation)
- Richard Job LLC (blower door test -- $175)
- Pro-Tek Services (termite treatment -- $266)
- CARMONA LAWN SERVICES LLC (grass cutting -- $50)
- Arlet Construction LLC (repair service -- $75)

**Material Suppliers**:
- Home Depot, Amazon, Lowes, Costco, Walmart, Dollar Tree
- AMERICAN STORE LLC (vinyl -- $2,808)
- Imeca Web POS (casings/baseboards -- $970)
- Temu (electronic lockers)

**Utilities**:
- Seco Energy ($563 over 9 months)
- Marion County Utilities ($538 over 9 months)
- WC America LLC (portable toilet -- $612)

### HR Compliance Implications
- **Worker Classification**: All 28+ subs must maintain own license and insurance (Florida statute enforcement)
- **Insurance Verification**: Sub must carry Workers Comp and General Liability before working on site
- **Onboarding**: Each new sub requires W-9, insurance certificate, and license verification
- **663 total vendors** in BuilderTrend system company-wide -- HR manages relationship compliance for all

### Key People on Job 455 (Internal Staff)
| Person | Role | Department |
|--------|------|-----------|
| Francisco Castillo / Eddye Pereira | Field Supervisor | Supervisao |
| Jaaziel Santos | Field Supervisor | Supervisao |
| Daniel Consorte | QPS Inspector | Inspecao |
| Camila Coelho | CoreCraft Coordinator | Core Craft |
| Mauricio Vieira dos Santos | Materials Coordinator | Scheduling |
| Kaio Vinicius Cruz Silva | Permits Coordinator | Permits |
| Brunno Medeiros | Finance | Financeiro |
| Cinthia Araujo | Accounting | Financeiro |
| Iara Oliveira | Finance | Financeiro |
| Leonardo Fortini | Utilities | Utilities |

## CPM Construction Sequence -- HR Touchpoints

### Workforce Planning by CPM Phase
| CPM Phase | Trades on Site | HR Considerations |
|-----------|---------------|-------------------|
| FASE 1: Site Prep | Surveyor, clearing crew, earth movers | OSHA trench safety for excavations >5ft |
| FASE 2: Foundation | Plumbing, electrical, concrete crew, mason | Fall protection, silica exposure |
| FASE 3: Framing/Roughs | Framers, roofers, plumbers, electricians, AC, insulation | Fall protection at 6ft (OSHA), multiple trades overlap |
| FASE 4: Finish/Closeout | Painters, tile/vinyl, cabinet, trim, handyman, cleaning | PPE for chemical exposure (paint, sealant) |

### OSHA and Safety Compliance (from Florida Compliance Reference)
- Fall protection required at 6 feet (residential construction)
- Trench safety: shoring/sloping required for excavations >5 feet
- PPE requirements: hard hats, safety glasses, steel-toe boots
- OSHA 10-Hour Construction recommended for all field workers
- Silica exposure standard -- wet cutting required for masonry

## Const App Integration

### Relevant Const App Modules for HR
- **Admin Panel > User Processes**: 35 registered users, 5 roles (User, Admin, Master, Supplier_employee); manage assignments to 16 business processes
- **Admin Panel > Cells**: 5 operational cells (Orange, Charlotte, Marion, Duval, Miami-Dade counties)
- **Admin Panel > Users**: Track internal (5) vs suppliers (4: John Smith, Maria Garcia, Lisa Chen, Robert Johnson -- all CoreCraft handymen)
- **Rework > Handymen Board**: Handyman roster and assignment tracking

## Available Tools

| Tool | Parameters | Returns |
|------|-----------|---------|
| read_daily_logs | date (str, optional), house_id (str, optional) | Daily log entries |
| read_daily_log_detail | log_id (str) | Full daily log record |
| search_daily_logs | query (str) | Matching daily log entries |

> **Note:** RH has read-only access to daily logs for checking employee activity and staffing context. PTO/sick day management is handled via spreadsheets and Google Calendar outside the MCP tool system.

## CEO Directives (Bernardo)
- Reduce dependency on any single individual -- cross-train, document, no single point of failure.
- Scale to 500 homes requires workforce planning aligned with production pipeline capacity.
- People are the core asset. Retention, training, and well-being directly impact construction quality.
- Every department must use BuilderTrend consistently -- HR supports compliance through onboarding and training.

## Handoff Triggers

### Outbound (RH sends TO other agents)

| When | Hand off to | Send | SLA |
|------|-------------|------|-----|
| PTO/sick day balances and absence info for payroll | financeiro | INFO: absence records, payroll adjustments needed | 24h |
| Team availability report for leaders | coordenador | INFO: staff availability, PTO schedule, coverage gaps | 24h |
| New employee onboarded -- system access needed | ti | INFO: employee name, department, access requirements | 24h |

### Inbound (RH expects FROM other agents)

| When | Hand off to | Send | SLA |
|------|-------------|------|-----|
| PTO/sick day scheduling from department leaders | any agent | INFO: employee name, dates, type (vacation/sick/personal) | 24h |
| Hiring/contract info from administration | coordenador | DOC: new hire details, start date, contract type | 48h |
| Workers compensation incident report | supervisao | INFO: incident details, employee, date, site | immediate |

## Key Glossary Terms

- **PTO (Paid Time Off)** / **Folga Remunerada**: Paid leave days -- accrued every 6 months, NOT cumulative
- **Sick Day** / **Dia de Doenca**: Paid sick leave -- 3-4 days/year depending on category
- **Falta** / **Ausencia Nao-Justificada**: Unexcused absence when PTO and sick days exhausted -- impacts payroll
- **Red (Leadership)** / **Lideranca**: Leadership category employees -- 5 PTOs per cycle, 4 sick days/year
- **Liderados** / **Equipe**: Non-leadership employees -- standard PTO allocation, 3 sick days/year
- **Blackout Period** / **Periodo de Restricao**: Construction peak season -- requires 2 weeks advance notice for PTO
- **Workers Comp** / **Seguro de Acidentes de Trabalho**: Mandatory worker injury insurance (Chapter 440)
- **W9** / **Formulario Fiscal W9**: Required tax form for any sub receiving > $300/year
