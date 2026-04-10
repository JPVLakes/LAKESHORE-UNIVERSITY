# Inspecao - Lakeshore Development

## Visao Geral
- **Missao:** Agendar, acompanhar e gerenciar todas as inspecoes municipais (county) necessarias durante a construcao, garantindo aprovacao em cada etapa e resolucao de reprovacoes e holds
- **Lider:** Dandara Souza (cpm2@lakeshoredevelopmentfl.com) - Responsavel por Inspecoes
- **Equipe:**
  - Dandara Souza - Responsavel principal (tambem atua em Utilities)
- **Departamentos relacionados:** Scheduling (servicos concluidos para inspecao), Supervisao/Field (verificacao previa), Financeiro (pagamento de fees e impact fees), Permits (status de holds e documentacao)

## Processos

### Processo 1: Agendamento de Inspecao
- **Objetivo:** Agendar inspecoes municipais nos sites dos condados conforme servicos sao concluidos, garantindo que a obra avance dentro das exigencias legais
- **Responsavel principal:** Dandara Souza
- **Frequencia:** Diaria
- **Ferramentas:** Sites dos condados (cada condado tem site diferente), Slack (canal de requests), Builder Trend (daily logs), Planilha de controle de inspecoes

**Passo a passo:**
1. Receber solicitacao de inspecao via canal do Slack (inspection requests) -- Responsavel: Dandara -- Ferramenta: Slack
2. Acessar site do condado especifico (Marion, Citrus ou Charlotte) -- Responsavel: Dandara -- Ferramenta: Site do condado
3. Agendar inspecao (normalmente para o dia seguinte; Citrus ate 15:30 do dia anterior) -- Responsavel: Dandara -- Ferramenta: Site do condado
4. Registrar no daily logs com tags e padroes -- Responsavel: Dandara -- Ferramenta: Builder Trend
5. Atualizar planilha de controle de inspecoes -- Responsavel: Dandara -- Ferramenta: Planilha Excel

**Inputs:** Solicitacao de inspecao (de Scheduling via Slack); servico concluido
**Outputs:** Inspecao agendada no site do condado; registro em daily logs e planilha
**Observacoes:** Prazo de agendamento varia por condado. Marion permite inspecoes aos sabados via SMS ao inspetor.

### Processo 2: Acompanhamento de Resultados de Inspecao
- **Objetivo:** Monitorar resultados das inspecoes (aprovacao/reprovacao) e manter registros atualizados para todas as equipes
- **Responsavel principal:** Dandara Souza
- **Frequencia:** Diaria
- **Ferramentas:** Sites dos condados, E-mail, Slack, Builder Trend, Planilha de controle

**Passo a passo:**
1. Verificar resultados por condado:
   - **Marion**: Notificacoes por e-mail + site do condado (mais completo) -- Responsavel: Dandara -- Ferramenta: E-mail, Site do condado
   - **Citrus**: Notificacoes via Slack do site do County (nem sempre corretas - sempre conferir no site) -- Responsavel: Dandara -- Ferramenta: Slack, Site do condado
   - **Charlotte**: Verificar diretamente no site do County -- Responsavel: Dandara -- Ferramenta: Site do condado
2. Transferir resultados para Builder Trend e Jogs -- Responsavel: Dandara -- Ferramenta: Builder Trend
3. Atualizar planilha de controle com codificacao:
   - **R** = Requested (cor branca) + data
   - **A** = Agendada para hoje (cor azul ciano)
   - **P** = Passou/Aprovada (verde)
   - **1, 2, 3...** = Numero de reprovacoes (vermelho)
   - **Numero + asterisco** = Reinspecao agendada para hoje
   - **P + numero** = Aprovada apos N reprovacoes (verde diferente)
   -- Responsavel: Dandara -- Ferramenta: Planilha Excel
4. Calcular estatisticas: percentual de aprovacao por inspecao e por casa -- Responsavel: Dandara -- Ferramenta: Planilha Excel

**Inputs:** Resultados de inspecao (de sites dos condados, e-mail)
**Outputs:** Registros atualizados no Builder Trend e planilha; estatisticas de aprovacao
**Observacoes:** Resultados do Citrus via Slack nem sempre sao precisos -- sempre confirmar no site. Cada condado tem regras diferentes para notificacao.

### Processo 3: Gestao de Holds (Inspection Hold e Final Hold)
- **Objetivo:** Identificar, registrar e acompanhar holds que impedem o progresso de inspecoes ou da obra
- **Responsavel principal:** Dandara Souza
- **Frequencia:** Continua (sob demanda)
- **Ferramentas:** Builder Trend (daily logs, card fixo), Sites dos condados, E-mail

**Passo a passo:**
1. Identificar hold por notificacao do condado ou durante tentativa de agendamento -- Responsavel: Dandara -- Ferramenta: Site do condado, E-mail
2. Classificar tipo de hold:
   - **Inspection Hold**: Barra QUALQUER agendamento de inspecao (casa literalmente parada, ex: problema com cerca, erosion control)
   - **Final Hold**: Permite continuar construcao, barra apenas inspecoes finais (ex: water main extension, modificacao de documentos)
   -- Responsavel: Dandara -- Ferramenta: [analise operacional]
3. Registrar no daily logs e card fixo do Builder Trend -- Responsavel: Dandara -- Ferramenta: Builder Trend
4. Comunicar equipes afetadas (Scheduling, Supervisao) -- Responsavel: Dandara -- Ferramenta: Slack
5. Checar manualmente TODOS OS DIAS se hold foi removido (NAO ha notificacao automatica) -- Responsavel: Dandara -- Ferramenta: Site do condado
6. Para holds de modificacao: acompanhar ate aprovacao do documento -- Responsavel: Dandara -- Ferramenta: Site do condado

**Inputs:** Notificacao de hold do condado; problemas identificados em campo
**Outputs:** Registro de hold; comunicacao para equipes; resolucao de hold
**Observacoes:** NAO ha notificacao quando hold e removido -- precisa checar manualmente todos os dias. Holds de modificacao impactam todas as inspecoes ate aprovacao do documento. Em Marion: informacoes no portal online + e-mail quando entra em hold.

### Processo 4: Inspecoes Finais e Codigo de Acesso
- **Objetivo:** Gerenciar as inspecoes finais da casa, incluindo envio de codigo de acesso ao inspetor e verificacao de pendencias
- **Responsavel principal:** Dandara Souza
- **Frequencia:** Por casa (na fase final)
- **Ferramentas:** SMS, Sites dos condados, Builder Trend

**Passo a passo:**
1. Verificar pendencias: inspecoes nao realizadas na lista "available to request" -- Responsavel: Dandara -- Ferramenta: Site do condado
2. Verificar fees pendentes que possam bloquear inspecao -- Responsavel: Dandara -- Ferramenta: Site do condado
3. Agendar inspecao final -- Responsavel: Dandara -- Ferramenta: Site do condado
4. NO DIA da inspecao: verificar nome do inspetor no site do condado -- Responsavel: Dandara -- Ferramenta: Site do condado
5. Enviar codigo de acesso (electronic lock) ao inspetor via SMS -- Responsavel: Dandara -- Ferramenta: SMS
6. Acompanhar resultado da inspecao final -- Responsavel: Dandara -- Ferramenta: Site do condado, E-mail

**Inputs:** Casa com servicos concluidos; codigo de acesso da casa; informacao de fees pendentes (Financeiro)
**Outputs:** Inspecao final agendada e acompanhada; resultado registrado
**Observacoes:** Inspetor reprova automaticamente se nao conseguir entrar na casa. Impact fees bloqueiam Final Electric em Marion (dependencia do Financeiro).

### Processo 5: Cancelamento e Reagendamento de Inspecoes
- **Objetivo:** Cancelar ou reagendar inspecoes quando servico nao esta pronto ou condicoes nao permitem
- **Responsavel principal:** Dandara Souza
- **Frequencia:** Sob demanda
- **Ferramentas:** Sites dos condados, Telefone, SMS

**Passo a passo:**
1. Receber informacao de que inspecao precisa ser cancelada -- Responsavel: Dandara -- Ferramenta: Slack
2. Se antes do dia: cancelar pelo site do condado -- Responsavel: Dandara -- Ferramenta: Site do condado
3. Se no dia: falar diretamente com inspetor (nem sempre atende) -- Responsavel: Dandara -- Ferramenta: Telefone
4. Atualizar planilha de controle e daily logs -- Responsavel: Dandara -- Ferramenta: Planilha Excel, Builder Trend
5. Para reinspecao apos reprovacao:
   - Em Citrus: pagar fee ANTES de reagendar (a partir de 2a/3a reprovacao) -- Responsavel: Dandara + Financeiro -- Ferramenta: Site do condado
   - Em Marion: fee paga no final -- Responsavel: Dandara -- Ferramenta: Site do condado

**Inputs:** Solicitacao de cancelamento; resultado de reprovacao
**Outputs:** Inspecao cancelada ou reagendada; fee paga quando aplicavel
**Observacoes:** Cancelamento no dia e muito dificil -- depende de contato direto com inspetor.

## Regras de Dependencia entre Inspecoes
- **Drain**: So passa se roof penetrations estiverem prontas (feitas no momento do rough AC)
- **Frame**: Precisa de TODOS os roughs aprovados + drain aprovado
- **Insulation**: Apos frame aprovado
- **Subsiding**: Sempre pedido junto do Roof Assembly
- **Water Service**: Sempre pedido junto do UP
- **Septic**: Inspetor privado, nao agenda no County, registro diferente

## Variacoes por Condado

| Aspecto | Marion | Citrus | Charlotte |
|---------|--------|--------|-----------|
| Notificacao resultado | E-mail + site | Slack (nem sempre preciso) + site | Site apenas |
| Fee de reinspecao | A partir de 2a/3a reprovacao, paga no final | Paga ANTES de reagendar | A definir |
| Inspecao sabado | Possivel via SMS ao inspetor | - | - |
| Prazo agendamento | Dia seguinte | Ate 15:30 do dia anterior | - |
| Final Electric | Requer pagamento de impact fees | - | Utilities por depto separado |
| Contato com inspetores | Mais facil | Mais ou menos | Dificil |
| Holds | Portal online + e-mail | E-mail/comunicacao direta | - |

## Dores e Problemas Conhecidos
- **Sem notificacao de remocao de hold**: Precisa checar manualmente todos os dias
- **Sistemas diferentes por condado**: Cada um com regras, sites e processos proprios
- **Resultados imprecisos via Slack (Citrus)**: Sempre precisa conferir no site
- **Cancelamento no dia**: Dependente de contato direto com inspetor
- **Fees bloqueiam reagendamento (Citrus)**: Precisa coordenar com financeiro
- **Impact fees bloqueiam Final Electric (Marion)**: Dependencia do financeiro
- **Holds de modificacao**: Param toda a casa ate aprovacao
- **Codigo de acesso manual**: Todo dia verificar finals, buscar inspetor, enviar SMS

## Dependencias
- **Recebe de:** Scheduling -> servicos concluidos prontos para inspecao; Supervisao/Field -> verificacao previa de qualidade; Financeiro -> pagamento de fees e impact fees; Permits -> status de holds, permit number
- **Entrega para:** Scheduling -> resultados de inspecao (aprovada libera proximo passo; reprovada exige rework); Supervisao -> notificacao de reprovacoes para resolucao; Financeiro -> informacao de fees necessarias; Warranty -> inspecoes finais aprovadas para fechamento

---

## Documentacao Formal (Fonte: Drive QPS)

### SOP 1: Verificacao de Resultado de Inspecao

- **Objetivo:** Processo padronizado para verificacao de resultados das inspecoes realizadas pelos Countys
- **Responsavel:** Departamento de Inspecoes
- **Documentos de referencia:** Planilha Lakeshore (aba Inspections) + Planilha Inspections Database

**Passo a passo (SOP formal):**
1. Acessar a rotina de inspecoes do dia (gerada ao final do dia anterior) com numero do permit e codigo da inspecao
2. Entrar no site do County correspondente e verificar se o resultado esta disponivel
3. Com o resultado aberto: tirar print da tela e copiar nota do inspetor
4. Enviar o print e o comentario (quando existente) para o grupo do WhatsApp da Fase correspondente; se reprovado, enviar tambem para o grupo Disapproved
5. Atualizar a planilha de Permit com o resultado
6. Atualizar a data do Schedule no Buildertrend com a data de aprovacao da inspecao
7. Atualizar o Daily Logs no Buildertrend

**Registros:** Planilha Inspections - Database

---

### SOP 2: Agendamento de Inspecao

- **Objetivo:** Processo padronizado para agendamento das inspecoes realizadas pelos Countys
- **Responsavel solicitante:** Departamento do Field (solicita)
- **Responsavel executor:** Departamento de Inspecoes (verifica e agenda)

**Passo a passo (SOP formal):**
1. Receber a solicitacao de agendamento via grupo de WhatsApp "Inspection Request"
2. Verificar na Planilha Lakeshore se a inspecao requisitada possui criterios especificos (inspecoes predecessoras obrigatorias)
3. Verificar no Daily Logs se a etapa para a qual foi solicitada a inspecao esta concluida
4. Com o numero do permit e o codigo da inspecao, realizar o agendamento no site do County
5. Confirmar o agendamento: reagir com emoji de verificacao na mensagem do WhatsApp Inspection Request
6. Atualizar a data do Schedule no Buildertrend com a data do primeiro agendamento
7. Atualizar a Planilha Lakeshore com a data do agendamento
8. Ao final da tarde (entre 17h30 e 17h44): atualizar a planilha com todas as inspecoes agendadas para o dia seguinte e enviar a rotina de inspecoes no grupo do Slack + grupo WhatsApp Inspection Request

**Registros:** Planilha Lakeshore - Database

---

### Dados de Predecessores (Codigos e Dependencias)

Tabela de dependencias formais entre inspecoes, com codigos do County:

| Inspecao | Codigo | Predecessora obrigatoria | Servico prerequisito |
|---|---|---|---|
| Underground | 243 | - | Underground Plumbing |
| Water Service | 246 | Underground (243) | - |
| Slab | 120 | - | Slab Prep + Electric Underground |
| Lintel | 119 | - | Masonry Assembly |
| Roof Assembly | 124 | - | Roof Assembly |
| TUG | 214 | Roof Assembly (servico para eletricista - confirmar com Sam) | TUG Install |
| Dry In | 152 | Rough AC + Insulation | Dry In |
| Rough Plumbing | 244 | - | Rough Plumbing + Water Meter Install |
| Lath | 118 | - | Lath |
| Rough AC | 264 | - | Rough AC |
| Rough Electric | 208 | Rough AC (264) | Rough Electric |
| Framing | 113 | Dry In (152) + Rough Plumbing (244) + Rough AC (264) + Rough Electric (208) | Windows/Ext. Doors + Shingles |
| Insulation | 262 | Rough AC (264) | Insulation + Shingles + Windows/Ext. Doors |
| Driveway Form Up | 354 | - | Driveway Preparation |
| Sidewalk | 125 | Driveway Form Up (354) | Driveway Preparation |
| Septic DOH (Health Dept) | 525 | - | Septic Install |
| Sewer Septic | 245 | - | Septic Connection (cano exposto) |
| Final Plumbing | 241 | Water Service (246) + Water Meter Install + Plumbing Trim + Sewer Septic (245) | - |
| Final AC | 260 | - | Blown-in Insulation + Electric Trim + AC Trim + AC ligado/vacuum |
| Final Electric | 201 | - | Electric Trim + Meter |
| Building Final | 108 | Final Plumbing (241) + Final Electric (201) + Final AC | Sod Order + Final Paint |
| Final Driveway | 352 | Septic | - |
| Pre Power | - | Final Electric (a confirmar) | Electric Trim |

**Codigos adicionais Marion County:** Pre Power (213), Electric Underground (210)

---

### Dados Estatisticos de Inspecoes

#### Taxas de aprovacao e reprovacao por tipo de inspecao (Marion County - base historica)

| Inspecao | Codigo | Total | Aprovadas | Reprovadas | % Aprovacao | % Reprovacao |
|---|---|---|---|---|---|---|
| Underground | 243 | 50 | 44 | 6 | 88% | 12% |
| Water Service | 246 | 34 | 30 | 4 | 88% | 12% |
| Slab | 120 | 46 | 40 | 6 | 87% | 13% |
| Lintel | 119 | 36 | 31 | 5 | 86% | 14% |
| Roof Assembly | 124 | 49 | 28 | 21 | 57% | **43%** |
| TUG | 214 | 27 | 24 | 3 | 89% | 11% |
| Rough Electric | 208 | 30 | 20 | 10 | 67% | 33% |
| Rough Plumbing | 244 | 27 | 22 | 5 | 81% | 19% |
| Rough AC | 264 | 33 | 27 | 6 | 82% | 18% |
| Lath | 118 | 23 | 22 | 1 | 96% | 4% |
| Dry In | 152 | 31 | 27 | 4 | 87% | 13% |
| Framing | 113 | 16 | 13 | 3 | 81% | 19% |
| Insulation | 262 | 10 | 9 | 1 | 90% | 10% |
| Health Dept (Septic DOH) | 525 | 8 | 5 | 3 | 63% | 38% |
| Sewer Septic | 245 | 9 | 8 | 1 | 89% | 11% |
| Sidewalk | 125 | 6 | 4 | 2 | 67% | 33% |
| Driveway Form Up | 354 | 5 | 3 | 2 | 60% | 40% |
| Driveway Final | 352 | 2 | 1 | 1 | 50% | 50% |
| Final Electric | 201 | 2 | 2 | 0 | 100% | 0% |
| Final Plumbing | 241 | 2 | 1 | 1 | 50% | 50% |
| Final AC | 260 | 3 | 2 | 1 | 67% | 33% |
| Building Final | 108 | 3 | 1 | 2 | 33% | **67%** |

**Destaques criticos (maiores taxas de reprovacao):**
- Roof Assembly: 43% de reprovacao (maior volume de falhas absolutas: 21 reprovacoes em 49 inspecoes)
- Building Final: 67% de reprovacao (base ainda pequena: 3 inspecoes)
- Driveway Form Up: 40% de reprovacao
- Health Dept (Septic DOH): 38% de reprovacao

#### Analise de falhas em Roof Assembly (dados detalhados por casa)

Principais causas de reprovacao na inspecao de Roof Assembly:
- **Hangers ausentes ou incorretos:** Falta de hangers nas trusses (bearing walls), hangers com pregos incorretos (deve ser 16D para 2-ply ou mais)
- **Straps instalados incorretamente:** Straps nao presos corretamente, faltando em bearing walls, parafusos incorretos (tap-cons)
- **Bracing incompleto:** Bracing nao realizado ou incompleto
- **Fill cells:** Compensado nao removido das fill cells
- **Bucks incompletos:** Bucks nao realizados
- **Engenharia faltando ou incompativel:** Carta de engenheiro ausente, engenharia nao bate com as trusses
- **Inspecao solicitada antes da conclusao do servico:** Casos em que o servico nao estava pronto no momento do agendamento

**Impacto do checklist:** Casos sem checklist preenchido previamente apresentaram maior incidencia de reprovacao. Introducao do checklist a partir de Out/Nov 2023 para casas fase 2+.

#### Dados de atraso por reprovacao (amostra Dez 2023 - Jan 2024)

| Inspecao | Fase | Casa(s) com maior atraso | Dias de atraso |
|---|---|---|---|
| Sewer Septic | 3 | Casa 10 | 23 dias |
| Framing | 3 | Casa 19 | 21 dias |
| Rough Electric | 3 | Casa 57 (3 reprovacoes) | 12+ dias |
| Insulation | 3 | Casa 33 (4 reprovacoes) | 16 dias |
| Roof Assembly | 2 | Casa 35 (2 reprovacoes) | 10 dias |
| Rough Electric | 4 | Casa 3 | 10 dias |

- **Media de atraso por reprovacao unica:** 2-7 dias uteis
- **Multiplas reprovacoes**: podem acumular 10-23 dias de atraso por inspecao

---

## Descricao de Cargo Formal (Fonte: Drive Lakeshore)

### Coordenador de Inspecoes

- **Setor:** Utilities & Inspections — Inspections
- **Descricao geral:** Realizar agendamentos, acompanhamentos e registrar os resultados das inspecoes nos sistemas
- **Principais responsabilidades:**
  - Verificar solicitacoes de inspecoes no Slack e realizar agendamentos no site do county
  - Registrar resultados de inspecoes nos sistemas (Buildertrend — schedule e daily logs — e planilha)
  - Sinalizar inspection holds e acompanhar resolucao
  - Conferir fees para pagamento no site do county e encaminhar ao financeiro
  - Informar codigo de acesso das casas para inspetores (Finals inspections)
  - Realizar download do CO (Certificate of Occupancy) no site do county, upload no Buildertrend e enviar para o Gerente Geral de Projetos

---

## CPM Construction Sequence Reference

The CPM flowchart defines the complete inspection sequence and county-specific variations that the Inspecao department must follow.

**Full Inspection Sequence (in construction order):**
1. UP Inspection (Underground Plumbing)
2. Slab Inspection
3. Lintel Inspection (Citrus only)
4. Sheating Inspection (Citrus only) / Roof Assembly Inspection (Marion)
5. Structural Frame Inspection (Citrus only) / Sub-siding Inspection (Marion)
6. TUG Inspection
7. DOH Inspection (Citrus only -- septic)
8. Sewer Septic Inspection (Marion only)
9. Dry In Inspection
10. Rough Plumbing, Rough AC, Rough Electric Inspections (group -- suggest same day)
11. Lath Inspection
12. Framing Inspection (suggest same day as Roughs; requires ALL Roughs + Dry In approved)
13. Insulation Inspection (requires insulation + shingles + windows)
14. Driveway Internal Inspection (Citrus) / Driveway Form Up + Sidewalk Inspections (Marion)
15. Final Utilities Inspection (Citrus only) / Water Service Inspection (Marion only)
16. Pre-Power Inspection (Citrus only)
17. Final Plumbing, Final Electric, Final AC Inspections
18. Final Roof Inspection
19. Final Driveway Inspection
20. Building Final Inspection (requires items 17-19 + Blown-in + Blower Door + Appliances)

**County Differences Summary:**

| Inspection | Marion | Citrus |
|-----------|--------|--------|
| Lintel Inspection | Skip | Required |
| Structural Frame / Sheating | Roof Assembly + Sub-siding | Structural Frame + Sheating |
| DOH (Septic) | Skip | Required |
| Sewer Septic | Required | Skip |
| Driveway | Form Up + Sidewalk (county) | Internal (Lakeshore) |
| Final Utilities | Skip (use Water Service) | Required |
| Water Service | Required | Skip |
| Pre-Power | Skip | Required |

**Inspection Validation Sub-System:** Defines the full state machine for validation -> scheduling -> result -> rework. See [cpm_subsystems.md](cpm_subsystems.md) for complete flow.

**Full reference:** [cpm_construction_sequence.md](cpm_construction_sequence.md) | [cpm_subsystems.md](cpm_subsystems.md)

---

## County Portal URLs

County portals used for inspection scheduling, result checking, and hold monitoring. These are the same public government portals used by the Permits department.

| County | Portal URL | Status | Capabilities |
|--------|-----------|--------|-------------|
| **Marion County** | https://aca-prod.accela.com/MARION/ | Active | Inspection scheduling, results, holds |
| **Citrus County** | https://aca3.accela.com/CitrusCounty/ | Active | Inspection scheduling, results |
| **Lake County** | https://aca.lakecountyfl.gov/ | Active | Inspection results only |
| **Charlotte County** | https://www.charlottecountyfl.gov/ | Planned | Not yet integrated |
| **Sumter County** | https://www.sumtercountyfl.gov/building | Planned | Not yet integrated |

**Notes:**
- Marion County: Results available via email notifications AND portal. Holds visible on portal with email notification when entering hold. Inspections can be scheduled for Saturdays via SMS to inspector.
- Citrus County: Results sometimes sent via Slack from county system, but NOT always accurate -- always confirm on the portal. Scheduling deadline: 15:30 the day before.
- Lake County: Portal has intermittent downtime; limited to result viewing only
- Charlotte and Sumter are planned for future integration
- Portal URLs tracked in county_portal_registry.json with last-verified dates

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- [Catalogo de Dores](07_CATALOGO_DORES.md)
- [Fluxo Spec Home](05_FLUXO_SPEC_HOME.md)
- [Fluxo Custom Home](06_FLUXO_CUSTOM_HOME.md)
- [Glossario de Termos](03_GLOSSARIO.md)
- **Departamentos relacionados:**
  - [Scheduling](dept_scheduling.md) — envia servicos concluidos prontos para inspecao; recebe resultados
  - [Supervisao](dept_supervisao.md) — faz verificacao previa de qualidade antes da inspecao
  - [Financeiro](dept_financeiro.md) — paga fees e impact fees; recebe informacao de fees necessarias
  - [Permits](dept_permits.md) — fornece status de holds e permit number
  - [Warranty](dept_warranty.md) — inspecoes finais aprovadas marcam fechamento de casa

## Key Glossary Terms

> Terms from [Glossario de Termos](03_GLOSSARIO.md) most relevant to the Inspecao (Inspection) department.

- **Inspection Hold** / **Retencao de Inspecao**: Hold that blocks ALL inspection scheduling -- house is completely stopped until resolved
- **Rough (Plumbing/Electric/AC)** / **Instalacao Bruta**: Pre-finish installation within walls -- three rough inspections must pass before frame
- **Certificate of Occupancy (CEO/CO)** / **Habite-se**: Certificate from county confirming house is fit for occupancy -- requires all inspections passed
- **Compact Test** / **Teste de Compactacao**: Soil compaction test before foundation -- failure delays all subsequent phases
- **Footing** / **Sapata/Radier de Fundacao**: Concrete foundation element distributing structural load -- inspected before concrete pour
- **Frame** / **Estrutura/Esqueleto**: Wood/steel skeleton of the house -- frame inspection is the most important Phase 2 inspection
- **Insulation** / **Isolamento Termico**: Thermal insulation in walls/ceiling -- inspection requires insulation + shingles completed
- **Partial Approval** / **Aprovacao Parcial**: Partial inspection pass -- allows work to continue while correcting failed items
- **Erosion Control** / **Controle de Erosao**: Measures to prevent soil erosion during construction -- violations cause Inspection Hold
- **Final Hold** / **Retencao Final**: Hold that allows construction but blocks final inspections (especially Final Electric)
- **Electronic Locker** / **Fechadura Eletronica**: Digital code lock on house for inspector access -- code sent by SMS on inspection day
- **MEP (Mechanical, Electrical, Plumbing)** / **Mecanica, Eletrica, Encanamento**: Combined services package -- Full MAP indicates bundled MEP

---

## BuilderTrend Job 455 -- Real Data (Supplement)

### Inspections on Job 455
| Inspection | Date | Result | Phase |
|-----------|------|--------|-------|
| UP Inspection | Feb 27-28, 2025 | Passed | Foundation |
| Water Service Inspection | Feb 27-28, 2025 | Passed | Foundation |
| Slab Inspection | Mar 5-6, 2025 | Passed | Foundation |
| Lintel Inspection | Mar 14-17, 2025 | Passed | Masonry |
| Septic Inspection | May 2025 | Passed ($150) | Roughs |
| Blower Door Test | Aug 2025 | Passed ($175) | Final |
| Building Final Inspection | ~Aug-Sep 2025 | Passed | Final |
| CO Issued | Sep 2025 | Approved | Close-out |

### Inspection Vendors on Job 455
| Service | Vendor | Cost |
|---------|--------|------|
| Septic Inspection | Rapid Septic Consulting LLC | $150 |
| Blower Door Test | Richard Job LLC | $175 |
| County Inspections | Marion County Building Safety | Included in permit fees |

### All 29 Inspection Types (Const App Service Catalog)
INS-001: UP Inspection, INS-002: Slab Inspection, INS-003: Lintel Inspection, INS-004: Sheathing Inspection, INS-005: Structural Frame Inspection, INS-006: Partial Roof/Dry In, INS-007: TUB Meter, INS-008: Rough Electric, INS-009: Rough Plumbing, INS-010: Rough AC, INS-011: Framing, INS-012: Insulation, INS-013: Lath, INS-014: Driveway Form UP, INS-015: Final Driveway, INS-016: Soffit In Progress, INS-017: Final Electric, INS-018: Final Plumbing, INS-019: Final A/C, INS-020: Final Roof, INS-021: Final Utilities, INS-022: Building Final, INS-023: T-Pole, INS-024: Footer, INS-025: Gas Rough, INS-026: Fireplace Install, INS-027: Drywall & Firewall, INS-028: Water Service & Sewer, INS-029: Final Grade Lot

## CPM Construction Sequence -- Inspection Deep Dive

### Inspection Validation Sub-System (Complete State Machine)
The CPM defines a detailed inspection lifecycle:
1. **Pre-inspection checklist done** -> triggers inspection scheduling
2. **Validation check** -> supervisor validates work quality before county inspection
3. **Inspection scheduled** with county
4. **Result**: Approved or Disapproved
5. **If disapproved**: Rework scheduled -> Rework checklist done -> Re-validation -> Re-inspection
6. **If validation failed**: Rework scheduled -> Re-validation -> Proceed to inspection

### Status Codes for Inspection Tracking
| Code | Meaning |
|------|---------|
| `{INSPECTION} + SCHEDULED` | Scheduled with county |
| `{INSPECTION} + INSPECTION APPROVED` | Passed |
| `{INSPECTION} + INSPECTION DISAPPROVED` | Failed |
| `{INSPECTION} + INSPECTION VALIDATED` | Pre-inspection validation passed |
| `{INSPECTION} + CANCELED` | Canceled |
| `{PRE-INSPECTION PROCESS} + REWORK SCHEDULED` | Rework scheduled after failure |
| `{PRE-INSPECTION PROCESS} + REWORK CHECKLIST DONE` | Rework completed |
| `NOT READY FOR INSPECT` | Pre-inspection checklist not done |

### County-Specific Inspection Differences
| Inspection | Marion | Citrus |
|-----------|--------|--------|
| Lintel | Skip | Required |
| Structural Frame | Roof Assembly Inspection | Required |
| Sheating | Sub-siding Inspection | Required |
| Sewer Septic | Required | Not required |
| Water Service | Required | Covered by Final Utilities |
| Final Utilities | Not required | Required |
| Pre-Power | Not required | Required |
| DOH | Not required | Required |

### Building Final Inspection Prerequisites (from CPM)
ALL of these must be completed before Building Final can be scheduled:
1. Final Plumbing Inspection
2. Final Electric Inspection
3. Final AC Inspection
4. Final Driveway Inspection
5. Blown in Insulation
6. Blower Door Test
7. Appliances Install

## Const App Integration (Supplement)

### Inspection Module Features
- **Inspections Flow**: Configure triggers for each inspection (Manual, Assisted, Auto modes)
- **Pre-Inspection Analysis Queue**: Validate inspections before routing to requests
- **Inspection Requests Matrix**: Track 17 construction categories per project with status legend
- **Scheduled Inspections**: Manage appointments by date (today, this week, all scheduled)
- **Reprobation Analysis**: Analyze failed inspections; identify patterns for resolution
- **Legend**: C=Not configured, -=Waiting, !=Pending, S/15=Scheduled 15th, A=Today, 1=Failed once, 1/8=Failed+rescheduled, P=Passed, P2=Passed 2nd attempt
