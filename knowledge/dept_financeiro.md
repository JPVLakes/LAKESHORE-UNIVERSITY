# Financeiro (Contas a Pagar + Contas a Receber) - Lakeshore Development

## Visao Geral
- **Missao:** Gerenciar todos os fluxos financeiros da construcao: pagamento de fornecedores e subcontratados (contas a pagar), cobranca de draws dos clientes (contas a receber), fechamento contabil de casas e conciliacao bancaria
- **Lider:** Fernanda - Supervisora Financeira / Notaria (executa pagamentos no banco)
- **Equipe:**
  - Iara Oliveira (ioliveira@lakeshoredevelopmentfl.com) - Contas a Pagar
  - Rayff Gregorio Cunha (rcunha@lakeshoredevelopmentfl.com) - Contas a Pagar
  - Ebano Maia - Financeiro
  - Cinthia Araujo - Contas a Receber
  - Thabata Thaty Goncalves (Tabata) - Fechamento de casas
  - Rafaella Almeida - Financeiro
- **Departamentos relacionados:** Scheduling, Orcamento/Budget, Compras, Contratos (Bruna), Permits (Cacia), Utilities (Dandara), Field, C-Level (Leo, Samuel, Moises)

## Processos

### Processo 1: Contas a Pagar - Fluxo Principal
- **Objetivo:** Processar pagamentos a fornecedores e subcontratados de forma controlada, com verificacao de PO, comprovacao de servico e aprovacao gerencial
- **Responsavel principal:** Iara Oliveira / Rayff Gregorio Cunha
- **Frequencia:** Diaria (pagamentos processados todas as tardes)
- **Ferramentas:** Builder Trend, Quickbooks, Planilhas Excel, E-mail, Slack

**Passo a passo:**
1. Receber invoices por e-mail (endereco, servico, valor) -- Responsavel: Iara / Rayff -- Ferramenta: E-mail
2. Verificar PO correta no Builder Trend para o servico -- Responsavel: Iara / Rayff -- Ferramenta: Builder Trend
3. Se PO existe e valor coincide: criar "bill" no sistema -- Responsavel: Iara / Rayff -- Ferramenta: Builder Trend
4. Registrar a bill em planilha interna para controle de fechamento -- Responsavel: Iara / Rayff -- Ferramenta: Planilhas Excel
5. Confirmar que servico foi realizado (via sistema de checklist) -- Responsavel: Iara / Rayff -- Ferramenta: Builder Trend (checklist done do Scheduling)
6. Enviar "release" ao sub (documento para notarizacao) -- Responsavel: Iara / Rayff -- Ferramenta: E-mail
7. Sub leva release ao notario publico para reconhecimento -- Responsavel: Sub (externo) -- Ferramenta: Notario publico
8. Receber release notarizado (foto/PDF) -- Responsavel: Iara / Rayff -- Ferramenta: E-mail
9. Montar planilha de pagamento diaria -- Responsavel: Iara / Rayff -- Ferramenta: Planilhas Excel
10. Enviar para Fernanda para execucao do pagamento no banco -- Responsavel: Iara / Rayff -- Ferramenta: Planilhas Excel
11. Leo aprova pagamento (sem aprovacao, pagamento nao sai) -- Responsavel: Leo (C-Level) -- Ferramenta: [detalhes nao disponiveis nos documentos fonte]
12. Pagamentos processados diariamente a tarde -- Responsavel: Fernanda -- Ferramenta: Sistema bancario
13. Dia seguinte: dar baixa no Builder Trend e Quickbooks -- Responsavel: Iara / Rayff -- Ferramenta: Builder Trend, Quickbooks
14. Adicionar "classe" no Quickbooks (projeto: CMER + numero da casa) -- Responsavel: Iara / Rayff -- Ferramenta: Quickbooks
15. Conciliacao bancaria na aba "transactions" do Quickbooks -- Responsavel: Iara / Rayff -- Ferramenta: Quickbooks

**Inputs:** Invoices dos fornecedores (por e-mail); POs no Builder Trend; checklist done do Scheduling
**Outputs:** Pagamentos processados; registros em Builder Trend e Quickbooks; release notarizado arquivado
**Observacoes:** Excecoes ao release (nao precisam notarizacao): parte inicial de permits, servicos de arquitetas, materiais (lisa, portas, luminarias), servicos de sceptic e tanque.

### Processo 2: Tratamento de Reparos (Invoices sem PO)
- **Objetivo:** Processar pagamentos de reparos que chegam sem PO no Builder Trend
- **Responsavel principal:** Iara Oliveira / Rayff Cunha
- **Frequencia:** Sob demanda (recorrente)
- **Ferramentas:** Builder Trend, E-mail, Slack

**Passo a passo:**
1. Receber invoice de reparo sem PO correspondente no Builder Trend -- Responsavel: Iara / Rayff -- Ferramenta: E-mail
2. Identificar que supervisores solicitaram reparos sem criar PO -- Responsavel: Iara / Rayff -- Ferramenta: Builder Trend
3. Contatar Moises ou Samuel para autorizacao do valor cobrado -- Responsavel: Iara / Rayff -- Ferramenta: Slack, WhatsApp
4. Aguardar confirmacao (processo pode ser demorado) -- Responsavel: Moises / Samuel -- Ferramenta: Slack
5. Apos autorizacao, criar PO retroativa e processar pagamento -- Responsavel: Iara / Rayff -- Ferramenta: Builder Trend

**Inputs:** Invoice de reparo sem PO; autorizacao de gerencia
**Outputs:** PO criada retroativamente; pagamento processado
**Observacoes:** Reparos com valores fixos (ex: Eco Onean) sao mais diretos. Grande dor de cabeca da equipe pela falta de comprovacao de valor.

### Processo 3: Bills Artificiais (Fechamento de Casa)
- **Objetivo:** Evitar prejuizo no fechamento de casas quando invoices reais ainda nao chegaram
- **Responsavel principal:** Thabata / Iara
- **Frequencia:** Por casa (no fechamento)
- **Ferramentas:** Builder Trend, Planilhas Excel

**Passo a passo:**
1. Identificar que casa precisa fechar mas invoice real nao chegou -- Responsavel: Thabata -- Ferramenta: Builder Trend
2. Criar bill no Builder Trend sem invoice real, baseada em media de valor estimado -- Responsavel: Thabata -- Ferramenta: Builder Trend
3. Registrar como bill artificial para controle -- Responsavel: Thabata -- Ferramenta: Planilhas Excel
4. Quando invoice real chega, substituir a artificial -- Responsavel: Iara / Rayff -- Ferramenta: Builder Trend

**Inputs:** Budget estimado; historico de valores similares
**Outputs:** Bill artificial para fechamento; substituicao posterior pela real
**Observacoes:** Evita prejuizo para Lake Shore -- apos fechamento nao se pode mais cobrar o dono da casa.

### Processo 4: Gastos do Field (Cartoes de Compras Emergenciais)
- **Objetivo:** Registrar e alocar contabilmente compras emergenciais feitas pela equipe de campo com cartoes da empresa
- **Responsavel principal:** Iara Oliveira / Rayff Cunha
- **Frequencia:** Diaria
- **Ferramentas:** Slack, Planilhas Excel, Builder Trend

**Passo a passo:**
1. Equipe do Field faz compras emergenciais com cartoes da conta do Field -- Responsavel: Equipe de Campo -- Ferramenta: Cartao corporativo
2. Recibos enviados pelo Slack (canal dedicado) -- Responsavel: Equipe de Campo -- Ferramenta: Slack
3. Financeiro identifica material/servico do recibo -- Responsavel: Iara / Rayff -- Ferramenta: Slack, Planilhas Excel
4. Ratear entre casas quando necessario -- Responsavel: Iara / Rayff -- Ferramenta: Planilhas Excel
5. Registrar como "variances" quando nao identificado -- Responsavel: Iara / Rayff -- Ferramenta: Planilhas Excel

**Inputs:** Recibos do Field via Slack
**Outputs:** Alocacao contabil por casa; registro de variances
**Observacoes:** Muitas vezes informacao insuficiente nos recibos -- equipe precisa "adivinhar" a alocacao. Corecraft usava conta do Field (conta separada sendo criada).

### Processo 5: Contas a Receber - Fluxo de Draws
- **Objetivo:** Cobrar draws (parcelas de pagamento) dos clientes conforme progresso da obra, desde a assinatura do contrato ate a entrega
- **Responsavel principal:** Cinthia Araujo
- **Frequencia:** Por casa/projeto (acompanha progresso da obra)
- **Ferramentas:** Builder Trend, E-mail, WhatsApp, Slack

**Passo a passo:**
1. Contrato assinado -> Cacia (Permit) notifica Cinthia via Slack -- Responsavel: Cacia (Permits) -- Ferramenta: Slack
2. Cinthia verifica draws no Builder Trend vs contrato -- Responsavel: Cinthia Araujo -- Ferramenta: Builder Trend
3. Editar manualmente valores de draws quando acordos com cliente diferem -- Responsavel: Cinthia Araujo -- Ferramenta: Builder Trend
4. Enviar cobranca do draw ao cliente por e-mail -- Responsavel: Cinthia Araujo -- Ferramenta: E-mail
5. Acompanhar gatilhos de cobranca conforme progresso da obra (ex: permit recebido = segundo draw) -- Responsavel: Cinthia Araujo -- Ferramenta: Builder Trend
6. Aplicar "hold" manual quando pagamento nao chega -- Responsavel: Cinthia Araujo -- Ferramenta: Builder Trend
7. Para pagamentos parciais: processar manualmente (sistema atual nao suporta) -- Responsavel: Cinthia Araujo -- Ferramenta: Planilhas Excel

**Inputs:** Contrato assinado (de Permits/Contratos); progresso da obra (de Scheduling); valores de draws
**Outputs:** Cobranhas enviadas; pagamentos recebidos; registros de hold
**Observacoes:** Valores dos draws podem mudar por acordos com cliente. Pagamentos parciais sao necessarios mas nao suportados pelo sistema atual. WhatsApp tambem usado para cobrancas.

## Dores e Problemas Conhecidos
- **Alto volume de e-mails com invoices**: grande desafio diario
- **Invoices sem PO**: fluxo de trabalho repetitivo; grande dor de cabeca
- **Inclusao de classe no Quickbooks**: processo super demorado (86 bills em um dia = 2 horas); dois sistemas lentos
- **Falta de contratos com valores exatos**: 27+ modelos; precos mudam conforme volume; equipe nao sabe valor correto
- **Confirmacao de reparos demorada**: depende de Moises/Samuel responderem
- **Pagamentos de subs maiores (FOCO, ECOWAN)**: valores mudam conforme volume, sem contratos atualizados
- **Gastos do Field sem informacao clara**: recibos incompletos; "achismos"
- **Notificacoes do Builder Trend nao funcionam**: equipe de permits nao consegue avisar financeiro eficazmente
- **Mudancas contratuais nao comunicadas ao financeiro**: POs ficam desatualizadas
- **Falta de visualizacao do historico financeiro completo de uma casa**: necessario para fechamento
- **Pagamentos parciais nao suportados**: sistema atual nao permite registrar pagamento parcial de draw
- **Integracao BT-Quickbooks incompleta**: data de vencimento nao serve como criterio; processo manual

## Dependencias
- **Recebe de:** Scheduling -> confirmacao de servico realizado (checklist done) para liberar pagamento; Orcamento/Budget -> valores de referencia de POs e budgets; Compras -> registro de compras, rateio de materiais; Contratos (Bruna) -> atualizacoes contratuais de valores; Permits (Cacia) -> notificacao de contrato assinado, taxas de permit; Utilities (Dandara) -> contas de utilities para pagamento; Field -> recibos de compras emergenciais; C-Level (Leo, Samuel, Moises) -> aprovacoes de pagamento, confirmacao de valores
- **Entrega para:** Fornecedores/Subs -> pagamentos processados; C-Level -> relatorios financeiros (DRE, balanco, T99); Quickbooks -> registros contabeis e conciliacao

---

## Especificacao do Software (Fonte: Drive QPS)

### Modulo FINANCES: Estrutura Geral

O modulo FINANCES e subdividido em **Payments** e **Project Details**, ambos com visao geral (todos os counties) e visao individual por county.

### Payments: Permitting Fees, Subcontractors, Purchase

**Permitting Fees**: todas as taxas de permit sao vinculadas a um projeto especifico. Podem ser importadas do Activity Log ou adicionadas diretamente em FINANCES > PAYMENTS > PERMITTING FEES. Campos: county, projeto, fee, descricao, valor, status (PENDING -> PAID), documentos, contatos, links. Ao mudar para PAID, as informacoes sao enviadas automaticamente para FINANCES > PROJECT DETAILS > BILLS do projeto correspondente.

**Subcontractors**: lista todas as Service Orders importadas do PROJECT MANAGEMENT > ACTIVITY LOG. Ao ser adicionado em uma etapa do cronograma, o subcontractor e seus valores aparecem aqui automaticamente. Status: PENDING ou PAID. Fluxo: selecionar um ou mais subcontractors -> ver todos os servicos prestados no periodo (padrao: ultimos 7 dias) -> marcar como pagos em lote -> status atualiza automaticamente.

**Purchase**: lista todas as Purchase Orders com status PENDING, APPROVED, COMPLETED, PAID. Usuarios com permissao podem aprovar ordens PENDING diretamente nesta tela. Ao receber status DELIVERED no Activity Log, a ordem passa automaticamente para COMPLETED e reflete em FINANCES > PAYMENTS > PURCHASE. Visao por supplier: valor pendente agregado de todos os pedidos COMPLETED, com opcao de marcar como pagos em lote.

### Project Details: Budget, Bills, Payments

**Budget**: cadastra os custos totais estimados antes do inicio da construcao, alem dos custos ja projetados (Permit Fees, Purchase Orders e Service Orders em aberto). O estimate vinculado ao projeto e a base - seus valores ficam congelados para o projeto mesmo que os precos na base de dados mudem. Apresenta comparativo: custos estimados x custos projetados x custos reais. Base de referencia: JOB COSTING BUDGET do BuilderTrend.

**Bills**: registra todos os gastos reais apos o inicio da construcao. Importa automaticamente de: PROJECT MANAGEMENT > SERVICE ORDERS, PURCHASE > PURCHASE ORDERS, FINANCES > PAYMENTS > PERMITTING FEES, e qualquer outro modulo que gere gasto no projeto. Organizado pelas mesmas secoes do Budget para permitir comparacao direta estimado x real.

**Payments (Draws)**: lista os draws de cada projeto com status e valor. Importa o Schedule of Value de PROJECT MANAGEMENT > PROJECT INFO e o status de pagamento do ACTIVITY LOG (Finance Update). Draws iniciam com status PENDING; ao serem registrados como pagos no Activity Log (status PAID ou PARTLY PAID), atualizam automaticamente aqui. O sistema notifica o responsavel por gerar o pedido de pagamento na data de vencimento de cada parcela.

### Fluxo de Pagamento de Subcontratados

1. Subcontractor executa servico e e registrado no ACTIVITY LOG (Schedule Update ou Service Update)
2. Informacao flui automaticamente para FINANCES > PAYMENTS > SUBCONTRACTORS com status PENDING
3. Equipe financeira filtra por subcontractor e periodo, seleciona servicos a pagar
4. Marca como pagos em lote -> status atualiza para PAID em todas as telas vinculadas

### Fluxo de Bills a partir de POs e SOs

- PO com status COMPLETED -> entra automaticamente como custo projetado em FINANCES > PROJECT DETAILS > BUDGET e como bill em FINANCES > PROJECT DETAILS > BILLS
- SO aprovada e concluida -> mesmo fluxo via SERVICE ORDERS
- Permitting fee com status PAID -> entra como bill no projeto vinculado
- Resultado: Bills do projeto agregam todos os gastos reais de todas as origens em um unico lugar

### Gestao de Contratos Pre-Obra (Fonte: FRS Requisitos Funcionais)

Fluxo de contrato que antecede a criacao do projeto no sistema financeiro:

- **RF-001 - Registro de Lead**: cliente externo preenche formulario publico; lead salvo com status PENDING para revisao interna.
- **RF-002 - Qualificacao**: usuario interno revisa o lead, associa obrigatoriamente um Owner e um Contact (e opcionalmente Realtor e HOA); lead passa para status QUALIFIED.
- **RF-003 - Criacao do Projeto**: ao converter o lead para status CONVERTED, o sistema cria automaticamente uma instancia de projeto com `started=false`, visivel para todos os departamentos se prepararem. Apos pagamento do 1st Draw, o projeto e atualizado para `started=true`.
- **Status do contrato**: contrato enviado -> assinado -> invoice enviado -> 1st draw pago. Ao atingir status "Assinado", o sistema notifica automaticamente o responsavel pelo envio do invoice.
- **Regras de negocio**: valor do contrato deve ser superior a $10.000; data de assinatura nao pode ser futura; todos os contratos devem ter documento PDF assinado anexado; historico completo de alteracoes e mantido com data, usuario e detalhes.

---

## Draw Gating & Payment Logic (from Interviews)

### MAP vs ECOWAN Payment Splits

Two major MEP subcontractors have different payment split structures across draws:

- **MAP** = Marion County Assessment Program (impact fees). These are county-mandated fees split across draws, not paid upfront. The split varies by county and project type.
- **ECOWAN** = Utility connection fees (Eco One / ECOWAN services). These cover plumbing, electrical, and AC rough/trim work with payments split across construction phases.

Payment split by contractor:
- **FOCO**: 40% - 40% - 20% (across three payment milestones)
- **ECOWAN**: 40% - 30% - 30% (across three payment milestones)

### Draw Schedule Breakdown

The draw schedule controls cash flow for each house and gates construction progress:

- **Draw 1**: Covers site work through foundation forms. Typically **15-20%** of total contract value. Includes: survey, clear lot, stake, pad, compact, robintec, form, and related permit fees.
- **Draw 2**: Covers Phase 1 construction (block, rough plumbing, rough electrical, underground utilities). Typically **25-30%** of total contract value. Released after foundation is complete and verified.
- **Draw 3**: Covers Phase 2 construction (drywall, paint, trim, cabinets, flooring, fixtures). Typically **30-35%** of total contract value. Released after frame inspection passes and rough trades are complete.
- **Draw 4**: Final draw covering landscaping, final inspection, Certificate of Occupancy (CO), and cleanup. Typically **15-20%** of total contract value. Released after all final inspections pass.

### Draw-Related Financial Rules

- Draw values in BuilderTrend may differ from contract values when special client agreements exist -- Cinthia must manually adjust
- Partial payments are common but NOT supported by the current system -- requires manual tracking in spreadsheets
- If a draw payment is delayed by the lender or client, Financeiro applies a "hold" that blocks Scheduling from advancing construction past that draw's scope
- Bills created before invoice arrival ("artificial bills") use estimated values to prevent closing delays -- replaced when real invoice arrives

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- [Catalogo de Dores](07_CATALOGO_DORES.md)
- [Fluxo Spec Home](05_FLUXO_SPEC_HOME.md)
- [Fluxo Custom Home](06_FLUXO_CUSTOM_HOME.md)
- [Glossario de Termos](03_GLOSSARIO.md)
- **Departamentos relacionados:**
  - [Scheduling](dept_scheduling.md) — envia confirmacao de servico (checklist done) para liberar pagamento
  - [Orcamento](dept_orcamento.md) — fornece valores de referencia de POs e budgets
  - [Compras](dept_compras.md) — fornece registro de compras e rateio de materiais
  - [Permits](dept_permits.md) — notifica contrato assinado e taxas de permit
  - [Utilities](dept_utilities.md) — envia contas de utilities para pagamento
  - [Inspecao](dept_inspecao.md) — informa fees necessarias para pagamento

## Key Glossary Terms

> Terms from [Glossario de Termos](03_GLOSSARIO.md) most relevant to the Financeiro (Finance) department.

- **Draw / Draw Request** / **Saque/Parcela de Pagamento**: Construction financing payment tied to progress milestones -- triggers payment clusters
- **Invoice** / **Fatura/Cobranca**: Bill from vendor/sub for payment -- received by email, processed daily by finance team
- **Retainage** / **Retencao Contratual**: Percentage withheld from payment as guarantee until satisfactory service completion
- **Lien Waiver** / **Renuncia de Penhor**: Legal document where sub waives lien rights after payment -- requires notarization
- **AIA** / **Documentos Padrao AIA**: Standardized construction industry documents for contracts and processes
- **Bill (BI)** / **Registro Contabil**: Accounting record of committed expense in BuilderTrend, created after invoice validation
- **Cost-Plus** / **Custo Mais Margem**: Contract type where client pays actual cost plus agreed markup
- **Backcharge** / **Cobranca Retroativa**: Charge to subcontractor for work that needed to be redone due to their error
- **CCO (Centro de Custos)** / **Centro de Custos**: Cost center identification for accounting classification by project
- **DRE** / **Demonstrativo de Resultado**: Financial report showing revenue, costs, and profit per project or period
- **Impact Fee** / **Taxa de Impacto**: County fee for infrastructure impact of new construction -- blocks Final Electric in Marion
- **Change Order** / **Ordem de Alteracao**: Formal scope/cost/schedule modification after contract -- impacts budget
- **Release** / **Documento de Quitacao**: Document sent to sub for notarization before payment release
- **Checklist Done** / **Checklist Concluido**: Supervisor verification completion -- PAYMENT TRIGGER for subcontractor
- **Class (QuickBooks)** / **Classe**: Project classification in QuickBooks for per-project financial reporting (format: CMER-###)

---

## BuilderTrend Job 455 -- Real Data (Supplement)

### Complete Financial Picture of Job 455
- **Contract Price**: $195,000 (open book: projected costs + markup)
- **Total PO Cost**: $150,850.83 across 122 Purchase Orders
- **Total Bills**: 178 processed bills
- **Contract Type**: Production/Spec (cost-plus model)

### Draw Schedule on Job 455
| Draw | Trigger | Date | Payment Cluster |
|------|---------|------|----------------|
| 1st Draw | Contract Sign | Dec 23-27, 2024 | Pre-construction: survey ($1,540), floor plan ($750), energy calc ($200), septic plan ($600) |
| 2nd Draw | Slab Complete | Feb 19, 2025 | Foundation materials, grading ($330), underground plumbing |
| 3rd Draw | Roof Complete | Mar 10-14, 2025 | Masonry ($5,450), framing ($5,160), roofing ($6,700) |
| 4th Draw | Insulation Complete | Mar 14-19, 2025 | Roughs: plumbing ($3,200), electric ($6,470), AC ($7,300), insulation ($1,450), stucco ($3,450) |
| Final | Close-Out | Sep 2025 | Finishing, landscaping, final clean, utility catch-up |

### Bill Payment Patterns
- **Average**: ~20 bills/month during active construction
- **Recurring**: Energy ($43-$129/mo), water ($13.50/mo), portable toilet ($122/period)
- **Largest single trade**: Windows ($22,368)
- **Water spike**: $456.64 in Oct 2025 (construction water or connection fees)

### Accounting Tags from Daily Logs
| Tag | Purpose |
|-----|---------|
| #F$1.01 - 1ST DRAW | Draw milestone tracking |
| #F$8 - DRAW RECEIVED | Payment received confirmation |
| #F$9 - PAYMENT HOLD | Payment hold flag |
| #F$ - ACCOUNTING CLOSED | Financial close-out |

### QuickBooks Integration
- Job 455 linked to QuickBooks Online with sub_customer = "AVLA LLC"
- Bills created in BuilderTrend replicated in QuickBooks for accounting

## CPM Construction Sequence -- Finance Touchpoints

### Exceeding Costs Sub-System
The CPM defines an Exceeding Costs sub-system with 4 triggers:
1. **Client Hold**: Client-initiated hold on a process
2. **Changelog**: Change to execution plan
3. **Purchase Upgrade**: Material/purchase upgrade needed
4. **Service Upgrade**: Service upgrade needed

**State Machine**: Client Hold Evaluation -> Cost Approved/Disapproved -> Project Discontinuation (worst case)
**Payment Hold Logic**: "PROCESS + PAYMENT HOLD" -> "PROCESS + DRAW RECEIVED" -> service scheduling continues
**Estimability Decision**: If estimable=TRUE -> standard flow; if FALSE -> requires additional draw request

### Financial Metrics from CPM
| Metric | Description |
|--------|-------------|
| Total Processing Time | End-to-end time for exceeding cost process |
| Cost Approval Rate | Target: 70% approval rate |
| Project Discontinuation Rate | Monitor discontinuation trends |
| Exceeding Costs Opening Rate | Which triggers most frequently start the process |

## Const App Integration (Supplement)

### Accounts Payable Module
- **Verified POs**: Review and manage payment-ready purchase orders (Pending Invoices, Ready for Payment, Processing, Authorized, Paid)
- **Payment Batches**: Create and manage payment batches for bulk processing
- **Authorization**: Authorize payment batches and manage approvals

### Accounts Receivable Module
- **Contract Payments**: Track draw payments per contract (CTR-2026-0001: $20 paid, 1 of 1 draws)
- **Payment tracking columns**: Contract #, Client, Total Amount, Payment Progress, Next Draw Due, Contract Status

### Client Relations Module (Financial)
- **Exceeding Costs**: Budget threshold events for utility services -- projects where actual utility costs exceeded budgeted amounts (read-only)
