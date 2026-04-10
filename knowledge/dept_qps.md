# QPS (Quality, Performance & Standards) - Lakeshore Development

## Visao Geral
- **Missao:** Garantir a qualidade de execucao em todas as fases da construcao, monitorar performance de subcontratados e departamentos, estabelecer e aplicar padroes de qualidade, seguranca e conformidade regulatoria em toda a operacao da Lakeshore
- **Lider:** Ana Maria M Gouveia (QPS Manager)
- **Equipe:**
  - **QPS Monitors/Inspectors:**
    - Donald Darby (Donaldo/Don) -- QPS Inspector, verificacao final (FCC), ~60 casas/dia
    - Fortine (Leo) -- QPS Inspector, controle de qualidade, reprovacoes, ~60 casas/dia
    - Daniel Consorte -- QPS Inspector, FCC (Final Construction Check) phases, walkthrough reports
  - **Analytics/BI:**
    - Diego Araujo -- Analytics, dashboards, extracao de dados, Power BI
    - Rost (Horst Flechtner) -- Gestao de rotas, controle de casas fechadas, dashboards
- **Departamentos relacionados:** Supervisao (verificacao de campo), Inspecao (resultados de inspecoes), Scheduling (rework frequency), Warranty (padroes de verificacao), Core Craft (rework handymen), Coordenador (escalacao)

## Processos

### Processo 1: Verificacao de Qualidade em Campo (Quality Control)
- **Objetivo:** Verificar a qualidade de execucao dos servicos em cada fase da construcao antes de permitir avanco para a proxima fase
- **Responsavel principal:** Don, Fortine (monitores QPS)
- **Frequencia:** Diaria (~60 casas/dia por monitor, rotas data-driven)
- **Ferramentas:** Builder Trend (daily logs, checklists), Photo/Video (evidencia obrigatoria), Dashboard de Construction Data

**Passo a passo:**
1. Receber lista de casas para verificacao (rota otimizada) -- Responsavel: Don/Fortine -- Ferramenta: Dashboard de rotas
2. Visitar casa e verificar servico contra checklist de qualidade -- Responsavel: Don/Fortine -- Ferramenta: Checklist BT
3. Documentar com fotos/video (OBRIGATORIO para toda finding) -- Responsavel: Don/Fortine -- Ferramenta: Camera/BT
4. Se aprovado: marcar como "Checklist Done" -- Responsavel: Don/Fortine -- Ferramenta: Builder Trend
5. Se reprovado: registrar issues, iniciar fluxo de rework -- Responsavel: Don/Fortine -- Ferramenta: Builder Trend
6. Actualizar daily log com resultado e evidencias -- Responsavel: Don/Fortine -- Ferramenta: Builder Trend

**Inputs:** Lista de casas com servicos concluidos (de Scheduling/Supervisao)
**Outputs:** Aprovacao ou reprovacao com evidencia; gatilho de pagamento (se aprovado) ou rework (se reprovado)
**Observacoes:** ALERTA CRITICO: Checklist Done = gatilho de pagamento. Sub pago nao volta para arrumar. Monitor deve ser criterioso antes de marcar.

### Processo 2: Quality Control 1 e Quality Control 2 (CPM)
- **Objetivo:** Duas verificacoes formais de qualidade no CPM, integradas na fase de closeout
- **Responsavel principal:** QPS Monitors (Don, Fortine, Daniel)
- **Frequencia:** Por casa, na fase final

**Quality Control 1:**
- Timing: Com Final Touches, no PRIMEIRO dia
- Verifica: todos os acabamentos, instalacoes, pintura, hardware
- Output: Lista de pendencias para correcao

**Quality Control 2:**
- Timing: Com Final Touches, no ULTIMO dia
- Verifica: correcoes do QC1 executadas, casa pronta para inspecao final
- Output: Aprovacao final para Building Final Inspection

### Processo 3: Face for Checklist Done (FCC)
- **Objetivo:** Verificacao presencial final de que a casa esta pronta para fechamento/entrega
- **Responsavel principal:** Donald Darby (Donaldo)
- **Frequencia:** Por casa (fase de closeout)
- **Ferramentas:** Dashboard de FCC, Builder Trend

**Passo a passo:**
1. Casa recebe status "Face for Requested" ou "Walkthrough Checklist Done" -- Ferramenta: Builder Trend
2. Donaldo monitora dashboard com duas secoes:
   - **Parte superior (prioritaria)**: casas com status "Face for Requested" / "Walkthrough Checklist Done" (precisam de FCC)
   - **Parte inferior**: casas ja com "Face for Checklist Done"
3. Donaldo visita a casa e faz o "Face for Check" -- verificacao completa
4. Apos verificacao aprovada: casa recebe status "Face for Checklist Done"
5. Se issues encontrados: correcoes solicitadas antes de marcar FCC

### Processo 4: Revisao de Daily Logs
- **Objetivo:** Garantir que daily logs de todos os departamentos cumprem os padroes de qualidade de dados
- **Responsavel principal:** QPS Team (Ana Maria)
- **Frequencia:** Diaria (audit continuo)

**Criterios de Revisao (IT-02):**

| Criterio | Requisito | Accao se Faltando |
|----------|-----------|-------------------|
| Accuracy de fase | Log deve corresponder a fase actual da casa | Flag, notificar Scheduling |
| Horas de equipe | Deve incluir horas reais, nao estimativas | Devolver ao submitter |
| Descricao do trabalho | Deve ser especifica (nao "worked on house") | Devolver com exemplo |
| Documentacao fotografica | Minimo 2 fotos por log: antes + depois ou progresso | Devolver, marcar "needs_revision" |
| Accuracy de tags | Tags BT devem corresponder ao status real | Corrigir tag, notificar Scheduling |
| Accuracy de data | Data do log deve corresponder a data real do trabalho | Flag se > 1 dia de gap |

**Correcao de inputs atrasados:**
- A data no banco e sempre a data de criacao do Daily Log
- Procedimento: inserir nota "Input atrasado" e informar data correcta para modificacao directa no BD

### Processo 5: Reestruturacao de Fases (Implementado Jan 2026)
- **Objetivo:** Simplificar fases de 5 para 4, eliminando sobreposicao operacional
- **Responsavel:** Ana Maria M Gouveia (QPS), aprovado por Bernardo + Leo

**Nova estrutura (4 fases):**
- **Fase 1 + 2**: Sem mudanca
- **Fase 3 (nova)**: equivale a antiga Fase 3.1 -- inicia no Drywall Checklist Done, termina no CO Issued
- **Fase 4 (nova)**: unifica antigas Fases 3.2 e 4 -- inicia no CO Issued, termina no Phase 4 Checklist Done

**Metas:**
- Eliminar sobreposicao entre fases (de 2 para 1 fase activa apos CO)
- Reduzir retrabalho pos-walkthrough
- Reduzir em 50% custos fora do escopo de reparo pos-walkthrough

## 53 Checklists de Qualidade (BT Job 455)

Baseado no caso completo Job 455, existem 53 checklists de verificacao cobrindo todas as fases:

### Phase 1: Pre-Construction (4 checklists)
1. Builder's Fee Bill | 2. UAL | 3. Contract Sign | 4. 1st Draw

### Phase 2: Permits (7 checklists)
5. Water Company Procedures | 6. Energy Company | 7. Permit Docs | 8. Apply Permit | 9. Permit Application Fee | 10. Permit Issued | 11. Permit Release Fee

### Phase 3: Land Preparation (13 checklists)
12. Clear Lot | 13. Stake House and Elevation | 14. Loads and Pad | 15. Compact Test | 16. Hub and Tack | 17. Doc-box | 18. Form | 19. Underground Plumbing | 20. Water Service | 21. Electric Underground | 22. Slab Preparation + Inspection | 23. Slab Pouring | 24. 2nd Draw

### Phase 4: Masonry and Roofing (6 checklists)
25. Masonry Assembly | 26. Lintel Inspection + Pouring | 27. Framing Assembly | 28. Fascia | 29. Roof (shingles) | 30. 3rd Draw

### Phase 5: Roughs (13 checklists)
31. Windows | 32. Plumbing Rough | 33. AC Rough | 34. Electrical Rough | 35. Lath | 36. Stucco | 37. Tub/Shower Pan | 38. Sewer Connection | 39. Batt Insulation | 40. Termite Treatment | 41. Electric Meter Conversion | 42. Blow-in Insulation | 43. 4th Draw

### Phase 6: Drywall (1 checklist)
44. Drywall

### Phase 7: Finishing (5 checklists)
45. Interior Paint | 46. Driveway | 47. Garage Door | 48. Tile | 49. Vinyl

### Phase 8: Trim (5 checklists)
50. AC Trim | 51. Cabinets + Countertops | 52. Trim Plumbing | 53. Trim Set | 54. Electric Trim

### Phase 9-11: Inspections + Final + Close-Out
55-65. Final inspections, clean, walkthrough, CO, accounting closed

## Inspection Pass/Fail Criteria

### 29 County Inspections (Const App Service Catalog)

| Code | Inspection | Pass Criteria | Fail Triggers |
|------|-----------|---------------|---------------|
| INS-001 | UP Inspection | Underground plumbing complete, no leaks, correct depth | Leaks, incorrect pipe size, missing cleanout |
| INS-002 | Slab Inspection | Rebar correct, plastic barrier, grounding in place | Missing rebar, gaps in vapor barrier |
| INS-003 | Lintel Inspection | Rebar junction slab-columns correct (Citrus only) | Incorrect rebar placement |
| INS-004 | Sheathing Inspection | Gable sheathing correct (Citrus only) | Gaps, incorrect nailing pattern |
| INS-005 | Structural Frame | All structural elements per plan (Citrus only) | Missing straps, incorrect spacing |
| INS-006 | Partial Roof/Dry In | Underlayment, flashing correct | Gaps in membrane, missing flashing |
| INS-008 | Rough Electric | Panel, outlets, GFCI/AFCI per code | Missing GFCI, incorrect wire gauge |
| INS-009 | Rough Plumbing | Pressure test passed, vent stack correct | Failed pressure test, missing vents |
| INS-010 | Rough AC | Ductwork, refrigerant lines correct | Duct leaks, incorrect sizing |
| INS-011 | Framing Inspection | ALL roughs approved + Dry In + straps | Missing strap, unapproved rough |
| INS-012 | Insulation Inspection | R-values correct + shingles + windows done | Incorrect R-value, missing insulation |
| INS-017 | Final Electric | All fixtures, GFCI/AFCI, smoke detectors | Missing GFCI, no smoke detector |
| INS-018 | Final Plumbing | All fixtures, water heater, gas connections | Leaks, missing fixtures |
| INS-019 | Final AC | HVAC operational, thermostat, duct test | Failed duct test, AC not cooling |
| INS-022 | Building Final | ALL final inspections + Blown Insulation + Blower Door + Appliances | Any prerequisite missing |

### Inspection Validation Sub-System (CPM)

O CPM define um sub-sistema completo para validacao de inspecoes:

**State Machine:**
```
Pre-inspection checklist done
  -> Scheduling and validation (waiting)
  -> Validation (pass/fail)
    -> Pass: Inspection scheduled -> Approved / Disapproved
    -> Fail: Rework -> Re-validation -> Re-inspection
```

**Rework Paths:**
- **Path A (Inspection Disapproved)**: Inspection fails -> Rework scheduled -> Rework done -> Re-validation -> Re-inspection
- **Path B (Validation Failed)**: Validation fails -> Rework scheduled -> Rework done -> Re-validation -> Proceed to inspection

**Status Codes:**
- `{INSPECTION} + SCHEDULED` -- Agendada com county
- `{INSPECTION} + INSPECTION APPROVED` -- Aprovada
- `{INSPECTION} + INSPECTION DISAPPROVED` -- Reprovada
- `{INSPECTION} + INSPECTION VALIDATED` -- Pre-validacao aprovada
- `{PRE-INSPECTION PROCESS} + REWORK SCHEDULED` -- Rework agendado
- `{PRE-INSPECTION PROCESS} + REWORK CHECKLIST DONE` -- Rework concluido

### Const App Inspection Module
- **6 tabs**: Overview, Inspections Flow, Pre-Inspection Analysis, Inspection Requests Matrix, Scheduled Inspections, Reprobation Analysis
- **Inspection Requests Matrix**: projectos rastreados em 17 categorias de construcao
- **Status Legend**: C=Not configured, -=Waiting, !=Pending, S/15=Scheduled for 15th, A=Today, P=Passed, 1=Failed once, P2=Passed 2nd attempt
- **Flow modes**: Unconfigured, Manual, Assisted, Auto
- **Reprobation Analysis**: Failed inspections analysis and pattern tracking

## Safety Regulations

### OSHA Requirements (Federal, enforced in Florida)
- **Fall protection**: Required at 6 feet for residential construction
- **Trench safety**: Shoring/sloping required for excavations > 5 feet
- **PPE requirements**: Hard hats, safety glasses, steel-toe boots on active sites
- **Jobsite safety plan**: Required
- **OSHA 10-Hour Construction**: Recommended for all field workers
- **Silica exposure**: Wet cutting required (respirable crystalline silica standard)

### Florida Building Code (FBC 8th Edition, 2023)
- All construction must comply with FBC Residential, Energy Conservation, Fuel Gas
- Wind speed zones vary by county (critical for structural design and product approvals):
  - Charlotte County: 140-150 mph
  - Marion, Citrus, Orange: varies
- **Flood zone**: FEMA flood maps, elevation certificates in Special Flood Hazard Areas (SFHA)
- **Product approval**: All products must be Florida Product Approved (FL#) or Miami-Dade NOA
- **Energy code**: Mandatory blower door test, duct leakage test, HERS rating for new residential
- **Permit expiration**: 180 days without inspection activity

### Florida Statutes
- **Chapter 489**: Contracting -- licensing, qualifying agents, CGC/CBC license required
- **Chapter 553**: Building Construction Standards -- FBC adoption, local amendments, inspections
- **Chapter 713**: Construction Liens -- Notice to Owner (NTO) within 45 days, Claim of Lien within 90 days
- **Section 553.79**: Permit required before commencement of work
- **Section 553.6**: CO required before occupancy

### Insurance Requirements
- Builder's Risk Insurance during construction (QPS monitors expiration)
- Commercial General Liability (CGL) -- minimum $300,000 per occurrence
- Workers Compensation -- required for 1+ employees
- Subcontractor insurance verification -- must carry own WC and GL
- **QPS monitors insurance expiration dates** to prevent gaps

### Environmental
- Stormwater management: SWPPP required for sites > 1 acre
- Gopher tortoise surveys required before clearing
- Tree protection varies by county

## Performance KPIs por Departamento

### Quality Metrics Tracked

| Metric | Description | Target | Measurement |
|--------|-------------|--------|-------------|
| Defect rate per phase | Defects found per construction phase | < 5% of items inspected | Weekly per project |
| Rework percentage | Tasks requiring rework after completion | < 10% | Monthly per subcontractor |
| Inspection pass rate | First-time pass rate for municipal inspections | > 85% | Monthly per county |
| Daily log completeness | Required fields filled correctly | > 95% | Daily audit |
| Photo documentation rate | Logs with required photo evidence | 100% | Daily audit |
| Correction turnaround | Time from QPS flag to corrected resubmission | < 24 hours | Weekly |
| Route coverage | Houses visited vs assigned per day | > 80% | Daily per monitor |
| Construction cycle time | Days from permit to CO per house | Minimize | Monthly |
| Cost per square foot | Real cost vs budget | Within allowance | Per project |
| Sub performance score | Composite: rework rate + inspection pass rate + schedule adherence | > 80% | Monthly per sub |

### KPIs by Department

| Department | Key KPI | Target | How QPS Measures |
|------------|---------|--------|------------------|
| Scheduling | Schedule adherence (planned vs actual) | > 90% | Compare BT schedule dates vs checklist done dates |
| Supervisao | Checklist accuracy (correct done markings) | > 95% | QPS field verification of "done" items |
| Inspecao | First-time inspection pass rate | > 85% | Track approved vs disapproved per county |
| Compras | Material delivery on time | > 90% | Compare order ETA vs actual delivery |
| Financeiro | Draw processing time | < 5 business days | Track draw request to release |
| Core Craft | Rework completion time | < 48 hours | Track rework assignment to completion |
| Permits | Permit processing time | < 7 weeks | Track application to issuance |
| Warranty | Repair resolution time | < 5 business days | Track request to completion |

### Rework Triggers (Escalation Logic)

```
IF inspection_fail_rate > 15% for subcontractor (rolling 30-day window)
  THEN flag subcontractor for review:
    - Pull all failed inspections in last 30 days
    - Categorize failures (workmanship, material, design compliance)
    - Generate subcontractor performance report
    - Route to Supervisao for field assessment

Escalation:
  1st occurrence -> Standard correction request (24h window)
  2nd consecutive fail -> Supervisao alert + sub watch list
  3rd consecutive fail -> Coordenador alert + mandatory field review + work stoppage
  5+ consecutive fails -> Executive escalation + sub suspension + alternative sourcing via Compras
```

## Quality Gates in CPM Sequence

Quality gates are checkpoints where QPS verification is required before the project can advance:

| Gate | CPM Phase | What QPS Verifies | Blocks If Failed |
|------|-----------|-------------------|------------------|
| G1: Compact Test | FASE 1 | Soil compaction certification | Form cannot proceed |
| G2: Slab Inspection | FASE 2 | Rebar, plastic, grounding | Slab pouring blocked |
| G3: Framing Inspection | FASE 3 | ALL roughs + Dry In approved | Interior work blocked |
| G4: Insulation Inspection | FASE 3 | Insulation + shingles + windows | Drywall blocked |
| G5: Quality Control 1 | FASE 4 | All finishes, installations | Final touches start |
| G6: Quality Control 2 | FASE 4 | QC1 corrections verified | Building Final blocked |
| G7: Building Final | FASE 4 | All final inspections + Blower Door + Appliances | CO blocked |
| G8: FCC (Final Construction Check) | Close-Out | Complete house readiness | Walkthrough blocked |

### CPM Exceeding Costs Sub-System (QPS Role)

When costs exceed budget, QPS is involved in the approval workflow:
- **Client Hold**: QPS evaluates if cost overrun is due to quality issue
- **Changelog**: QPS verifies that change execution meets standards
- **Cost Approval Rate target**: 70%
- **Project Discontinuation Rate**: QPS monitors trends

## Documentacao Formal (Lista Mestra)

QPS manages the formal document system (Lista Mestra IT-01 to IT-11):

| Document | Purpose |
|----------|---------|
| IT-01 | Master Document List (Lista Mestra) |
| IT-02 | Daily Log Standards -- mandatory fields, tags, photo requirements |
| IT-03 to IT-11 | Department-specific work instructions |

### QPS-Specific Documents
- **Plano de Acao para Mudanca de Regra de Negocio**: Reestruturacao de fases (Jan 2026)
- **Dicionario de Qualidade para casas spec**: Padroes de qualidade por item
- **Modelo de relatorio de reparos de walkthrough**: Template de reporting
- **CPM Flowchart**: Sequencia de construcao com dependencias

## Const App -- QPS-Relevant Modules

### Verification Module
- **Pending Verifications**: Review and verify completed services
- **Filters**: Pending, Site Visits Today, Photo Review, Failed, Verified
- **Columns**: PO Number, Supplier, Service, Project, Completed At, Photos, Status
- **Site Visits**: Plan and manage verification routes (route optimization coming soon)

### Rework Module
- **Rework Queue**: Manage inspection items sent for rework
- **Filters**: Pending Assignment, Sent to Handymen, All Reworks
- **Handymen Kanban Board**: Drag-and-drop assignment to handymen
- **Completed History**: Full audit trail of all completed reworks

### Inspection Module
- **29 inspection types** in service catalog (INS-001 to INS-029)
- **Pre-Inspection Analysis Queue**: Review and validate manual inspections before routing
- **Inspection Requests Matrix**: Track across 17 construction categories per project
- **Reprobation Analysis**: Analyze failed inspections, track failure patterns

## Available Tools

| Tool | Parameters | Returns |
|------|-----------|---------|
| read_daily_logs | date (str, optional), house_id (str, optional) | Daily log entries |
| read_daily_log_detail | log_id (str) | Full daily log record |
| search_daily_logs | query (str) | Matching daily log entries |
| update_daily_log | log_id (str), corrections (list), status (str) | Updated log confirmation |
| create_daily_log | house_id (str), content (str), tags (list) | New daily log ID |

## Handoff Triggers

### Outbound (QPS sends TO other agents)

| When | Hand off to | Send | SLA |
|------|-------------|------|-----|
| Quality standards/checklists for field verification | supervisao | DOC: quality checklist, standards reference | 48h |
| Quality standards for warranty verification | warranty | DOC: quality checklist, verification standards | 48h |
| Lawn cut need reported by monitors | warranty | INFO: house_id, lawn condition, urgency | 24h |
| Non-compliance detected | coordenador | INFO: violation type, house_id, corrective action, deadline | immediate |
| Daily Log corrections required | any agent | INFO: log_id, corrections needed, deadline | 24h |
| Sub performance review (5+ failures) | coordenador + compras | INFO: sub name, failure history, suspension recommendation | immediate |
| Rework assigned to handyman | core_craft | INFO: house_id, rework items, priority | 24h |
| Insurance expiration warning | financeiro + contratos | INFO: sub/house, expiring policy, deadline | 48h |

### Inbound (QPS expects FROM other agents)

| When | Hand off to | Send | SLA |
|------|-------------|------|-----|
| Quality issue flagged in field | supervisao | INFO: issue description, house_id, phase, photos | 24h |
| Inspection failure patterns | inspecao | INFO: failure type, frequency, house_ids | 24h |
| Daily logs submitted for review | any agent | DOC: daily log entries for quality check | 24h |
| Rework frequency data | scheduling | INFO: rework events, service types, house_ids | 24h |
| Rework completion confirmation | core_craft | INFO: rework items completed, photos, handyman | 24h |

## Key Glossary Terms

- **FCC (Face for Checklist Done)**: Verificacao presencial final que confirma casa pronta para fechamento
- **Quality Control 1/2**: Duas verificacoes formais no CPM -- QC1 no primeiro dia de Final Touches, QC2 no ultimo
- **Rework**: Trabalho que precisa ser refeito apos reprovacao em inspecao ou verificacao de qualidade
- **Backcharge**: Cobranca retroativa ao subcontratado por trabalho deficiente
- **Checklist Done**: Confirmacao de servico concluido -- GATILHO DE PAGAMENTO (critico para QPS)
- **Inspection Hold**: Barra QUALQUER agendamento de inspecao (casa literalmente parada)
- **Final Hold**: Permite continuar construcao, barra apenas inspecoes finais
- **FMEA**: Failure Mode and Effects Analysis -- proposta de fluxo de identificacao de problemas (em desenvolvimento)
- **Blower Door Test**: Teste de estanqueidade de ar obrigatorio pelo FBC
- **Punch List**: Itens pendentes identificados no walkthrough final

---

## Navegacao

- [CPM Construction Sequence](cpm_construction_sequence.md) -- Sequencia completa com quality gates
- [CPM Sub-Systems](cpm_subsystems.md) -- Inspection Validation Sub-System detalhado
- [Job 455 Lifecycle](bt_analysis/construction_lifecycle_job455.md) -- 53 checklists reais
- [Florida Compliance](reference_florida_compliance.md) -- FBC, OSHA, lien law
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md) -- Handoffs QPS com todos os depts
- [CEO Directives](shared_ceo_directives.md) -- ROI-driven quality control
- **Departamentos relacionados:**
  - [Supervisao](dept_supervisao.md) -- verificacao de campo, checklist done
  - [Inspecao](dept_inspecao.md) -- inspecoes municipais, holds
  - [Scheduling](dept_scheduling.md) -- rework frequency, schedule adherence
  - [Warranty](dept_warranty.md) -- padroes de verificacao pos-entrega
  - [Core Craft](dept_core_craft.md) -- handymen para rework
