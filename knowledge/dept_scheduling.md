# Scheduling - Lakeshore Development

## Visao Geral
- **Missao:** Gerenciar o agendamento de todos os servicos de construcao nas tres fases da obra (pre-construction/fundacao, rough/estrutura, finish/acabamento), coordenando subcontratados, materiais e prazos para cada casa
- **Lider:** Daniela Santiago - Scheduler Fase 3 / Lideranca de Scheduling
- **Equipe:**
  - **Fase 1 (Pre-Construction/Fundacao):**
    - Mauricio Vieira - Scheduler Fase 1
    - Giovana Sousa (gsousa@lakeshoredevelopmentfl.com) - Scheduler Fase 1
  - **Fase 2 (Rough/Estrutura):**
    - Joao Victor Serra (jserra@lakeshoredevelopmentfl.com) - Scheduler Fase 2
    - Thercyo Augusto Pereira (tpereira@lakeshoredevelopmentfl.com) - Scheduler Fase 2
  - **Fase 3 (Finish/Acabamento):**
    - Daniela Santiago - Scheduler Fase 3 (lideranca)
    - Antonio Santos (asantos@lakeshoredevelopmentfl.com) - Scheduler Fase 3
    - Guilherme Barbosa (gbarbosa@lakeshoredevelopmentfl.com) - Scheduler Fase 3
- **Departamentos relacionados:** Supervisao/Field, Financeiro (draws), Permits, Budget/Takeoff, Compras, Warehouse, Client Relations, Inspecao

## Processos

### Processo 1: Agendamento Fase 1 - Pre-Construction/Fundacao
- **Objetivo:** Gerenciar todas as etapas iniciais da construcao, desde a limpeza do terreno ate a preparacao da fundacao (form)
- **Responsavel principal:** Mauricio Vieira / Giovana Sousa
- **Frequencia:** Diaria (acompanhamento continuo de multiplas casas)
- **Ferramentas:** Builder Trend (daily logs, POs, schedule), WhatsApp (90%+ comunicacao com subs), Planilha pessoal (Google Sheets), ClickUp (Mauricio), Sites de condados (Property Appraiser)

**Passo a passo:**
1. Identificar nova casa disponivel pela tag "Survey Received" no daily logs -- Responsavel: Mauricio / Giovana -- Ferramenta: Builder Trend
2. **Clear Lot (Limpeza do terreno):**
   - Verificar se o stake lot esta no lugar (via monitores/topografo) -- Responsavel: Mauricio -- Ferramenta: Slack (monitores)
   - Enviar site plan ou levantamento topografico para o sub via WhatsApp -- Responsavel: Mauricio / Giovana -- Ferramenta: WhatsApp
   - Consultar Property Appraiser para dados do lote (tamanho) -- Responsavel: Mauricio / Giovana -- Ferramenta: Site do condado
   - Agendar servico com sub -- Responsavel: Mauricio / Giovana -- Ferramenta: WhatsApp
   - Registrar no daily logs, preencher POs, atualizar schedule -- Responsavel: Mauricio / Giovana -- Ferramenta: Builder Trend
3. **Stake House** - Pre-agendar quando clear lot esta proximo da conclusao -- Responsavel: Mauricio -- Ferramenta: WhatsApp
4. **Calculo de Loads** - Supervisores calculam loads apos stake house -- Responsavel: Supervisores -- Ferramenta: [equipamento de campo]
5. **Pad** - Agendar apos entrega dos loads; supervisor confirma elevacao correta -- Responsavel: Mauricio / Giovana -- Ferramenta: WhatsApp, Builder Trend
6. **Compact Test** - Crucial, pode falhar e atrasar todo o cronograma -- Responsavel: Mauricio -- Ferramenta: WhatsApp (sub de teste)
7. **Robintec** - Pedido junto com compact test por questao de prazo -- Responsavel: Mauricio -- Ferramenta: WhatsApp
8. **Form** - Nao pode avancar sem resultado do compact test -- Responsavel: Mauricio -- Ferramenta: WhatsApp

**Para cada agendamento de servico, repetir:**
- Enviar solicitacao no grupo de WhatsApp
- Enviar documentos necessarios (site plan, survey, etc.)
- Preencher daily logs com tags apropriadas
- Preencher Purchase Orders (POs)
- Preencher Schedule
- Atualizar planilha pessoal de acompanhamento

**Inputs:** Tag "Survey Received" (de Permits/Client Relations); draws financeiros (primeiro draw libera ate Robintec; segundo draw libera resto da fase 1); permit liberado (varia por condado)
**Outputs:** Servicos de fundacao completados; daily logs, POs e schedule atualizados no Builder Trend
**Observacoes:** Diferenca entre condados: Citrus exige permit para iniciar; Alachua permite avancar ate form sem permit. GARGALO CRITICO: Demora no calculo de loads por falta de equipamentos.

### Processo 2: Agendamento Fase 2 - Rough/Estrutura
- **Objetivo:** Gerenciar a fase de instalacoes brutas (rough plumbing, electric, AC), frame, isolamento e drywall -- fase NAO LINEAR que exige constante verificacao de pre-requisitos
- **Responsavel principal:** Joao Victor Serra / Thercyo Augusto Pereira
- **Frequencia:** Diaria
- **Ferramentas:** Builder Trend (daily logs, schedule, POs), WhatsApp (90%), Planilha pessoal (Google Sheets), Caderno fisico (Thercyo), E-mail (Termite/Protec)

**Passo a passo:**
1. Recebimento do 4o Draw libera para chamar drawin, 3 Rs e instalacao de porta/janela -- Responsavel: Joao Victor / Thercyo -- Ferramenta: Builder Trend (notificacao financeira)
2. Agendar **Rough Plumbing, Rough Electric, Rough AC** (tres roughs que precisam ser aprovados) -- Responsavel: Joao Victor / Thercyo -- Ferramenta: WhatsApp
3. Agendar **Drain** (precisa dos roughs feitos) -- Responsavel: Joao Victor / Thercyo -- Ferramenta: WhatsApp
4. Acompanhar **Left Inspection** - aprovada, segue para estanque -- Responsavel: Joao Victor / Thercyo -- Ferramenta: Builder Trend
5. Agendar **Shingles** (cobertura do telhado) -- Responsavel: Joao Victor / Thercyo -- Ferramenta: WhatsApp
6. Acompanhar **Frame Inspection** (inspecao mais importante da fase) - requer todos os roughs aprovados + drain + portas e janelas instaladas -- Responsavel: Joao Victor / Thercyo -- Ferramenta: Builder Trend
7. Agendar **Termite** (tratamento contra cupins) - DEVE ser feito ANTES do insulation (senao custa o dobro) -- Responsavel: Joao Victor / Thercyo -- Ferramenta: E-mail (Protec)
8. Agendar **Insulation** (isolamento termico) apos frame aprovado -- Responsavel: Joao Victor / Thercyo -- Ferramenta: WhatsApp
9. Acompanhar **Insulation Inspection** - requer insulation + shingles feitos -- Responsavel: Joao Victor / Thercyo -- Ferramenta: Builder Trend
10. Solicitar material de **Drywall** com antecedencia ao sub apos aprovacao do frame -- Responsavel: Joao Victor / Thercyo -- Ferramenta: WhatsApp

**Sistema de listas com subs (WhatsApp):**
- Isaias (strap, WF assembly, frame windows): lista de servicos -- 3 fases solicitando
- Alliance e MLI: listas de servicos que funcionam bem
- Demais subs: solicitacao direta individual

**Inputs:** 4o Draw liberado (Financeiro); roughs aprovados (Inspecao); materiais disponiveis (Compras/Warehouse)
**Outputs:** Estrutura da casa completada; inspecoes aprovadas; casa pronta para Fase 3
**Observacoes:** Fase NAO LINEAR -- constante necessidade de verificar servicos anteriores, ir e voltar. Isaias nao atualiza a lista de servicos, causando esquecimentos.

### Processo 3: Agendamento Fase 3 - Finish/Acabamento
- **Objetivo:** Gerenciar a fase final de acabamento (pisos, pintura, cabinets, fixtures, etc.) ate a casa estar pronta para inspecao final e entrega
- **Responsavel principal:** Daniela Santiago / Antonio Santos / Guilherme Barbosa
- **Frequencia:** Diaria
- **Ferramentas:** Builder Trend (daily logs, schedule, POs), WhatsApp, Google Sheets (planilha pessoal), Dashboard de Construction Data, Slack (Slack Bots para notificacoes)

**Passo a passo:**
1. Verificar andamento de cada casa (nao conseguem todas diariamente pelo volume) -- Responsavel: Daniela / Antonio / Guilherme -- Ferramenta: Dashboard de Construction Data
2. Avaliar prioridades usando dashboard (tempo total em progresso) -- Responsavel: Daniela -- Ferramenta: Dashboard de Construction Data
3. Comunicar-se internamente na equipe para priorizar casas -- Responsavel: Equipe Fase 3 -- Ferramenta: Slack
4. Para cada servico a agendar:
   - Copiar informacoes da casa (modelo, endereco, parcel ID, pin drop) da planilha pessoal -- Responsavel: Scheduler -- Ferramenta: Google Sheets
   - Digitar informacoes no titulo da PO (sem campos padronizados) -- Responsavel: Scheduler -- Ferramenta: Builder Trend
   - Enviar para sub via WhatsApp com template padronizado -- Responsavel: Scheduler -- Ferramenta: WhatsApp
   - Preencher daily log + schedule + PO (informacoes repetidas 3x) -- Responsavel: Scheduler -- Ferramenta: Builder Trend
5. Verificar customizacoes no Card fixo do Builder Trend (stone veneer, paleta diferente, pavers) -- Responsavel: Scheduler -- Ferramenta: Builder Trend
6. Adaptar fluxo conforme necessidade (fase NAO linear, servicos nao-dependentes podem ser feitos simultaneamente) -- Responsavel: Daniela -- Ferramenta: [decisao operacional]

**Inputs:** Casa com Fase 2 completa; informacoes de customizacao (Client Relations); draws liberados; materiais disponiveis (Compras/Warehouse)
**Outputs:** Casa completamente acabada; pronta para inspecao final e entrega
**Observacoes:** Fase 3 NAO e linear -- exige analise critica e flexibilidade. Consideram impacto humano (custos de diarias extras para subs). Mudancas de material de ultima hora causam reagendamento.

### Processo 4: Validacao de Servico (Checklist Done)
- **Objetivo:** Confirmar conclusao de servicos pelos monitores/supervisores, acionando gatilho de pagamento ao subcontratado
- **Responsavel principal:** Monitores / Supervisores
- **Frequencia:** Continua (por servico concluido)
- **Ferramentas:** Builder Trend (checklist), Slack

**Passo a passo:**
1. Monitor/supervisor visita a obra e verifica servico concluido -- Responsavel: Monitor/Supervisor -- Ferramenta: Visita presencial
2. Preencher checklist de verificacao no Builder Trend -- Responsavel: Monitor/Supervisor -- Ferramenta: Builder Trend
3. Marcar como "checklist done" -- Responsavel: Monitor/Supervisor -- Ferramenta: Builder Trend
4. Sistema notifica Financeiro para liberar pagamento ao sub -- Responsavel: [automatico] -- Ferramenta: Builder Trend

**Inputs:** Servico executado pelo sub; visita de verificacao
**Outputs:** Confirmacao de servico (gatilho de pagamento)
**Observacoes:** ALERTA CRITICO: Checklist done = gatilho de pagamento. Monitor deve ser criterioso antes de marcar. Sub pago nao volta para arrumar -- problema vira custo para Lakeshore. Novos monitores precisam ser treinados sobre esse impacto.

### Processo 5: Separacao Order vs Schedule (Pedido de Material vs Agendamento de Servico)
- **Objetivo:** Distinguir claramente entre solicitacao de material (order) e agendamento de servico (schedule), evitando confusao no fluxo
- **Responsavel principal:** Equipe de Scheduling (todas as fases)
- **Frequencia:** Por servico
- **Ferramentas:** Builder Trend (tags), WhatsApp, E-mail

**Passo a passo:**
1. **Order** (tag): Criar solicitacao de material (ex: blocos para masonry) -- Responsavel: Scheduler -- Ferramenta: Builder Trend
2. Enviar e-mail/WhatsApp ao fornecedor com pedido -- Responsavel: Scheduler -- Ferramenta: E-mail, WhatsApp
3. Registrar "Delivered" quando material chega -- Responsavel: Scheduler -- Ferramenta: Builder Trend
4. **Schedule** (tag): Agendar servico de assembly com subcontratado -- Responsavel: Scheduler -- Ferramenta: WhatsApp
5. Registrar opcoes de status: schedule, reschedule, rework schedule, rework reschedule -- Responsavel: Scheduler -- Ferramenta: Builder Trend

**Inputs:** Necessidade de material ou servico identificada no cronograma
**Outputs:** Material pedido e entregue; servico agendado e executado
**Observacoes:** Separacao clara entre essas etapas e essencial para evitar confusao. Software em desenvolvimento deve separar claramente essas funcoes.

## Dores e Problemas Conhecidos
- **Informacao repetida 3x (Top 1)**: Daily logs + Schedule + PO com mesmos dados -- todos os schedulers reclamam
- **Builder Trend lento**: Carregamento pesado, recarregamento de pagina apos cada input
- **Tags excessivas e confusas**: Muitas tags, algumas duplicadas entre fases
- **Slack instavel e lento**: Equipe recorre ao WhatsApp por ser mais leve
- **Demora no calculo de loads**: Falta de equipamentos especificos, paralisa processos subsequentes
- **Survey Received ausente**: Se a tag nao for colocada, equipe nao sabe que nova casa existe
- **Comunicacao com subs**: Demora nas respostas e descumprimento de prazos; subs com letramento limitado
- **Falta de campos padronizados na PO**: Titulo digitado livremente (inconsistencia)
- **Modelo da casa dificil de acessar**: Precisa navegar por varias pastas no Builder Trend
- **Informacao descentralizada**: Cada pessoa cria sua propria planilha pessoal
- **Falta de notificacao de checklist done**: Precisa buscar manualmente
- **Takeoff desatualizado para novos modelos**: Dependem de atualizacao do departamento de takeoff
- **Mudancas de material de ultima hora**: Notificados muito tarde, exigem reagendamento
- **Dependencia de draws financeiros**: Primeiro draw limita ate Robintec; segundo draw libera resto

## Dependencias
- **Recebe de:** Supervisores/Monitores -> confirmacao de elevacao, calculo de loads, verificacao de servicos; Financeiro -> draws (liberacao financeira); Permits -> liberacao para inicio de construcao; Budget/Takeoff -> informacoes de materiais e quantidades; Compras/Warehouse -> materiais disponiveis; Client Relations -> informacoes de customizacao
- **Entrega para:** Financeiro -> confirmacao de servico realizado (checklist done) para liberar pagamento; Supervisao -> informacoes de agendamento para acompanhamento; Inspecao -> servicos concluidos para agendamento de inspecoes; Compras -> pedidos de material

---

## Documentacao Formal (Fonte: Drive QPS)

### Reestruturacao de Fases

**Documento:** Plano de Acao para Mudanca de Regra de Negocio - Escopo de Fase de Obra
**Elaborado por:** Ana Maria M Gouveia
**Responsaveis aprovadores:** Bernardo Lira (President), Leonardo Lira (VP)

**Situacao anterior (5 fases):**
- Fase 1, Fase 2, Fase 3.1, Fase 3.2 e Fase 4
- Fases 3.1, 3.2 e 4 eram as mais criticas
- Geravam sobreposicao operacional e ambiguidade de responsabilidade entre 3.2 e 4

**Nova estrutura (4 fases):**
- Fase 1, Fase 2, Fase 3 e Fase 4
- **Fase 3 (nova):** equivale a antiga Fase 3.1 — inicia no Drywall Checklist Done e termina no CO Issued
- **Fase 4 (nova):** unifica antigas Fases 3.2 e 4 — inicia no CO Issued e termina no Phase 4 Checklist Done

**Redistribuicao de responsabilidades dos supervisores:**
- Supervisor da antiga Fase 3.2 passa a ser responsavel integral pela nova Fase 4 (acompanhamento continuo do inicio ao fim)
- Supervisor da antiga Fase 4 passa a atuar exclusivamente como agente de walkthrough e supervisor de garantias (acionado apenas quando walkthrough for agendado ou em caso de garantia)

**Novo processo formal de analise de reparos do walkthrough:**
- Responsabilidade: equipe de Closing (Gestora: Debora)
- Passos:
  - Analisar relatorio de walkthrough
  - Aprovar reparos compativeis com o produto padrao
  - Identificar solicitacoes fora do escopo
  - Gerar relatorio formal
  - Enviar comunicacao ao cliente
  - Registrar a decisao no sistema

**Metas da reestruturacao:**
- Eliminar sobreposicao entre fases: reduzir de 2 para 1 fase ativa apos CO (Responsaveis: Sam - Construction Manager; Moises - PM; Ana - QPS Manager)
- Reduzir retrabalho pos-walkthrough (Responsaveis: Sam; Moises)
- Reduzir em 50% custos fora do escopo de reparo pos-walkthrough (Responsavel: Debora - Closing Manager)

**Plano de acao e prazos:**
- **Jan 12, 2026** — Redefinir estrutura das fases nos sistemas da empresa (Gestor: Evandro / IT)
- **Jan 12, 2026** — Desenvolver IT's dos processos por departamento (Gestora: Ana Maria / QPS)
- **Jan 12, 2026** — Desenvolver dicionario de qualidade para casas spec (Gestora: Ana Maria / QPS)
- **Jan 12, 2026** — Desenvolver modelo de relatorio de reparos de walkthrough (Gestoras: Ana Maria / Debora)
- **Jan 14, 2026** — Atualizar escopo e responsabilidades dos supervisores (Gestores: Samuel / Moises / Construction)
- **Jan 14, 2026** — Notificar todas as equipes envolvidas (Gestores: Ana Maria / Samuel / Moises / Debora / Fernanda)
- **Jan 16, 2026** — Treinar equipes para o novo procedimento de analise de reparos do walkthrough (Departamentos: QPS / Construction / Scheduling / Closing / Client Relations)

---

### Guia de Tags para Daily Logs

**Referencia formal:** Todo input de Daily Log deve conter obrigatoriamente um **Processo** e um **Status**.

**Tags de Permit (#P-):**

| Processo | Status | Quando usar |
|---|---|---|
| #P - SURVEY | DOCUMENT REQUESTED | Ao solicitar o processo |
| #P - SURVEY | CHECKLIST DONE | Ao concluir o processo, recebendo o Site Plan |
| #P - APP FORM & NOC | CHECKLIST DONE | Ao concluir o processo |
| #P - TRUSSES | DOCUMENT REQUESTED | Ao solicitar a documentacao |
| #P - TRUSSES | CHECKLIST DONE | Ao receber a documentacao |
| #P - TREE SURVEY | DOCUMENT REQUESTED | Ao solicitar a documentacao |
| #P - TREE SURVEY | CHECKLIST DONE | Ao receber a documentacao |
| #P - ENERGY CALC | DOCUMENT REQUESTED | Ao solicitar a documentacao |
| #P - ENERGY CALC | CHECKLIST DONE | Ao receber a documentacao |
| #P - FLOOR PLAN | DOCUMENT REQUESTED | Ao solicitar a documentacao |
| #P - FLOOR PLAN | CHECKLIST DONE | Ao receber a documentacao |
| #P - SEPTIC | DOCUMENT REQUESTED | Ao solicitar o processo |
| #P - SEPTIC | CHECKLIST DONE | Ao concluir o processo |
| #P - PERMIT | APPLIED | Ao realizar a aplicacao do permit no county |
| #P - PERMIT | ISSUED | Ao receber o permit |
| #P - PERMIT | REPORT | Ao sinalizar informacoes pontuais |
| #P - PERMIT | CANCELED | Quando um permit for cancelado |
| #P - REVISION | REWORK | Quando houver Reject — ao solicitar ajuste do processo/documentacao |
| #P - REVISION | CHECKLIST DONE | Ao receber a documentacao correta e enviar ao county |
| #P - PERMIT HOLD | REWORK | Ao receber solicitacao de modificacao de documentacao apos Permit Issued (ex: Survey, Floor Plan, Septic) |
| #P - PERMIT HOLD | CHECKLIST DONE | Apos envio e aprovacao da documentacao corrigida pelo County |
| #P - PERMIT HOLD | REPORT | Ao receber requisicao de modificacao vinda do cliente apos Permit Issued (ex: mudanca de modelo) |
| #P - PERMIT HOLD | CHECKLIST DONE | Apos envio e aprovacao de toda documentacao corrigida pelo County |

**Tags de Finance:** (a definir — campos em branco no documento fonte)

**Tags de Field:** (a definir — campos em branco no documento fonte)

**Correcao de inputs atrasados:**
- A data adicionada ao banco de dados sera sempre a data de criacao do Daily Log, independente da data informada no input
- Procedimento: inserir a nota com a informacao "Input atrasado" e informar a data correta para que seja modificada diretamente no banco de dados

---

### Dados QPS (Referencia: agosto 2024)

**Documento:** QPS - Processos e Sistematizacao (19/08/2024)
**Contexto:** Reuniao de priorizacao de melhorias sistemicas envolvendo Construction, Scheduling, Financeiro e automacoes

**Prioridades identificadas com impacto direto em Scheduling:**

- **Controle de Producao (Prioridade 1):**
  - Meta: ferramenta de acompanhamento de field, office e diretoria com roteirizacao de Daily Loggers implementada
  - Pendencia: organizar padrao de inputs para fase 5 (Ana e Evandro)
  - Pendencia: monitorar e registrar utilizacao de inputs com tags REWORK e REQUEST (Horst - prazo 31/07/2024)
  - Pendencia: monitoracao das tags REWORK SCHEDULED / REPORT pelo subs team (Horst e Evandro)
  - Pendencia: desenvolver sistema inicial de planejado x realizado (Evandro - prazo 23/08/2024)
  - Pendencia: desenvolver sistema acelerador de reuniao de planejamento (Evandro - prazo 23/08/2024)
  - Pendencia: revisar todas as tags e banco de dados relacionados aos sistemas C1-C2 (Evandro, Ale, Horst, Wallyson, Don, Diego e Caio - prazo 23/08/2024)

- **Monitoramento de Tempo de Construcao (Prioridade 1):**
  - Meta: base de dados com tempo medio por fase e reducao dos tempos
  - Pendencia: analise de outliers e dispersao (Ale)
  - Pendencia: validar delimitadores de fase existentes (Ana)
  - Pendencia: definir processo de entrega da casa nas fases 4 e 5 (Ana)
  - Pendencia: verificar quais inputs tem maior percentual de falta (Ale e Horst)

- **Automacao de Relatorio de Schedule Desatualizado:**
  - Objetivo: identificar casas com schedule items nao completed via tags do Daily Log
  - Pendencia: identificar divergencias pelas tags do DL (Horst e Diego)
  - Pendencia: criar proposta de procedimento para novas tags e schedule items (Evandro, Horst e Diego)
  - Status em 19/08: 2 de 8 relatorios completados

- **Cronoanálise CPM:**
  - Iniciar cronoanalise com Valdir (Horst - adiado em 22/08/2024)
  - Escrever relatorio sobre resultados do mapeamento (Horst - prazo 23/08/2024)

- **Planejamento por Celula (C1-C6):**
  - Planejamento C1 e C2: ajustar budgets dos templates por modelo/county (Wallyson e Caio - 60% concluido em 19/08)
  - Planejamento C2: estruturar avaliacao de subs (adiado)
  - Planejamento C3, C4, C5 e C6: reorganizar e atualizar planejamentos de TH Clemson e Eustis (Caio)

- **Mapeamento e Quantificacao de Problemas (FMEA - Caio):**
  - Fluxograma inicial de inputs de problemas via daily logs proposto (Caio e Horst)
  - Reuniao agendada para 19/08 para desenhar proposta do fluxo basico do FMEA

---

## Dados Operacionais (Fonte: Drive Lakeshore)

### Divisao de Responsabilidades: Purchasing vs Scheduling

O Purchasing interno e dividido entre tres pessoas com escopo definido:

**Amanda** — responsavel por subcontratados de servico (subs com contrato):
- Clearing lot, Slab, Underground Plumbing, Underground Electric, Masonry Assembly, Layout for Trusses, Lintel Pouring, Roof Assembly, Roofing, Rough Electric, Lath and Stucco, Polyseal and Insulation, Drywall, Paint, Tile e Vinyl, Soffit, Garage Door, Blow-in, HVAC, Cabinets, Driveway, Trim Set, Appliances, Final Grade, SOD, Final Clean, Contratos com os subs
- Sequencia de status por atividade: Buscando Contato -> Orcando -> PO -> Assinar Contrato -> Schedule -> Follow-up -> Invoices

**Ellen** — responsavel por materiais e itens especificos:
- Windows and Exterior Doors, Interior Doors, Instalar e levar Dumpster (manutencao), Instalar e levar Portable (manutencao), Trim Set, Termite, Framing and Trusses (compra de todo o material), Flooring

**Ana** — responsavel por materiais de obras civis e kits:
- Slab (compra do concreto), Blocks (compra de tudo incluso no Masonry Assembly), Driveway (compra de malha e concreto, eventualmente loads extras), Kits do banheiro, Door Knob, Door Stop, Appliances

**Orcamentos:** quando necessario buscar novos fornecedores, as tres fazem forca-tarefa para agilizar o processo. Meta futura: planilha de fornecedores com precos unitarios por obra.

---

### Estrutura do Cronograma de Construcao

O cronograma de construcao acompanha cada casa individualmente com colunas para cada etapa da obra. As etapas seguem a ordem de execucao do canteiro:

**Fase Pre-Construcao / Fundacao:**
Stake Lot -> Clear Lot -> Stake House -> Loads and Pad -> Compact Test -> Hub and Tack -> Form -> Foundation Material -> UG Plumbing -> Slab Prep -> Electric UG -> Slab Pouring

**Fase Estrutura:**
Blocks and Precast -> Masonry Assembly -> Lintel Pouring -> Trusses and Lumber -> Roof Assembly -> Framing -> TUG Install -> Windows Install -> Polyseal -> Dry In -> Rough Plumbing -> Septic -> Termite Treatment -> Goose Neck -> Rough AC -> Rough Electric -> Shingles -> Lath -> Stucco -> Texture -> Insulation -> Drywall

**Fase Acabamento:**
Exterior Paint -> Soffit -> Driveway Cut -> Interior Paint -> Blow-in Insulation -> Trim Set -> Driveway Prep -> Garage Door -> Tiles and Vinyl (Tiles Install / Vinyl Install) -> Driveway Pouring -> AC Trim -> Grout -> Cabinets -> Blower Door Test -> Granite -> Site Drainage -> Plumbing Trim -> Trim Set Install -> Dishwasher Install -> Electric Trim -> SOD (SOD Install) -> Final Paint -> Hot Check -> Turn On AC

Cada coluna de etapa registra: empresa/sub responsavel, datas de order e delivery, datas de schedule e checklist done, e notas especificas da casa.

Campos de controle por casa: numero da casa, endereco, county (MARION, CITRUS, etc.), notas gerais, flags WM (Warranty Manager) e EM (Escrow Manager), e DL (Daily Log atualizado).

---

### Estrutura do Controle MEP

O controle MEP (Mechanical, Electrical, Plumbing) rastreia invoices e change orders por subcontratado, casa e tipo de servico. Campos principais:

- **Identificador da casa:** codigo de referencia (ex: C1-0445-ND0M2) + numero do lote/permit
- **Sub:** empresa executora (ex: Eco One Plumbing Services, Eco One Electrical Services)
- **Valor:** valor da invoice ou change order
- **Numero da Invoice:** referencia fiscal
- **Descricao do servico:** o que foi realizado (ex: Broken Pipe Repair, Kitchen Disconnect, Change Order: Connect Meter)
- **Situacao:** OK (aprovado para pagamento) ou NEGADO (rejeitado com justificativa)
- **Data da Invoice:** data de emissao

Situacoes comuns registradas: trip charges ($90 padrao), broken pipe repair, change orders, fill up for inspection, kitchen disconnect and connect. Justificativas de negacao ficam registradas na linha abaixo do item.

---

## Operational Detail (from Interviews)

### 8-Step Clear Lot Process

The Clear Lot process follows a strict 8-step dependency chain. Each step depends on the successful completion of the previous one. Weather can delay any step in the sequence.

1. **Survey** -- Topographic survey of the lot (prerequisite for everything else)
2. **Clear Lot** -- Physical clearing of vegetation and debris from the lot
3. **Stake** -- Stake the house position on the lot (depends on Survey completion)
4. **Load Calc** -- Supervisors calculate structural loads (depends on engineering review + Stake completion). CRITICAL BOTTLENECK: lack of specialized equipment causes delays
5. **Pad** -- Grade and prepare the building pad (depends on Clear Lot + Stake + Load Calc delivery)
6. **Compact** -- Compaction test of the pad soil (depends on Pad completion). Can fail and delay the entire schedule
7. **Robintec** -- Robintec survey/verification (ordered simultaneously with Compact Test for scheduling efficiency)
8. **Form** -- Foundation formwork (depends on Compact Test passing + Robintec completion). Cannot advance without confirmed compact test result

#### Dependency Chain Summary

Survey -> Clear Lot -> Stake -> Load Calc -> Pad -> Compact -> Robintec -> Form

If any step fails (especially Compact Test), the entire downstream schedule shifts.

### Draw Gating Logic

Financial draws act as gates that control which construction phases can begin. The draw structure determines the maximum scope of work allowed at each stage:

- **Draw 1**: Covers site work through Robintec forms (foundation preparation). Typically 15-20% of contract value. Limits work to: Survey, Clear Lot, Stake, Load Calc, Pad, Compact, Robintec, Form.
- **Draw 2**: Unlocks Phase 1 work -- block, rough plumbing, rough electrical, underground utilities. Typically 25-30% of contract value. Cannot start block or rough trades until Draw 2 is released.
- **Draw 3**: Unlocks Phase 2 work -- drywall, paint, trim, cabinets, flooring. Typically 30-35% of contract value. Finishing trades cannot be scheduled until Draw 3 clears.
- **Draw 4**: Final draw -- landscaping, final cleanup, final inspections, Certificate of Occupancy (CO). Typically 15-20% of contract value. Covers all remaining work to house completion.

**Critical rule**: Scheduling CANNOT advance work beyond what the current draw covers. If a draw is delayed by the lender or client, the entire construction schedule stalls at that gate.

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- [Catalogo de Dores](07_CATALOGO_DORES.md)
- [Fluxo Spec Home](05_FLUXO_SPEC_HOME.md)
- [Fluxo Custom Home](06_FLUXO_CUSTOM_HOME.md)
- [Glossario de Termos](03_GLOSSARIO.md)
- **Departamentos relacionados:**
  - [Supervisao](dept_supervisao.md) — confirma elevacao, calcula loads, verifica servicos
  - [Financeiro](dept_financeiro.md) — libera draws (liberacao financeira)
  - [Permits](dept_permits.md) — libera para inicio de construcao
  - [Orcamento](dept_orcamento.md) — fornece informacoes de materiais e quantidades
  - [Compras](dept_compras.md) — confirma materiais disponiveis no armazem
  - [Inspecao](dept_inspecao.md) — recebe servicos concluidos para agendamento de inspecoes
  - [Client Relations](dept_client_relations.md) — fornece informacoes de customizacao

## CPM Construction Sequence Reference

The CPM (Critical Path Method) flowchart defines the complete construction sequence used by Lakeshore. Scheduling must follow this sequence for all task ordering and dependency management.

**Pre-Scheduling Concept:** When a predecessor task receives "checklist done", Scheduling must:
1. **Schedule** the immediate successor (exact date)
2. **Pre-schedule** the next successor (estimate only -- "put it on the sub's radar")
3. Status lifecycle: `pre-scheduled -> scheduled -> checklist done`

**Phase Gating:** Each phase has strict prerequisites:
- FASE 1 (Site Prep): Permit Issued required in Citrus before starting; not in Marion
- FASE 2 (Foundation): Form cannot start without Compact Test passing
- FASE 3 (Framing): Framing Inspection requires ALL Rough inspections + Dry In approved
- FASE 4 (Finish): Cabinets/Granite require Tile + Vinyl completion; Building Final requires 7 prerequisites

**County Differences (Marion vs Citrus):** Affect inspection types, driveway inspections, and Pre-Power requirements. See [cpm_construction_sequence.md](cpm_construction_sequence.md) for full table.

**Process Types:** scheduling (blue), material (green), lakeshore services (orange), inspection (red), request (yellow) -- each has different status inputs and outputs.

**Full reference:** [cpm_construction_sequence.md](cpm_construction_sequence.md) | [cpm_subsystems.md](cpm_subsystems.md)

---

## Key Glossary Terms

> Terms from [Glossario de Termos](03_GLOSSARIO.md) most relevant to the Scheduling department. (10 terms -- file near size limit)

- **Draw / Draw Request** / **Saque/Parcela de Pagamento**: Construction financing payment tied to progress milestones -- triggers scheduling phases
- **Clear Lot** / **Limpeza do Terreno**: First construction activity after Survey Received -- removal of vegetation and initial leveling
- **Compact Test** / **Teste de Compactacao**: Soil compaction test before foundation concrete -- can fail and delay subsequent phases
- **Rough (Plumbing/Electric/AC)** / **Instalacao Bruta**: Pre-finish installation of plumbing, electrical, or AC within walls -- three inspections needed
- **Sub / Subcontractor** / **Subcontratado**: Third-party service provider for specific construction phases -- scheduled via WhatsApp
- **Punch List** / **Lista de Pendencias**: Items needing correction before house delivery -- identified during final walkthrough
- **Survey Received** / **Levantamento Recebido**: Daily log tag indicating survey received -- TRIGGER for scheduling to begin on a new house
- **Hold** / **Retencao/Paralisacao**: Restriction preventing a project phase from advancing (financial, technical, or regulatory)
- **Checklist Done** / **Checklist Concluido**: Confirmation that supervisor completed verification -- PAYMENT TRIGGER for subcontractor
- **Drywall** / **Gesso Acartonado**: Interior wall/ceiling covering installed after frame and insulation -- material requested from sub in advance

---

## BuilderTrend Job 455 -- Real Data (Supplement)

### Job 455 Schedule Structure
- **50 schedule items** tracked in BT covering Dec 2024 - Mar 2025 (first 3 months)
- Remaining 6 months tracked via **396 Daily Logs** (Roughs through Close-out)
- **53 To-Do Checklists** aligned with construction phases

### Schedule by Phase on Job 455
**Land Preparation (Dec 30, 2024 - Mar 7, 2025)**:
Stake Lot -> Clear Lot -> Silt Fence -> Stake House -> Water Meter -> Docbox -> Loads -> Pad -> Compact Test -> Hub and Tack -> Form -> Underground Plumbing -> Underground Electrical -> UP Inspection -> Foundation Material -> Slab Prep -> Slab Inspection -> Slab Pouring

**Masonry and Roofing (Mar 11 - Mar 24, 2025)**:
Blocks -> Precast -> Masonry Assembly -> Lintel Inspection -> Mark Straps -> Lintel Pouring -> Lumber -> Trusses -> Framing

**Roughs through Final (Daily Logs only)**:
Windows -> Plumbing/AC/Electric Rough -> Lath -> Stucco -> Insulation -> Drywall -> Paint -> Tile -> Vinyl -> Cabinets -> Trim -> Final Grade -> Final Clean -> Walkthrough -> CO

### Checklist Assignments (Supervisor Handoffs)
| Phase | Assigned To | Checklists |
|-------|------------|------------|
| Pre-Construction | Iara Oliveira | Builder's Fee Bill |
| Land Prep through Roughs | Francisco Castillo / Eddye Pereira | 28 checklists |
| Finishing through Final | Jaaziel Santos | 22 checklists |

### Draw Schedule Alignment
| Draw | Scheduling Milestone | Date |
|------|---------------------|------|
| 1st | Contract sign | Dec 23, 2024 |
| 2nd | Slab complete | Feb 19, 2025 |
| 3rd | Roof complete | Mar 10-14, 2025 |
| 4th | Insulation complete | Mar 14-19, 2025 |

## CPM Construction Sequence -- Scheduling Deep Dive

### Pre-Scheduling Concept (CPM Core Innovation)
The CPM introduces "pre-scheduling" as a critical scheduling technique:
1. **Predecessor receives "checklist done"** -> Scheduling performs "schedule" of immediate successor AND "pre-schedule" of next successor
2. **Pre-schedule**: Anticipated advance scheduling; orients subcontractor they will be called within days
3. **Status lifecycle**: pre-scheduled -> scheduled -> checklist done
4. **Rule**: "Scheduled" requires exact date; "pre-scheduled" requires only estimate or no date

### Process Types (Color-Coded in CPM)
| Type | Color | Example | Scheduling Action |
|------|-------|---------|-------------------|
| Scheduling | Blue | Clear Lot, Slab Pouring | Schedule sub with date |
| Material | Green | Foundation Material, Tile | Order with ETA |
| Lakeshore Services | Orange | Quality Control 1, 2 | Schedule internal LS services |
| Inspection | Red | UP Inspection, Framing | Schedule with county |
| Request | Yellow | Precast Delivery, Trusses Mfg | Manufacturing/delivery request |

### Complete CPM Task Sequence (66 Activities)
**FASE 1**: Doc Box -> Portable -> Survey -> Stake Lot -> Clear Lot -> Silt Fence -> Stake House -> Loads -> Pad -> Compact Test -> Hub and Tack -> Wood Dumpster
**FASE 2**: Form -> Underground Plumbing -> Underground Electrical -> UP Inspection -> Foundation Material -> Slab Prep -> Slab Inspection -> Slab Pouring -> Blocks -> Precast -> Masonry Assembly -> Lintel Inspection -> Lintel Pouring
**FASE 3**: Lumber -> Trusses -> Framing + Roof Assembly -> Mark Straps -> Inspections -> TUG Install/Inspection -> Termite Treatment -> Septic -> Windows/Doors -> Dry In -> Rough Plumbing/AC/Electric -> Lath -> Stucco -> Insulation -> Drywall
**FASE 4**: Paint -> Tile/Vinyl -> Soffit -> Garage Door -> Cabinets/Granite -> Trim Set -> Plumbing/Electric/AC Trim -> Driveway -> Final inspections -> Final Grade -> SOD -> Garden -> Final Clean -> FCC -> Walkthrough -> CO

### 29 Operational Notes for Scheduling
Key scheduling constraints from CPM:
- Blocks must arrive 2 days after slab pouring (cure time)
- Trusses ETA = Foundation Material ETA + 2 weeks; never Monday delivery
- Underground Electrical with Slab Prep but NEVER after
- Framing Inspection same day as Rough inspections when possible
- Interior + Exterior Paint by same sub, 2 days after Drywall
- Trim Set Material must arrive during Cabinets/Granite phase
- House Number 2 days after Exterior Paint + after Soffit
- Garage Door + Electronic Locker before Trim Set (theft protection)
- Quality Control 1 with Final Touches (FIRST day); QC2 (LAST day)
- Building Final requires all final inspections + Blown Insulation + Blower Door Test + Appliances

## Const App Integration (Supplement)

### Project Management Module
- **Active Projects**: Track all projects and task progress (On Track, Has Blocked, Delayed)
- **Blocked Tasks**: Identify and resolve blocked tasks across projects

### Construction Module
- **156 executable services** in the service catalog covering all trades
- **Service types**: Construction (labor/material), Inspection, Planning, Licensing, Utility, Concrete

### Inspection Requests Matrix
Projects tracked across 17 construction categories with inspection status legend:
- C=Not configured, -=Waiting, !=Pending, S/15=Scheduled, A=Today, P=Passed, 1=Failed once
