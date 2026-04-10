# Compras / Purchasing - Lakeshore Development

## Visao Geral
- **Missao:** Gerenciar todas as compras de materiais de construcao (estoque e diretas), controlar o armazem, distribuir materiais por casa e manter rastreabilidade contabil de cada item
- **Lider:** Brenda Amorim (bamorim@lakeshoredevelopmentfl.com) - Equipe de Compras
- **Equipe:**
  - Marilia Marie Santos - Equipe de Compras
  - Emily - Nova integrante da equipe
  - Seu Clauser - Responsavel pelo estoque fisico/armazem (warehouse)
- **Departamentos relacionados:** Orcamento/Budget, Financeiro, Scheduling, Setor de Projetos, Field/Supervisao

## Processos

### Processo 1: Compras de Estoque
- **Objetivo:** Abastecer o armazem com materiais necessarios para construcao, garantindo disponibilidade e controle contabil
- **Responsavel principal:** Brenda Amorim
- **Frequencia:** Grande compra mensal (inicio do mes) + reposicoes conforme necessidade
- **Ferramentas:** Zorro (software de estoque), Planilhas Excel, Builder Trend, E-mail

**Passo a passo:**
1. Realizar grande compra no inicio do mes baseada em necessidades previstas -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel, E-mail
2. Verificar estoque via planilha atualizada por Seu Clauser -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel
3. Registrar a compra com data, material, quantidade, numero da ordem e fornecedor -- Responsavel: Brenda Amorim / Marilia -- Ferramenta: Planilhas Excel
4. Inserir informacao no software Zorro (secao Resorders) -- Responsavel: Brenda Amorim -- Ferramenta: Zorro
5. Apos chegada do material, registrar na planilha de distribuicao para alocacao contabil -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel
6. Distribuir contabilmente: estoque -> casas (alocacao por projeto) -- Responsavel: Brenda Amorim / Marilia -- Ferramenta: Planilhas Excel
7. Replicar no Builder Trend (PO -> BI) -- Responsavel: Brenda Amorim -- Ferramenta: Builder Trend

**Inputs:** Takeoff e budget (do Orcamento); necessidades do Scheduling; nivel de estoque atual (de Seu Clauser)
**Outputs:** Material disponivel no armazem; registros de compra no Zorro e Builder Trend; distribuicao contabil por casa
**Observacoes:** Reposicoes adicionais ocorrem conforme demanda. Informacao duplicada intencionalmente em multiplos sistemas para verificacao.

### Processo 2: Fluxo de Saidas de Material
- **Objetivo:** Controlar e registrar todas as saidas de material do armazem para as obras, garantindo rastreabilidade
- **Responsavel principal:** Seu Clauser (registro fisico) / Brenda Amorim (registro contabil)
- **Frequencia:** Diaria
- **Ferramentas:** Zorro (Sales Orders), Planilhas Excel

**Passo a passo:**
1. Saidas registradas por Seu Clauser no Zorro (Sales Orders) -- Responsavel: Seu Clauser -- Ferramenta: Zorro
2. Equipe de Compras filtra saidas no Zorro (incluindo drafts nao confirmados) -- Responsavel: Brenda Amorim -- Ferramenta: Zorro
3. Numero da saida transferido para planilha de Purchase (aba Compras de Estoque) -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel
4. Consultar Planilha de Ordens Disponiveis para selecionar ordens com materiais necessarios -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel
5. Subtrair quantidade utilizada do total comprado -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel
6. Registrar casa de destino em ambas planilhas (Purchase e Ordens Disponiveis) -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel
7. Calcular e distribuir valor por casa -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel

**Inputs:** Registros de saida do Zorro (de Seu Clauser); ordens de compra existentes
**Outputs:** Distribuicao de custo por casa; atualizacao de saldo de estoque
**Observacoes:** Seu Clauser usa drafts para separar materiais antes da confirmacao, o que gera incertezas quando a confirmacao atrasa.

### Processo 3: Compras Diretas
- **Objetivo:** Adquirir materiais que nao passam pelo estoque, com entrega direta na obra
- **Responsavel principal:** Brenda Amorim
- **Frequencia:** Sob demanda
- **Ferramentas:** Builder Trend, E-mail, Home Depot, Amazon

**Passo a passo:**
1. Identificar necessidade de compra direta baseada no Takeoff -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel
2. Agendar entrega direto com fornecedor -- Responsavel: Brenda Amorim -- Ferramenta: E-mail, Telefone
3. Realizar compra (ex: azulejos na Home Depot) -- Responsavel: Brenda Amorim -- Ferramenta: Home Depot, Amazon
4. Controlar ordem por boleto/cartao de credito -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel
5. Inserir informacoes no Builder Trend -- Responsavel: Brenda Amorim -- Ferramenta: Builder Trend

**Inputs:** Takeoff com lista de materiais; specification sheet
**Outputs:** Material entregue diretamente na obra; registro no Builder Trend
**Observacoes:** Materiais como azulejos (tile) sao frequentemente comprados na Home Depot. Fornecedor Amazon apresenta problemas recorrentes de entrega (USPS nao encontra o armazem).

### Processo 4: Distribuicao Contabil de Materiais
- **Objetivo:** Rastrear destino e custo de cada material comprado, alocando valores corretamente por casa para fechamento contabil
- **Responsavel principal:** Brenda Amorim / Marilia Marie Santos
- **Frequencia:** Continua (acompanha cada saida)
- **Ferramentas:** Planilhas Excel (12+ abertas diariamente), Zorro, Builder Trend

**Passo a passo:**
1. Transferir dados de saida do Zorro para planilha de compras -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel
2. Inserir referencia da ordem e valor manualmente (Zorro nao integra) -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel
3. Na planilha de distribuicao, organizar por grupos de materiais, ordens especificas e quantidades por casa -- Responsavel: Marilia -- Ferramenta: Planilhas Excel
4. Rastrear destino de cada ordem -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel
5. Duplicar informacoes intencionalmente para verificacao cruzada -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel

**Inputs:** Dados de saida do Zorro; ordens de compra; informacao de destino das casas
**Outputs:** Planilha de distribuicao completa para fechamento contabil
**Observacoes:** Processo complexo de rastreamento, melhorado recentemente. A duplicacao intencional de informacoes serve como mecanismo de verificacao.

### Processo 5: Checklist de Fechamento de Casas
- **Objetivo:** Garantir que todos os valores de materiais estejam corretamente alocados antes do fechamento contabil da casa
- **Responsavel principal:** Brenda Amorim
- **Frequencia:** Por casa (no fechamento)
- **Ferramentas:** Planilhas Excel, Builder Trend

**Passo a passo:**
1. Conferir valores de distribuicao (planilha Purchase vs Builder Trend) -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel, Builder Trend
2. Garantir que valores estejam dentro do budget -- Responsavel: Brenda Amorim -- Ferramenta: Planilhas Excel
3. Somente apos verificacao, criar a BI (Bill) no Builder Trend -- Responsavel: Brenda Amorim -- Ferramenta: Builder Trend

**Inputs:** Planilha de distribuicao; budget original; registros do Builder Trend
**Outputs:** Aprovacao para criacao de BI; casa pronta para fechamento contabil
**Observacoes:** Este processo previne discrepancias entre o planejado e o realizado antes do fechamento financeiro.

## Dores e Problemas Conhecidos
- **Volume excessivo de planilhas**: 12+ planilhas com multiplas abas abertas diariamente; informacoes semelhantes em formatos diferentes
- **Zorro ineficaz para custos**: nao atualiza precos automaticamente; valores desconsiderados pela equipe
- **Zorro nao referencia lote de compra**: nao informa de qual compra veio o material saindo; dificulta calculo de custos
- **Inconsistencia no Takeoff**: takeoff muitas vezes nao seguido na pratica; diferentes subs usam quantidades variadas
- **Entregas da Amazon nao encontram o armazem**: problema recorrente com USPS; gera retrabalho e atrasos
- **Drafts nao confirmados no Zorro**: Seu Clauser usa drafts para separar materiais; confirmacao atrasada gera incertezas
- **Saidas de materiais volateis**: demandas repentinas e inesperadas impactam previsao de compras
- **Falta de controle de Seu Clauser sobre saidas**: nao tem autonomia para validar com Takeoff; nao sabe uso especifico
- **Casas finalizadas sem registro de saida**: Zorro mostra inconsistencias
- **Distribuicao manual propensa a erros**: processo complexo de rastreamento
- **Mudanca de fornecedor de lumber**: ninguem na empresa sabe fazer takeoff de lumber; novo fornecedor nao fara

## Dependencias
- **Recebe de:** Orcamento/Budget -> takeoff e budget como base para compras; Setor de Projetos -> takeoff, specification sheet; Scheduling -> agendamento de servicos e entregas; Field -> compras emergenciais com cartao
- **Entrega para:** Financeiro -> replicacao no Builder Trend, pagamentos, rateio; Scheduling -> materiais disponiveis no armazem; Corecraft -> materiais para entregas; Field/Obra -> materiais para construcao

---

## Manuais de Capacitacao (Fonte: Drive Lakeshore)

### Processo de Solicitacao de Lumber

**Fornecedor:** 84Lumber — Representante: Jacob Sherrill (Jacob.Sherrill@84lumber.com) — Canal: E-mail

**Gatilho:** Solicitacao de Blocos e Precast da casa (producao e entrega ocorrem juntas)

**Fluxo:**
1. Identificar dados da casa no BuilderTrend: endereco, cidade, estado, zip code, modelo (sq ft), pin drop, elevacao e lado da garagem (FL = Floor Plan na pasta Approved Docs)
2. Baixar documento NOC (deve sempre acompanhar a solicitacao) e o Floor Plan da pasta Approved Docs
3. Enviar e-mail em ingles com o modelo abaixo para Jacob Sherrill, anexando o NOC:

```
Hello, good afternoon!

We'd like to request Lumber to the address below:

1) [Street Address], [City], FL, [Zip code]
Pin drop: [Link do Pindrop]
For reference: House [numero] | Model [modelo]
ELEVATION [elevacao da casa]
ETA: [data de entrega]

Please, tell your guys to deliver the lumber to the back of the property so it won't be stolen easily.
Also, could you, please, confirm the ETA?

Thank you!
```

- ETA: mesmo dia do ETA do pedido de Blocos/Precast ou proximo dia util (Jacob confirma depois)
- Informacoes de elevacao e lado da garagem (GL = Garage Left, GR = Garage Right) vem do Floor Plan
- Para o modelo no email: usar o valor em square feet da casa

4. Aguardar email de Jacob com o estimate do valor
5. Criar/editar PO no BuilderTrend: Financial -> Purchase Orders -> buscar PO de Lumber com CTRL+F
   - Assigned to: 84Lumber
   - Marcar "Materials only"
   - Editar valor com base no estimate recebido de Jacob
   - Clicar em Save & Close
6. Criar Daily Log: Project Management -> Daily Logs -> + Daily Log
   - Tags: **#M - LUMBER MATERIALS** e **#ORDERED**
   - Title: "ETA - [data de entrega, ex: 06/16]"
   - Clicar em Publish (aguardar confirmacao de Jacob antes de publicar)

**Controle de qualidade:** manter planilha de compras diretas com registro individual por casa (data solicitacao, ETA confirmado, status de entrega)

---

### Processo de Solicitacao de Trusses

**Dois gatilhos distintos:**
- **Gatilho de producao:** solicitacao de Foundation Material da casa
- **Gatilho de entrega:** solicitacao de Blocos e Precast da casa (entrega deve ocorrer apos os blocos para nao atrapalhar a logistica)

**Fornecedores — como identificar qual usar:**
Consultar o documento Trusses Layout (TL) ou Trusses Engineering (TE) na pasta Approved Docs do projeto no BuilderTrend. A logo da empresa estara indicada no documento.

| Empresa | Representante | Canal | Contato |
|---|---|---|---|
| Truss Direct | Marcelo Franca | E-mail / WhatsApp | supplies@truss-direct.com / +1 (407) 758-8253 |
| Hitek | Suzanne Jensen, Bill, Gary | E-mail | scheduling@hitek-truss.com / bill@hitek-truss.com / gary@hitek-truss.com |

Obs: Modelos 1774 sao geralmente Truss Direct; demais geralmente Hitek. Confirmar sempre pelo TL/TE.

**Solicitacao de producao — Hitek (email em ingles, enviar para os tres emails simultaneamente):**
```
Hello, good [morning/afternoon]!

Request to production and schedule delivery of Trusses to the address:

1) [Street Address], [City/State], [Zip code] | [GL ou GR]
Pindrop: [pindrop]
For reference: House [numero] | Model [modelo]
ETA: [data de entrega estimada]
ELEVATION [elevacao da casa e estilo: Farmer ou Contemporary]

Thank you!
```

**Solicitacao de producao — Truss Direct (email em portugues para Marcello):**
```
Ola Marcello, tudo bem?

Segue a lista de producao de trusses:

Casa [numero] - [modelo] - [lado da garagem]
[endereco], [cidade], [estado], [zip code]
[link do Pin drop]
ETA: [data de entrega]

Obrigada!
```

**Calculo do ETA de producao:** ETA do Foundation Material + 2 semanas (tempo medio de construcao no cenario ideal). Nunca solicitar com ETA em segunda-feira.

**Valores de PO por fornecedor e modelo:**

Truss Direct:
| Modelo | Valor |
|---|---|
| 1630 / new 1630 | $7,500 |
| 1751 | $7,500 |
| 1774 | $6,500 |
| 1879 | $9,200 |
| 1888 | $9,800 |
| 1912 | $9,600 |
| 1919 | $10,200 |
| 2040 | $9,200 |

Hitek (por modelo e elevacao):
| Modelo + Elevacao | Valor |
|---|---|
| 1751 GBL / 1751 H | $5,500 |
| 1888 | $5,600 |
| 1878 A | $6,675 |
| 1878 B | $6,050 |
| 1896 A | $6,650 |
| 1896 B | $5,875 |
| 2040 A | $8,600 |
| 2040 B | $8,475 |
| 2040 C | $7,750 |
| 1959 | $6,000 |
| 1919 | $5,825 |
| 1912 | $5,850 |
| 1799 A | $5,525 |
| 1799 B | $6,200 |
| 1936 A | $6,350 |
| 1936 B | $6,900 |
| 2515 A | $9,400 |
| 2515 B | $9,700 |
| 2100 A | $6,725 |
| 2100 B | $8,000 |
| 2211 A | $8,300 |
| 2211 B | $7,175 |
| 2022 | $7,575 |
| 1955 | $6,350 |

**Criacao de PO no BuilderTrend:**
- Financial -> Purchase Orders -> buscar "Trusses" com CTRL+F
- Atencao: ha duas POs com nome Trusses — editar apenas a chamada "Trusses" (nao a "Trusses Plan")
- Assigned to: Truss Direct ou Hitek conforme fornecedor
- Marcar "Materials only"
- Editar valor conforme tabela acima (modelo + elevacao)
- Save & Close

**Daily Log de producao:**
- Tags: **#M - TRUSSES MATERIALS** e **#PRE ORDERED**
- Notes: "Producao de Trusses"
- Clicar em Publish

**Acompanhamento de entrega:**
- Quando faltar ~7 dias para a data de entrega sem sinal de pedido de blocos: verificar Daily Logs da casa
- Se nao houver previsao de blocos: adiar a entrega (Hitek via e-mail; Truss Direct via WhatsApp para Marcello) — adiar por 1 a 2 semanas
- Quando blocos forem pedidos e data de entrega confirmada: novo Daily Log
  - Tags: **#M - TRUSSES MATERIALS** e **#ORDERED**
  - Title: "ETA - [data, ex: 06/16]"
  - Publish

---

### Processo de Criacao de PO (Guia Geral)

Fluxo padrao para criacao de PO no BuilderTrend a partir de uma compra:

1. Pesquisar o numero da casa
2. Financial -> Purchase Orders
3. Filtrar por Tags para localizar a PO correspondente (ex: Door Knobs)
4. Verificar se a PO ja existe; se nao, criar nova
5. Para criar: clicar em Purchase Order e preencher:
   - Titulo da PO
   - Fornecedor (Assigned to)
   - PDF da order (quando disponivel)
   - Materiais e valores
6. Criar itens: Numero de Ordem + Nome do material -> Cost type -> Cost code -> Unit cost
   - O cost code normalmente recebe o nome do material
   - Alocar proporcional por casa quando a order cobre multiplas unidades (ex: 30 packs comprados, 6 units para esta casa)
7. Clicar em Save & Close

---

## Descricao de Cargo Formal (Fonte: Drive Lakeshore)

### Coordenador de Compras (Purchase)

- **Setor:** Compras / Purchasing
- **Descricao geral:** Gestao de compras diretas e de estoque de materiais de construcao, garantindo disponibilidade e rastreabilidade contabil por casa e por fase

**Compras diretas — Fases 1 e 2 (Critical Materials)**
- Verificar em qual etapa a construcao esta
- Verificar Take Off de acordo com o modelo da casa
- Confirmar as datas de entrega (ETAs)
- Solicitar os materiais
- Materiais de compra direta por fase:
  - Fase 1: Aluguel do Portable, Foundation Material
  - Fase 2: Blocks e Pre-Cast, Trusses e Lumber, Windows e External Doors (todas as janelas, sliding glass door e garage to house door)
  - Fase 3: Tile WC, Appliances (fogao, geladeira, microondas, lava-loucas)
- Para windows e doors: comunicar ao fornecedor sobre producao (Stocking List), realizar Pre-Walk para correcao de medidas e solicitar instalacao
- Apos cada solicitacao: atualizar sistemas (planilhas e Buildertrend)

**Compras de estoque — Fases 3 e 4**
- Levantamento de quantitativo de material por periodo (geralmente 1 mes)
- Logistica e controle de estoque dos materiais
- Procedimentos financeiros e atualizacao de sistema
- Materiais de estoque por categoria:
  - Materiais de construcao (Fase 3) e Hardware (Fase 2): Asphalt, Self-leveling
  - Trim-set materials (Fase 3): Front door, portas internas, bifolds, AC door, casings e baseboard
  - Flooring material (Fase 3): Vinil, plastico, builder paper, blue tape
  - Plumbing trim (Fase 3): chuveiros, torneiras (cozinha e banheiro), garbage disposal
  - Door knobs (Fase 3): macenetas de todas as portas, stop doors, electronic locker
  - Light fixtures (Fase 3): luzes gerais, pendentes (banheiros, cozinha e area externa)
  - Acessorios (Fase 3): house number, kits de banheiro, espelhos, prateleiras (closets e laundry), shutters, brackets
  - Garden set (Fase 4): plantas, mulch, mangueiras, sprinkles, timers

---

## Especificacao do Software (Fonte: Drive QPS)

### Modulo PURCHASE: Suppliers, Materials, Purchase Orders

O modulo PURCHASE e subdividido em tres areas, todas com visao geral (todos os counties) e visao individual por county.

**Suppliers (Fornecedores)**
Cadastro de fornecedores com: nome da empresa, county(s) atendidos, materiais fornecidos com unidade e preco, e multiplos contatos. Regra de county: ao selecionar um fornecedor em qualquer parte do sistema, apenas os fornecedores que atendem o county do projeto aparecem como opcao. Ex: material X tem fornecedores A, B e C; se B nao atende Marion County, ele nao aparece na selecao para projetos desse county.

**Materials (Materiais)**
Cadastro de materiais com: nome do material, fornecedores associados com preco e ETA por fornecedor. Um material pode ter multiplos fornecedores. O link material-fornecedor e bidirecional: ao cadastrar um material, associa-se fornecedor(es); ao cadastrar um fornecedor, associa-se material(is).

**Vinculo de materiais com o orcamento**: os valores dos materiais alimentam FINANCES > ESTIMATE. Mudancas de preco na base nao afetam projetos ou etapas ja iniciadas - apenas projetos futuros. O valor real no momento da compra (quando a PO e emitida) entra como BILL no projeto.

### Purchase Orders: Workflow e Aprovacao Automatica

A lista de purchase orders pode ser filtrada por status (PENDING, APPROVED, COMPLETED), data e projeto.

**Regra de aprovacao automatica**: se o valor da PO for menor ou igual ao valor previsto no estimate do projeto, ela e aprovada automaticamente. Se for maior, ou se nao estava prevista (ex: reparo), precisa de aprovacao manual do project manager.

**Fluxo completo de uma PO**:
1. PO criada (do zero ou via Purchase Update no Activity Log) -> status PENDING
2. Se valor dentro do estimate: aprovacao automatica -> status APPROVED
3. Se valor acima: aguarda aprovacao do PM -> ao aprovar, status APPROVED
4. Responsavel pela compra recebe notificacao + task para fazer o pedido
5. Confirmacao de entrega registrada em ACTIVITY LOG (Delivery Update) -> status COMPLETED automaticamente
6. Com status COMPLETED: informacoes enviadas automaticamente para FINANCES > PROJECT DETAILS > BILLS e FINANCES > PROJECT DETAILS > BUDGET do projeto como custo projetado
7. Apos pagamento processado: status PAID

**Integracao com o Activity Log**: ao registrar um Purchase Update no Activity Log, selecionando material e supplier, o sistema cria automaticamente uma PO puxando dados de PURCHASE > MATERIALS e PURCHASE > SUPPLIERS.

---

## Operational Detail (from Interviews)

### Concrete Ordering Workflow

The concrete ordering process follows a strict 6-step sequence coordinated between Scheduling, Estimator, Compras, and the supplier:

1. **Scheduler requests pour date** -- Scheduling department identifies when a house needs a concrete pour and communicates the target date
2. **Estimator calculates yardage from takeoff** -- Pedro Henrique or Gabriela calculates the exact yardage needed based on the takeoff quantities (per-footing calculation)
3. **Compras creates PO with supplier** -- Brenda creates the Purchase Order in BuilderTrend with the calculated quantity and supplier details
4. **Supplier confirms delivery window** -- Supplier confirms the delivery date and time window
5. **Pour crew confirms readiness** -- The subcontractor crew confirms they are ready to receive and pour on the scheduled date
6. **Compras finalizes delivery time** -- Brenda finalizes the exact delivery time with the supplier based on crew readiness

### Vendor Takeoff Gaps

Not all vendors provide material breakdowns (takeoffs). Compras must cross-reference PO quantities against the takeoff from Gabriela's team. Common issues include:

- **Lumber packages missing trim pieces** -- 84Lumber provides the main lumber package but trim pieces may not be included; Compras must verify completeness against the takeoff
- **Block quantity discrepancies** -- Different masonry subs request different block quantities for the same model; Compras flags discrepancies to Budget for resolution
- **Direct purchase items** -- Materials like tile, appliances, and door knobs are purchased directly by Compras without vendor takeoff; quantities come entirely from the internal takeoff

### Deposito (Warehouse) Operations

#### Daily Assignment-to-Takeoff Reconciliation

The Deposito (warehouse) performs a daily reconciliation process: Clauser checks what materials were assigned to specific jobs (houses) against what the takeoff specifies for those jobs. When discrepancies are found -- for example, more material sent to a house than the takeoff calls for, or material sent to a house not in the current schedule -- Clauser flags the discrepancy to Compras (Brenda) for resolution.

#### Clauser's Validation Limitation

Warehouse staff (Clauser) receives materials from suppliers and distributes them to job sites, but cannot autonomously validate incoming shipments against the Purchase Order. Clauser does not have access to PO details or takeoff quantities in the system. When he notices discrepancies (wrong quantities, wrong materials, damaged goods), he must flag them to Compras for resolution rather than resolving independently. This creates a bottleneck when Brenda is unavailable and materials need to go out urgently.

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- [Catalogo de Dores](07_CATALOGO_DORES.md)
- [Fluxo Spec Home](05_FLUXO_SPEC_HOME.md)
- [Fluxo Custom Home](06_FLUXO_CUSTOM_HOME.md)
- [Glossario de Termos](03_GLOSSARIO.md)
- **Departamentos relacionados:**
  - [Orcamento](dept_orcamento.md) — fornece takeoff e budget como base para compras
  - [Escritorio de Projetos](dept_escritorio_projetos.md) — fornece takeoff e spec sheet
  - [Scheduling](dept_scheduling.md) — solicita agendamento de servicos e entregas
  - [Financeiro](dept_financeiro.md) — recebe registros de compras e rateio
  - [Core Craft](dept_core_craft.md) — recebe invoices de appliances

## Key Glossary Terms

> Terms from [Glossario de Termos](03_GLOSSARIO.md) most relevant to the Compras (Purchasing) department.

- **PO (Purchase Order)** / **Ordem de Compra**: Formal purchase authorization document with defined value -- base for financial control and payment
- **Vendor** / **Fornecedor**: External company supplying materials or services to Lakeshore projects
- **Sub / Subcontractor** / **Subcontratado**: Third-party service provider contracted for specific construction tasks
- **Non-stock** / **Material Nao-estocado**: Material purchased internally for a specific project but not kept in regular inventory -- common for custom homes
- **Stocked** / **Em Estoque**: Material stored in Lakeshore warehouse, available for immediate distribution
- **Lead Time** / **Prazo de Entrega**: Time between placing an order and receiving the material on site
- **Take-Off (Takeoff)** / **Levantamento Quantitativo**: Material quantity survey from plans -- feeds purchasing decisions
- **Invoice** / **Fatura/Cobranca**: Bill sent by vendor/sub for payment -- received by email, processed daily
- **Retainage** / **Retencao Contratual**: Percentage withheld from payment as guarantee until satisfactory completion
- **By Sub** / **Fornecido pelo Subcontratado**: Material or service provided directly by the sub, not purchased by Lakeshore
- **Quoted** / **Cotado**: Material/service requiring vendor quotation (not in stock) -- needs quotes from 3+ vendors
- **BID** / **Proposta de Preco**: Price proposal from a vendor or sub for a service or material supply

## CPM Construction Sequence Reference

The CPM flowchart defines critical material delivery timing that Compras must coordinate with Scheduling.

**Material Delivery Timing Rules:**
- **Blocks and Precasts:** Must arrive 2 days AFTER Slab Pouring (concrete cure time -- materials stored on slab)
- **Foundation Material:** Order after UP Inspection approval; if UP fails, verify order to avoid theft risk
- **Trim Set Material:** Must arrive during final Cabinets/Granite phase, BEFORE Trim Set starts. Ensure Garage Door + Electronic Locker installed first (security)
- **Lumber:** Delivery triggered by Foundation Material; ETA = Foundation Material + 2 weeks. Deliver to back of property (theft prevention). Never schedule Monday delivery.
- **Trusses Manufacturing Request:** Triggered by Foundation Material order; delivery must come AFTER blocks
- **Windows and Doors Manufacturing Request:** Recently moved to after Stake House (earlier in the process)
- **Tile Material, Vinyl Material:** Must be delivered before Interior Paint phase
- **Electric Trim Material, Plumbing Trim Material:** Must arrive before respective trim installations
- **Drywall Material:** Request from sub with advance notice after Frame approval

**Key Dependencies:**
- Underground Electrical must be done with Slab Prep, NEVER after
- Electrical Meter requires house painted externally + house number (utility company, variable date)
- Water Meter installation by water company -- should be done early, no exact timing

**Windows and Doors Sub-System:** Full state machine for manufacturing -> ordering -> delivery -> installation. See [cpm_subsystems.md](cpm_subsystems.md) for complete flow.

**Full reference:** [cpm_construction_sequence.md](cpm_construction_sequence.md) | [cpm_subsystems.md](cpm_subsystems.md)

---

## Vendor Takeoff Workflows (Batch 5)

### Vendor-Side Takeoff Process (from Batch 5 validation interviews, 12/03/2026 - 23/03/2026)

When a vendor performs their own takeoff, the purchasing flow changes significantly:

**How Vendors Do Their Own Quantity Estimates:**
1. Compras (or Budget team) marks item as "Enable Vendor Takeoff" in the software
2. Vendor receives the project plans (floor plan, design book) via email or software request
3. Vendor performs their own material survey using their specialized tools and knowledge
4. Vendor returns a total price (often NOT itemized -- just a lump sum for the service + materials)
5. For vendors like CAS Creed (foundation/precast), they provide a detailed line-item breakdown
6. For other vendors, only a total price is returned -- internal team cannot verify individual quantities

**Vendor Takeoff Categories:**
- **Foundation materials**: CAS Creed provides detailed takeoff (blocks, precast, lintels)
- **Trusses**: Truss Direct or Hitek provide price per model/elevation (no itemized breakdown)
- **Lumber**: 84Lumber provides estimate but does NOT do takeoff -- critical gap since no one at Lakeshore knows lumber takeoff
- **Plumbing/Electrical (MEP)**: FOCO and ECOWAN provide service-inclusive quotes with payment splits

### Discrepancy Handling: When Vendor Takeoff Differs from Internal Takeoff

From Batch 5 sessions, the team described their process for handling discrepancies:

**Detection:**
- Internal takeoff (Gabriela's team) produces quantity X for a material
- Vendor takeoff produces quantity Y for the same material
- Compras flags any variance exceeding 10% to Budget team

**Resolution Process:**
1. **Under 10% variance**: Accepted without review (natural measurement differences between methodologies)
2. **10-15% variance**: Budget team (Pedro Henrique) contacts vendor to understand their measurement methodology
3. **Over 15% variance**: Escalated to Samuel Torres; one of three outcomes:
   - Internal takeoff prevails (vendor methodology deemed less accurate)
   - Vendor takeoff prevails (vendor has specialized expertise for their material)
   - New joint measurement performed (rare, for high-value items only)

**Common Sources of Discrepancy:**
- Different waste factor assumptions (internal uses 10%, vendor may use 5% or 15%)
- Different counting methodology for blocks (corner blocks counted differently)
- Vendor includes delivery/logistics in their quantity (e.g., extra material for breakage during transport)
- Rounding differences when converting between units

### Software Validation Findings from Batch 5

Real-world testing with the purchasing team revealed:

**BT Integration Gaps:**
- Zorro (warehouse software) does not integrate with Builder Trend -- all data transferred manually
- PO creation in BT requires manual lookup and data entry even when data exists in Zorro
- No automatic stock level check when creating PO -- team relies on Clauser's spreadsheet updates

**Manual Workarounds Still Required:**
- 12+ spreadsheets open simultaneously for daily purchasing operations
- Distribution of costs per house requires manual calculation across multiple spreadsheets
- Cross-referencing Zorro Sales Orders with BT Purchase Orders is a daily manual reconciliation task
- For custom homes: Camila provides links to purchase from retail stores (Lowes, Amazon, Home Depot) -- Compras buys using those links directly, no formal PO process for these items

**Purchasing Flow for Custom Homes (from Batch 5):**
1. Camila/Projects defines specifications with owner (selections for finishes, fixtures, appliances)
2. Camila creates purchase list with direct links to retail stores (Lowes, Amazon, Home Depot)
3. Compras (Brenda) purchases using provided links
4. Items delivered to warehouse or directly to job site
5. No formal vendor takeoff for retail purchases -- quantities come entirely from internal takeoff

---

## BuilderTrend Job 455 -- Real Data (Supplement)

### Complete Vendor List on Job 455 (28+ Vendors)
| Vendor | Category | Notable Costs |
|--------|----------|---------------|
| CoreCraft Services LLC | Handyman, painting, slab grading, driveway | $2,050+ (8+ POs) |
| AMB Surveying and Mapping | Survey, stake out, lot grading | $1,540 (6 POs) |
| Home Depot | Doors, hardware, shutters, shelves, tiles | $2,580+ (8+ POs) |
| Amazon | Bathroom kits, brackets, mirrors, lockers, fixtures | ~$500+ (7+ POs) |
| Lowes | Door knobs, garden set, shelves, vinyl, paper | $880+ (4+ POs) |
| ONYX GRANITE COUNTERTOPS | Cabinets and countertop | $6,978 (2 bills) |
| IVISION GROUP LLC | Tile + vinyl install + shower glass | $4,204 (3 bills) |
| Cemex | Concrete blocks | $5,713 |
| Del Zotto Concrete LLC | Lintel concrete | $1,693 |
| Truss Direct LLC | Trusses | $6,500 |
| 84 Lumber Company LP | Lumber + AC door | $6,177 |
| Red Twelve LLC | Driveway pavers | $5,053 |
| Strong Quality Garage Door | Garage door installation | $1,850 |
| Leesburg Septic, INC | Sewer connection | $4,600 |
| ETERNAL INSULATION LLC | Insulation | $1,450 |
| J.A.S.H. Services | Lath + stucco | $3,450 |
| AMERICAN STORE LLC | Vinyl material | $2,808 |
| Imeca Web POS | Casings and baseboards | $970 |
| MLI Home Improvements | Door locks, brackets, appliances, front door | ~$575 |
| Rapid Septic Consulting | Septic plan + inspection | $750 |
| Quick eCalcs | Energy calculations | $200 |
| Gizelle Holz & Eliane | Floor plan | $750 |
| Eco One Plumbing Services | Plumbing rough + trim | ~$3,350 |
| Pro-Tek Services | Termite treatment | $266 |
| Richard Job LLC | Blower door test | $175 |
| WC America LLC | Portable toilet | $612 |
| CARMONA LAWN SERVICES | Grass cutting | $50 |
| Costco Wholesale | Electronic lockers, garden set | ~$3 |

### PO Creation Pattern
- 122 POs total over 9 months
- ~14 POs/month average
- Burst activity during roughs and finishing (multiple trades active simultaneously)
- Large monthly material purchase + as-needed replenishment

### Material Sourcing Strategy (from Job 455)
- **Primary retail**: Amazon, Home Depot, Lowes (finish materials, fixtures, hardware)
- **Specialty suppliers**: 84 Lumber, Imeca Web POS, AMERICAN STORE LLC
- **Direct subs**: Cemex (blocks), Truss Direct (trusses), Del Zotto (concrete)
- **Service subs**: Trade-specific (plumbing, electrical, AC, roofing, masonry)

## CPM Construction Sequence -- Purchasing Touchpoints

### Material Ordering Triggers from CPM
| Material | Order Trigger | Delivery Timing |
|----------|--------------|-----------------|
| Foundation Material | After UP Inspection scheduled | After UP Inspection approved |
| Blocks | After slab pouring | 2 days after slab pour (cure time) |
| Precast | Delivery request after schedule | After Masonry Assembly |
| Trusses | Manufacturing request at Foundation Material | ETA = Foundation + 2 weeks; never Monday |
| Lumber | After blocks ordered | To back of property (theft) |
| Windows/Doors | Manufacturing request after Stake House | Before framing |
| Tile Material | Before tile labor scheduled | FASE 4 |
| Vinyl Material | Before vinyl labor scheduled | FASE 4 |
| Trim Set Material | During Cabinets/Granite phase | Before Trim Set starts; after Garage Door + Electronic Locker |
| Plumbing Trim Material | Before plumbing trim scheduled | FASE 4 |
| Electric Trim Material | Before electric trim scheduled | FASE 4 |

### Purchasing Risks from CPM Operational Notes
1. If UP Inspection fails, verify Foundation Material order (materials sitting at site = theft risk)
2. Lumber should be delivered to back of property (theft prevention)
3. Trim Set Material: house must have Garage Door + Electronic Locker first (theft protection)
4. Never request trusses delivery for Monday

## Const App Integration (Supplement)

### Accounts Payable Module (Purchasing Related)
- **Verified POs**: Review payment-ready purchase orders after verification
- **Payment Batches**: Create bulk payment batches for approved POs
- **Authorization**: Multi-level approval for payment batches

### Stock Module (Purchasing Related)
- **Stock Levels**: Cumulative stock requirements from active projects
- **Material Purchases**: Register and track POs with delivery status
- **Material Pickups**: Coordinate supplier pickups; confirm warehouse separation
- **Extraordinary Orders**: Non-standard material requests with justification

### Service Catalog -- Procurement Types
| Procurement | Description | Count |
|-------------|-------------|-------|
| Stocked | In warehouse, standard distribution | 27 items |
| Quoted | Requires vendor quotation each time | 6 items |
| By Sub | Subcontractor provides material + labor | 10 items |
| - (no procurement) | Service/labor only | Remaining |
