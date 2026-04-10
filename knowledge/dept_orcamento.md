# Orcamento / Budget - Lakeshore Development

## Visao Geral
- **Missao:** Elaborar e gerenciar orcamentos (budgets) para todas as casas construidas pela Lakeshore, incluindo spec homes e custom homes, garantindo controle de custos por cost code e modelo
- **Lider:** Felipe Nery - Engenheiro de Orcamento / Budget Lead (fnery@lakeshoredevelopmentfl.com)
- **Equipe:**
  - Ana Helena Torres (atorres@lakeshoredevelopmentfl.com) - Equipe de Orcamento, integracao estimate-POs no Builder Trend
  - Pedro Henrique Cordeiro - Equipe de Cotacoes
  - Rodrigo Cordeiro - Responsavel pela Concretagem/Budget de concreto
- **Departamentos relacionados:** Setor de Projetos/Arquitetura, Compras, Financeiro, Scheduling, Permits, Contratos, Client Relations

## Processos

### Processo 1: Orcamento de Spec Homes
- **Objetivo:** Criar e manter templates de orcamento para casas padronizadas (M1, M9, M10, M32, etc.) com replicabilidade
- **Responsavel principal:** Felipe Nery / Samuel Torres (Sam)
- **Frequencia:** Por modelo novo; atualizacao quando precos mudam
- **Ferramentas:** Builder Trend (templates de POs), Planilhas Excel (budgets), ClickUp (acompanhamento)

**Passo a passo:**
1. Receber planta e especificacoes do modelo padronizado -- Responsavel: Setor de Projetos (Camila) -- Ferramenta: Google Drive
2. Utilizar templates replicaveis com POs na ordem dos Cost Codes -- Responsavel: Felipe Nery -- Ferramenta: Builder Trend
3. Aplicar cotacoes ja existentes (mesmos materiais e precos por modelo) -- Responsavel: Felipe Nery / Ana Helena -- Ferramenta: Planilhas Excel
4. Ajustar taxas especificas por condado (Marion, Citrus, Charlotte) -- Responsavel: Felipe Nery -- Ferramenta: Planilhas Excel
5. Samuel (Sam) revisa valores finais com base na experiencia -- Responsavel: Samuel Torres -- Ferramenta: Planilhas Excel
6. Budget fechado; alterado apenas em caso de aumento de preco de material ou mao de obra -- Responsavel: Felipe Nery -- Ferramenta: Builder Trend

**Inputs:** Floor plans, spec sheet, design book (do Setor de Projetos); cotacoes de fornecedores
**Outputs:** Budget fechado por modelo, disponivel para Scheduling e Financeiro
**Observacoes:** Para specs, dependencia menor do setor de projetos. Orcamentos fechados sao replicaveis entre casas do mesmo modelo.

### Processo 2: Orcamento de Custom Homes
- **Objetivo:** Elaborar orcamento individualizado para casas personalizadas com base em especificacoes unicas do cliente
- **Responsavel principal:** Felipe Nery
- **Frequencia:** Por projeto (cada casa custom e unica)
- **Ferramentas:** Planilhas Excel, Builder Trend, Google Drive

**Passo a passo:**
1. Camila (arquiteta) ouve o cliente e produz o Design Book -- Responsavel: Camila Martins -- Ferramenta: AutoCAD, SketchUp
2. Receber Design Book + Takeoff como base para orcamento -- Responsavel: Felipe Nery -- Ferramenta: Google Drive
3. Solicitar cotacoes individuais para cada novo projeto a pelo menos 3 fornecedores -- Responsavel: Felipe Nery / Pedro Henrique -- Ferramenta: E-mail, WhatsApp
4. Detalhar itens e custos personalizados (piscina, acabamentos especiais) -- Responsavel: Felipe Nery -- Ferramenta: Planilhas Excel
5. Definir allowances e by owner com Camila antes de fechar contrato -- Responsavel: Camila Martins / Felipe Nery -- Ferramenta: Reuniao presencial
6. Samuel e Camila aprovam budget inicial (R3, estimativa) -- Responsavel: Samuel Torres, Camila Martins -- Ferramenta: Planilhas Excel
7. Apos contrato, PMs (Daniel, Cris, Edson) aprovam budget real com cotacoes de subs -- Responsavel: PMs -- Ferramenta: [detalhes nao disponiveis nos documentos fonte]

**Inputs:** Design Book, Takeoff, spec sheet, floor plans (de Camila/Projetos); cotacoes individuais de fornecedores
**Outputs:** Budget personalizado para aprovacao do cliente; budget real pos-contrato para execucao
**Observacoes:** Nao ha setor de compras dedicado a customs; compra feita pelo scheduling de custom homes. Clientes mudam especificacoes durante a obra, exigindo revisao constante do budget.

### Processo 3: Fluxo de Cotacao
- **Objetivo:** Obter cotacoes competitivas de fornecedores para materiais e servicos, garantindo melhor custo-beneficio
- **Responsavel principal:** Pedro Henrique Cordeiro / Ana Helena Torres
- **Frequencia:** Por projeto (custom) ou por atualizacao de precos (spec)
- **Ferramentas:** Planilhas Excel (com codificacao por cores), E-mail, WhatsApp

**Passo a passo:**
1. Contatar fornecedores para obter precos de materiais e servicos -- Responsavel: Pedro Henrique / Ana Helena -- Ferramenta: E-mail, WhatsApp
2. Buscar 2-3 cotacoes por servico para melhores negociacoes e backup -- Responsavel: Pedro Henrique -- Ferramenta: E-mail
3. Registrar cotacoes na planilha com status por cores (Amarelo=pendente, Branco=recebida, Laranja=todas recebidas, Verde=aprovado) -- Responsavel: Pedro Henrique -- Ferramenta: Planilhas Excel
4. Apresentar informacoes ao Sam para negociacao em volume -- Responsavel: Pedro Henrique -- Ferramenta: Planilhas Excel
5. Sam revisa valores finais, marca em vermelho se incoerente -- Responsavel: Samuel Torres -- Ferramenta: Planilhas Excel
6. Aprovacao final pelo Sam (status verde) -- Responsavel: Samuel Torres -- Ferramenta: Planilhas Excel

**Inputs:** Lista de servicos/materiais necessarios (do Takeoff); tabelas de precos de fornecedores
**Outputs:** Cotacoes aprovadas que alimentam o budget e o modulo de Contratos
**Observacoes:** Comunicacao com subs principalmente por e-mail e WhatsApp. Muitos fornecedores tem dificuldade tecnologica.

### Processo 4: Cotacao de Materiais com Valor Unitario (Blocos, Concreto)
- **Objetivo:** Calcular custo de materiais onde o fornecedor nao faz takeoff, usando tabela de precos unitarios multiplicada pela quantidade do takeoff
- **Responsavel principal:** Pedro Henrique Cordeiro / Gabriela Medeiros (takeoff)
- **Frequencia:** Por projeto/modelo
- **Ferramentas:** Planilhas Excel, Software Globin, ChatGPT

**Passo a passo:**
1. Fornecedor envia tabela de precos com valor unitario (ex: DZ Blocks - bloco regular $1,89) -- Responsavel: Pedro Henrique -- Ferramenta: E-mail
2. Equipe de Takeoff (Gabriela) faz levantamento de quantidade usando IA e Globin -- Responsavel: Gabriela Medeiros -- Ferramenta: Software Globin, ChatGPT
3. Calculo manual: quantidade do takeoff x valor unitario da tabela de precos -- Responsavel: Pedro Henrique -- Ferramenta: Planilhas Excel
4. Valor final inserido na planilha do projeto -- Responsavel: Pedro Henrique -- Ferramenta: Planilhas Excel

**Inputs:** Tabela de precos do fornecedor; quantidades do takeoff (de Gabriela/Equipe de Projetos)
**Outputs:** Valor total calculado por item para o budget
**Observacoes:** Variacao natural de ~10% na quantidade (diferentes subs montam de formas diferentes). Materiais com valor unitario incluem: slab concrete, lintel concrete, blocks. Para servicos com valor fechado, o sub faz seu proprio takeoff.

### Processo 5: Estimativas Pre-Contrato (R3)
- **Objetivo:** Fornecer estimativa de custo ao cliente antes do contrato formal, baseada em custo por square feet de projetos anteriores
- **Responsavel principal:** Samuel Torres (Sam)
- **Frequencia:** Por lead/projeto custom
- **Ferramentas:** Planilhas Excel

**Passo a passo:**
1. Cliente paga para desenvolver conceito do projeto -- Responsavel: Camila Martins -- Ferramenta: [detalhes nao disponiveis nos documentos fonte]
2. Estimar custo por square feet com base em projetos recentes da mesma categoria -- Responsavel: Samuel Torres -- Ferramenta: Planilhas Excel
3. Aplicar coeficiente de custo por square feet para o nivel adequado (entrada, medio, alto padrao) -- Responsavel: Samuel Torres -- Ferramenta: Planilhas Excel
4. Apresentar estimativa ao cliente -- Responsavel: Samuel Torres / Camila -- Ferramenta: Reuniao

**Inputs:** Conceito do projeto, area em square feet, categoria/nivel do projeto
**Outputs:** Estimativa de custo (R3) para negociacao de contrato
**Observacoes:** Variaveis de terreno (final grading, septic connection) impactam precisao. Derivado da media dos custos totais de projetos recentes / square feet total. Quote inicial deve se transformar em budget ao virar contrato.

### Processo 6: Fluxo de MAP (Mecanica, Eletrica, Encanamento)
- **Objetivo:** Gerenciar orcamento de servicos MEP considerando diferentes contratos e divisoes de pagamento
- **Responsavel principal:** Felipe Nery
- **Frequencia:** Por projeto
- **Ferramentas:** Planilhas Excel, Builder Trend

**Passo a passo:**
1. Departamento de Permits define se e Full MAP ou nao no momento da aplicacao -- Responsavel: Equipe de Permits -- Ferramenta: Site do condado
2. Aplicar divisao de pagamento conforme fornecedor (FOCO: 40%-40%-20%; ECOWAN: 40%-30%-30%) -- Responsavel: Felipe Nery -- Ferramenta: Planilhas Excel
3. Registrar deducoes especificas quando aplicavel (ex: $679.01 por banheira nao fornecida) -- Responsavel: Felipe Nery -- Ferramenta: Planilhas Excel
4. Controlar que invoices vinculadas a uma PO nao excedam o valor da PO -- Responsavel: Ana Helena / Financeiro -- Ferramenta: Builder Trend

**Inputs:** Definicao de Full MAP (do Permit); contratos com fornecedores MEP
**Outputs:** POs com divisao de pagamento correta para Financeiro
**Observacoes:** Contratos diferentes entre FOCO e ECOWAN exigem atencao na divisao de pagamento.

## Dores e Problemas Conhecidos
- **Atualizacao de precos**: materiais e tarifas mudam rapidamente nos EUA; invoices com valores diferentes das POs
- **Integracao estimate-POs no BT**: tarefa manual trabalhosa feita por Ana Helena
- **Volatilidade do takeoff**: projeto muda varias vezes; takeoff precisa ser refeito; conversao de areas em unidades e manual
- **Falta de padronizacao**: muito conhecimento na cabeca dos gestores; falta caminho padronizado
- **POs fora de ordem no BT antigo**: cadastradas aleatoriamente, dificultando comparacao com planilha de orcamento
- **Dificuldade com casas custom**: cada projeto e unico; cotacoes iniciais inevitavelmente mudam
- **Duplicacao de funcoes**: ex: Energy Calculation solicitado tanto por budget quanto por permit
- **Comunicacao com subs**: muitos tem dificuldade tecnologica; dependem de WhatsApp/telefone
- **Inconsistencia no takeoff de blocos**: diferentes subs pedem quantidades variadas; nao ha padrao definido
- **Falta de historico centralizado**: mudancas de takeoff nao notificam automaticamente equipe de budget
- **Budget deveria estar pronto antes do permit sair, mas frequentemente esta atrasado**

## Dependencias
- **Recebe de:** Setor de Projetos -> takeoff, design book, specification sheet, floor plans; Permit -> definicao de full MAP, condado; Client Relations (Camila) -> definicao de allowance, by owner, upgrades
- **Entrega para:** Contratos (Bruna) -> cotacoes selecionadas como base para contratos; Scheduling -> budget como referencia para pedidos; Financeiro -> valores de referencia de POs e budgets; Compras -> base para compras de materiais

---

## Especificacao do Software (Fonte: Drive QPS)

### Templates: Models e Estimates

O modulo PROJECT MANAGEMENT > TEMPLATES e subdividido em dois tipos:

- **MODEL**: template de cronograma de construcao vinculado a um modelo de planta. Cada template de modelo e atrelado a um condado - mesmo modelo em condados diferentes exige templates separados. Campos obrigatorios: Model Code, County, Square Footage, Floor Plan. Apos criar o template, o usuario cadastra os itens do cronograma com seus predecessores. Cada item pode ser do tipo Service (selecionado da base de servicos cadastrados) ou Internal Process. O template de modelo pode ser atrelado a um template de Estimate.
- **ESTIMATE**: template de orcamento com custos estimados por cost code, com breakdown de servicos dentro de cada cost code. Tipos de custo possiveis: Service, Material, Other. O cost code e preenchido automaticamente para servicos e materiais, ou selecionado manualmente para o tipo Other.

Regra critica: ao vincular um estimate a um projeto, os valores ficam congelados no projeto - mudancas de preco na base de dados refletem apenas em projetos futuros, nunca no estimate de projetos ja cadastrados.

### Vinculo Estimate -> Projeto

Ao criar um novo projeto, o usuario seleciona um Model Code (filtrado pelo condado do projeto). Se houver um estimate atrelado ao modelo selecionado, ele e sugerido automaticamente. O estimate selecionado gera o Schedule of Value do projeto (parcelas de 1st a 5th draw), com percentuais ajustaveis que devem totalizar 100%.

### Estrutura de Cost Codes

Cada servico e material cadastrado no sistema carrega um cost code. Os estimates organizam os custos por cost code, com detalhamento de servicos e materiais dentro de cada codigo. Essa estrutura alimenta o modulo FINANCES > PROJECT DETAILS > BUDGET para comparacao de custos estimados x projetados x reais.

### Fluxo de Aprovacao de Service Orders e Purchase Orders

- **Aprovacao automatica**: se o valor da ordem (servico ou compra) for menor ou igual ao valor previsto no estimate do projeto, a ordem e aprovada automaticamente.
- **Aprovacao manual**: se o valor for maior que o estimado, ou se a ordem nao estava prevista (ex: reparo), ela requer aprovacao do project manager.
- Ao ser aprovada, o responsavel pela compra/contratacao recebe notificacao e uma task para executar o pedido.
- Ao receber confirmacao de conclusao em ACTIVITY LOG, a ordem passa automaticamente para status COMPLETED.

---

## Dados de Referencia (Fonte: Drive Lakeshore)

### Estrutura do Controle MEP

O controle MEP (Mechanical, Electrical, Plumbing) e usado pelo Orcamento para validar valores de invoices e change orders frente ao budget aprovado. Campos principais:

- **Identificador da casa:** codigo de referencia (ex: C1-0445-ND0M2) + numero do lote/permit
- **Sub:** empresa executora (ex: Eco One Plumbing Services, Eco One Electrical Services)
- **Valor:** valor da invoice ou change order
- **Numero da Invoice:** referencia fiscal para cruzamento com PO
- **Descricao do servico:** o que foi realizado (ex: Broken Pipe Repair, Change Order: Connect Meter, Fill Up for Inspection)
- **Situacao:** OK (aprovado) ou NEGADO (rejeitado — justificativa registrada na linha seguinte)
- **Data da Invoice:** data de emissao para controle de fluxo de caixa

Valores de referencia recorrentes: trip charge padrao $90; servicos como broken pipe repair, kitchen disconnect and connect, vacuum breaker, water line repair. Change orders acima do escopo contratual sao negados com justificativa documentada.

---

### Estimativa de Desembolso

Planilha de referencia para projecao de desembolso financeiro ao longo do tempo, com cenarios de pagamento. Estrutura:

**Cabecalho:** descricao do item, quantidade, valor unitario, valor total

**Fluxo de desembolso por cenario:** distribui o total em datas especificas (ex: Sep-29, Sep-26, Oct-20, Aprovacao I-140), permitindo comparar timing de pagamentos entre cenarios.

Exemplo de estrutura com 4 cenarios:
| Cenario | Total | Logica |
|---|---|---|
| Cenario 1 | valor total | todos os itens pagos, timing padrao |
| Cenario 2 | valor total | reordenacao de pagamentos por data |
| Cenario 3 | valor reduzido | exclusao de alguns itens |
| Cenario 4 | valor reduzido | idem, timing alternativo |

Uso no Orcamento: modelo de referencia para estruturar fluxo de desembolso de projetos com pagamentos parcelados em datas distintas (ex: materiais, servicos MEP, draws). Aplicavel para projetar cronograma financeiro por fase de obra alinhado com datas de draw.

---

## Operational Detail (from Interviews)

### Quote Color-Coding System

The quoting process uses a color-coding system in spreadsheets to track status:

- **Yellow** = Pending / needs review -- quote has been requested but not yet received or evaluated
- **White** = Standard / received -- quote received from vendor, awaiting comparison
- **Orange** = All received / needs attention -- all quotes for this item received, ready for Sam's review
- **Green** = Approved / within budget -- Sam has reviewed and approved the quote
- **Red** = Over budget / rejected / incoherent -- Sam flagged the value as incoherent or over budget

### 10% Variance Expectation

Budget estimates are expected to be within 10% of actual costs. A variance greater than 10% triggers a review by Samuel Torres. This is especially relevant for materials with unit pricing (blocks, concrete) where different subs may use slightly different quantities. The ~10% natural variation in takeoff quantities across subs is considered acceptable.

### Budget R3 vs Real

- **R3** = Initial budget estimate (revision 3 of the cost model). Created before contract signing, based on cost-per-square-foot of recent similar projects. Used for client negotiation and contract pricing.
- **Real** = Actual costs as invoices come in during construction. Tracked against the R3 estimate to flag divergence.

Agents must track both R3 and Real values and flag when actual costs diverge significantly from the initial estimate. The R3-to-Real comparison is critical for the Financeiro closing process and for detecting cost overruns early.

### Vendor Takeoff Gaps

Some vendors do not provide detailed takeoffs (material breakdowns). In these cases, the Estimator (Felipe Nery / Pedro Henrique) must verify quantities independently. Common gaps include:

- **Concrete**: Vendor quotes per yard, but actual needs require per-footing calculation based on the takeoff. The estimator must cross-reference the vendor's unit price with Gabriela's takeoff quantities.
- **Blocks**: Different subs request different quantities for the same house model. No industry standard exists for block counts -- the estimator must reconcile.
- **Lumber**: The new lumber supplier (84Lumber) does not perform takeoffs. Nobody on the Lakeshore team currently knows how to do lumber takeoffs, creating a critical knowledge gap.

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- [Catalogo de Dores](07_CATALOGO_DORES.md)
- [Fluxo Spec Home](05_FLUXO_SPEC_HOME.md)
- [Fluxo Custom Home](06_FLUXO_CUSTOM_HOME.md)
- [Glossario de Termos](03_GLOSSARIO.md)
- **Departamentos relacionados:**
  - [Escritorio de Projetos](dept_escritorio_projetos.md) — fornece takeoff, design book, spec sheet
  - [Permits](dept_permits.md) — fornece definicao de full MAP
  - [Client Relations](dept_client_relations.md) — define allowances e upgrades
  - [Scheduling](dept_scheduling.md) — usa budget como referencia para pedidos
  - [Financeiro](dept_financeiro.md) — recebe valores de referencia de POs e budgets
  - [Compras](dept_compras.md) — recebe base para compras de materiais

## Key Glossary Terms

> Terms from [Glossario de Termos](03_GLOSSARIO.md) most relevant to the Orcamento (Budget/Estimating) department.

- **Take-Off (Takeoff)** / **Levantamento Quantitativo**: Detailed material quantity survey from project plans -- feeds budget calculations and PO creation
- **Cost Code** / **Codigo de Custo**: Numeric code categorizing each cost type/service phase in a project -- base for POs and accounting allocation
- **Budget R3** / **Orcamento Estimativo Inicial**: Rough cost estimate without formal sub quotes, based on cost per square foot and past projects (~$250/sq ft)
- **Budget (Orcamento)** / **Orcamento**: Detailed estimate of all project costs including materials, labor, and fees -- central to all departments
- **Variance** / **Variacoes**: Unclassified or unexpected costs, often from emergency field purchases without proper classification
- **Change Order** / **Ordem de Alteracao**: Formal modification to scope, cost, or schedule after contract signing -- impacts budget and scheduling
- **Allowance** / **Provisao/Verba Estimada**: Contractual margin for items with unknown exact cost (e.g., loads, finishes) -- defined before contract
- **Unit Price** / **Preco Unitario**: Cost per unit of material or service from vendor price tables (e.g., $2.85/block)
- **Markup** / **Margem**: Percentage added to costs for overhead and profit
- **Cost-Plus** / **Custo Mais Margem**: Contract type where client pays actual cost plus agreed markup percentage
- **Subcontract** / **Sub / Subcontratado**: Third-party service provider hired for specific construction phases
- **Material** / **Material**: Physical goods purchased for construction (blocks, lumber, fixtures)
- **Labor** / **Mao de Obra**: Workforce cost for installation and construction services
- **Overhead** / **Custos Indiretos**: Indirect costs not tied to a specific task (insurance, office, permits)
- **Contingency** / **Contingencia**: Budget reserve for unforeseen costs, typically 5-10% of total

## Vendor Quote Matching (Batch 5)

### Vendor Quote Matching Issues (from Batch 5 validation interviews, 12/03/2026 - 23/03/2026)

The budget team faces significant challenges when comparing quotes from different vendors due to incompatible naming systems:

**CAS Creed vs CMEX Nomenclature Problem:**
- CAS Creed (CAS CR) provides foundation and precast takeoff and pricing
- CMEX provides competing prices using a completely different item naming system
- There is NO standardized nomenclature between vendors -- each uses their own internal catalog
- Example: CAS Creed "8x8x16 regular block" may correspond to CMEX "Standard CMU 8-inch" -- but this mapping must be done manually for every item
- The team takes CAS Creed's takeoff (quantities) and tries to find equivalent items in CMEX's price table to negotiate better prices

**How to Reconcile Cost Codes Between Systems:**
1. Start with CAS Creed's itemized takeoff (they provide detailed material breakdown)
2. Open CMEX's price table side by side
3. For each CAS Creed item, manually search for the equivalent CMEX item by description, dimensions, and material type
4. Record the mapping in a spreadsheet (no permanent equivalence table exists)
5. Compare unit prices between CAS Creed and CMEX for each mapped item
6. Select the vendor with better pricing per item or negotiate volume discounts

**Real Validation Findings from Batch 5 Sessions:**
- **Price discrepancies**: Same material can have 15-30% price difference between vendors -- comparing apples to apples is critical
- **Unit mismatches**: One vendor quotes per unit (each), another per pallet, another per cubic yard -- team must normalize units before comparison
- **Missing items**: CMEX price table may not include all items from CAS Creed's takeoff -- these gaps must be filled by requesting specific quotes
- **Volume pricing**: Vendors like FOCO and ECOWAN have volume-dependent pricing (e.g., FOCO: 40%-40%-20% payment split; ECOWAN: 40%-30%-30%) -- direct unit price comparison is misleading without considering payment terms

### Software Validation Insights (Batch 5)

During real-world testing of the Lakeshore software with the budget team:
- **Vendor takeoff feature approved**: "Enable Vendor Takeoff" correctly transfers responsibility to vendor
- **Price table registration needed**: Team requested ability to register a vendor's complete price table in the system (detached from specific model) so quotes can be auto-calculated
- **Numeric validation missing**: System needed cifrão/comma/period format validation for monetary values
- **Stocked vs Quoted redefinition**: Team clarified that "Stocked" means ONLY items in warehouse; "Quoted" means materials purchased internally; "Non-stock" means custom project materials not in regular inventory; "By Sub" means provided by subcontractor

---

## BuilderTrend Job 455 -- Real Data

### Budget vs Actual on Job 455
- **Contract Price**: $195,000 (open book, cost-plus)
- **Total PO Cost**: $150,850.83 (122 POs)
- **Total Bills**: 178 processed
- **Change Orders**: 0 (no scope changes)
- **Model**: 1774 sqft, Marion County

### Cost Breakdown by Trade (from Bills)
| Trade | Estimated Cost | Vendor |
|-------|---------------|--------|
| Windows | $22,368 | (largest single trade) |
| AC/HVAC | $7,300 | AC sub |
| Cabinets & Countertop | $6,978 | ONYX GRANITE |
| Roofing | $6,700 | Roofing sub |
| Electrical | $6,470 | Electrical sub |
| Trusses | $6,500 | Truss Direct LLC |
| Lumber | $6,177 | 84 Lumber |
| Blocks | $5,713 | Cemex |
| Framing | $5,160 | Framing sub |
| Masonry | $5,450 | Masonry sub |
| Driveway Pavers | $5,053 | Red Twelve LLC |
| Sewer Connection | $4,600 | Leesburg Septic |
| Stucco + Lath | $3,450 | J.A.S.H. Services |
| Plumbing Rough | $3,200 | Eco One Plumbing |
| Vinyl Material | $2,808 | AMERICAN STORE LLC |
| Tile + Vinyl Install | $2,404 | IVISION GROUP |
| Garage Door | $1,850 | Strong Quality |
| Lintel Concrete | $1,693 | Del Zotto Concrete |
| AMB Surveying (all) | $1,540 | AMB Surveying |
| Insulation | $1,450 | ETERNAL INSULATION |
| Casings/Baseboards | $970 | Imeca Web POS |

### PO Categories Mapped to Cost Codes
| Category | Cost Code | PO Count | Total |
|----------|-----------|----------|-------|
| Pre-construction | 1-2 | 7 | ~$3,240 |
| Land prep | 4 | 5+ | ~$2,510 |
| Foundation | 5 | 5+ | ~$8,406 |
| Plumbing | 6 | 2+ | ~$3,350 |
| Electrical | 7 | 1+ | ~$6,470 |
| Masonry | 8 | 3+ | ~$12,863 |
| Roofing/Framing | 9 | 3+ | ~$19,377 |
| Windows | 10 | 1+ | ~$22,368 |
| Doors | 11 | 4+ | ~$2,232 |
| Finishing | 13 | 10+ | ~$17,690 |
| Exterior | 14 | 5+ | ~$5,903 |
| Utilities | 3 | 8+ | ~$1,713 |

### Budget Template Validation
The 19 cost categories in the Const App model 1774 match the structure used on Job 455. Only Utilities (category 3) has a set budget: $4,300 (Water $1,500, Sewage $800, Energy $2,000). Actual utilities on Job 455: $563 energy + $538 water = $1,101 (well under budget).

## CPM Construction Sequence -- Budget Touchpoints

### Cost Estimation by CPM Phase
| CPM Phase | Key Budget Items | Typical Duration |
|-----------|-----------------|-----------------|
| FASE 1: Site Prep | Survey ($1,540), Clear Lot ($1,150), Slab Grading ($330) | 2-3 weeks |
| FASE 2: Foundation | Blocks ($5,713), Concrete ($1,693), Foundation Material | 2 weeks |
| FASE 3: Framing/Roughs | Trusses ($6,500), Lumber ($6,177), Windows ($22,368), MEP roughs ($16,970) | 6+ weeks |
| FASE 4: Finish/Close | Cabinets ($6,978), Tile/Vinyl ($5,212), Painting, Trim, Clean | 6+ weeks |

### Exceeding Costs Sub-System -- Budget Impact
The CPM exceeding costs sub-system affects budget when:
- **Purchase Upgrade**: Material upgrade requested -> quotation -> cost approval -> additional draw if needed
- **Service Upgrade**: Service upgrade requested -> quotation -> cost approval -> additional draw if needed
- **Client Hold**: Cost overage detected -> budget evaluation -> approved or discontinued
- **Target**: 70% cost approval rate

### Budget Variations by County
Budget templates vary by county due to different:
- Permit fees and impact fees
- Wind speed requirements (120 mph Marion vs 140-150 mph Charlotte)
- Utility providers and connection costs
- Inspection requirements (Marion vs Citrus differences)
- Labor rates (coastal counties typically higher)

## Const App Integration

### Model 1774 Cost Structure (206 Line Items)
19 cost categories with 206 line items covering all construction trades. Items with quantities defined include:
- Foundation: 8 components (rebar, poly, bar chair, tape)
- Precast: 12 components (lintels, sills, rebar, dowels, corner bars, formmat)
- Plumbing Fixtures: 13 components (toilets, sinks, faucets, bath kit, mirrors)
- Electrical Fixtures: 6 components (coach lights, recessed, vanity, pendant, vintage)
- Roofing: Architectural shingles 2,722.88 sqft
- Trim: Baseboard 512 lf, Window Sill 48 lf, Casings 544 lf
- Tile: Wall tile 179 sqft, floor tile 14.25 sqft + mortar, grout, caulk
- Countertop: 76.15 sqft + backsplash 24 sqft
- Flooring: Engineered wood 1,544.9 sqft + moisture barrier, adhesive

### Quotation Module
- **Take-off page**: Define service quantities per model (19 cost codes, 33 services, 74 components)
- **Supply types**: Stocked (27), Quoted (6), By Sub (10)
- **Vendor Takeoff**: Certain items flagged for vendor to provide their own quantity/price (foundation, precast)
