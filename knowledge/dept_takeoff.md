# Take-Off - Lakeshore Development

## Visao Geral
- **Missao:** Realizar o levantamento quantitativo de todos os materiais necessarios para construcao a partir das plantas arquitetonicas, alimentando os setores de Orcamento e Compras com dados precisos de quantidades
- **Lider:** Camila Martins (cmartins@lakeshoredevelopmentfl.com) - Gerente de Projetos / Responsavel pelo escritorio de projetos (aprovacao final de takeoff para acabamentos)
- **Equipe:**
  - Gabriela Medeiros (gmedeiros@lakeshoredevelopmentfl.com) - Arquiteta, responsavel principal pelo takeoff de materiais
  - Luana Morais (lmorais@lakeshoredevelopmentfl.com) - Arquiteta, coordena envio para engenheiro
  - Candida Tenorio - Arquiteta no Brasil, takeoff com BlueBeam, quantificacao de materiais
  - Henrique Lima (hlima@lakeshoredevelopmentfl.com) - Arquiteto, renderizacao
  - Victoria Vidal - Arquiteta, renderizacao com Enscape
  - Maria Caroline Elizeu - Nova integrante, usuario final entre arquitetura e software
- **Departamentos relacionados:** Orcamento/Budget, Compras/Purchasing, Scheduling, Permits

## Processos

### Processo 1: Take-Off com BlueBeam (Quantificacao de Materiais)
- **Objetivo:** Quantificar todos os materiais necessarios para construcao a partir do projeto executivo em PDF, gerando lista detalhada para orcamento e compras
- **Responsavel principal:** Gabriela Medeiros / Candida Tenorio
- **Frequencia:** Por modelo novo (spec) ou por projeto (custom)
- **Ferramentas:** BlueBeam, AutoCAD, Software Globin, ChatGPT, Google Drive

**Passo a passo:**
1. Projeto desenvolvido no escritorio de arquitetura -- Responsavel: Camila Martins / equipe -- Ferramenta: AutoCAD, SketchUp
2. Enviar projeto para engenheiro externo -- Responsavel: Luana Morais -- Ferramenta: E-mail
3. Receber projeto executivo (PDF) do engenheiro -- Responsavel: Luana Morais -- Ferramenta: E-mail
4. Abrir PDF no BlueBeam -- Responsavel: Gabriela / Candida -- Ferramenta: BlueBeam
5. Calibrar escala obrigatoriamente usando cotas de referencia -- Responsavel: Gabriela / Candida -- Ferramenta: BlueBeam
6. Tracar areas, linhas e pontos para quantificar itens:
   - Volume de concreto de lajes e vergas
   - Quantitativo de blocos (CMU/lintels)
   - Paredes (drywall)
   - Pisos e revestimentos
   - Bancadas (countertops)
   - Iluminacao pontual
   - Plumbing fixtures
   - Portas e janelas (com direcao de abertura)
   - Acabamentos externos (stucco, painting)
   - Telhado (com angulacao para calcular area de shingles)
   - Trims, mao francesa (brackets)
   -- Responsavel: Gabriela / Candida -- Ferramenta: BlueBeam
7. Compilar resultados manualmente em lista no Word -- Responsavel: Gabriela / Candida -- Ferramenta: Microsoft Word
8. Adicionar 10% de desperdicio a cada item -- Responsavel: Gabriela -- Ferramenta: Word
9. Salvar PDF do takeoff no Drive em pasta acessivel -- Responsavel: Gabriela -- Ferramenta: Google Drive
10. Para revisoes: arquivo antigo vai para pasta "revision", novo substitui -- Responsavel: Gabriela -- Ferramenta: Google Drive

**Inputs:** Projeto executivo em PDF (do engenheiro via Luana); floor plan; design book; spec sheet
**Outputs:** Lista quantitativa de materiais (PDF no Drive) para Budget e Compras
**Observacoes:** Para spec homes, takeoff feito uma vez por modelo e raramente revisado. Para custom homes, cada projeto requer takeoff unico criado do zero. Funcao paga do BlueBeam para linkar com planilhas nunca foi utilizada.

### Processo 2: Takeoff de Blocos e Materiais sem Takeoff do Fornecedor
- **Objetivo:** Levantar quantidade de blocos e materiais cujo fornecedor NAO faz takeoff, usando ferramentas internas
- **Responsavel principal:** Gabriela Medeiros
- **Frequencia:** Por projeto/modelo
- **Ferramentas:** Software Globin, ChatGPT (IA), Planilhas Excel

**Passo a passo:**
1. Identificar materiais onde fornecedor nao faz takeoff (blocos, concreto de verga) -- Responsavel: Gabriela -- Ferramenta: [processo interno]
2. Fazer levantamento de quantidade usando IA (ChatGPT) e software Globin (desenho sobre planta) -- Responsavel: Gabriela -- Ferramenta: Globin, ChatGPT
3. Calcular componentes padrao: regular blocks, lintel blocks, rough blocks, blocos 3/4, blocos de coluna, areia, cimento, frete, taxa ambiental -- Responsavel: Gabriela -- Ferramenta: Planilhas Excel
4. Repassar quantidades para equipe de Budget para calculo de custo (quantidade x preco unitario) -- Responsavel: Gabriela -- Ferramenta: Planilhas Excel, Google Drive

**Inputs:** Planta da casa (floor plan); dados do projeto
**Outputs:** Quantidade de blocos e materiais para equipe de Budget calcular custo
**Observacoes:** Variacao natural de ~10% na quantidade (diferentes subs montam de formas diferentes). Mauricio (Scheduling) pode precisar alterar quantidade no ato do pedido. Sobras de material entre casas sao aproveitadas.

### Processo 3: Vendor Takeoff (Takeoff pelo Fornecedor)
- **Objetivo:** Gerenciar o processo quando o fornecedor faz seu proprio takeoff a partir da planta, retornando cotacao fechada
- **Responsavel principal:** Gabriela Medeiros (marcacao) / Pedro Henrique Cordeiro (cotacao)
- **Frequencia:** Por projeto/modelo, para servicos especificos
- **Ferramentas:** E-mail, Google Drive, Software Lakeshore (em desenvolvimento)

**Passo a passo:**
1. Identificar servicos onde sub faz seu proprio takeoff (foundation materials, precast, trusses) -- Responsavel: Gabriela -- Ferramenta: [processo interno]
2. Marcar item como "Enable Vendor Takeoff" na lista de takeoff -- Responsavel: Gabriela -- Ferramenta: Planilhas Excel
3. Enviar planta do projeto para o fornecedor -- Responsavel: Pedro Henrique / Ana Helena -- Ferramenta: E-mail
4. Fornecedor retorna com preco total baseado em seu proprio levantamento -- Responsavel: Fornecedor (externo) -- Ferramenta: E-mail
5. Registrar cotacao recebida -- Responsavel: Pedro Henrique -- Ferramenta: Planilhas Excel

**Inputs:** Planta do projeto (floor plan, projeto executivo)
**Outputs:** Cotacao fechada do fornecedor para inclusao no budget
**Observacoes:** Para servicos como foundation e precast (CAS Creed), nao e necessario detalhar itens individuais. Equipe compara takeoff de um fornecedor (CAS Creed) com tabela de precos de outro (CMEX) -- trabalho manual de encontrar equivalencias entre itens.

### Processo 4: Gestao de Documentos e Versionamento de Plantas
- **Objetivo:** Manter documentos de projeto organizados e atualizados, garantindo que todas as equipes trabalhem com a versao mais recente
- **Responsavel principal:** Luana Morais / Gabriela Medeiros
- **Frequencia:** Continua
- **Ferramentas:** Google Drive, BlueBeam

**Passo a passo:**
1. Fazer upload de documentos (floor plan, design book, spec sheet) em pasta padronizada -- Responsavel: Luana / Gabriela -- Ferramenta: Google Drive
2. Para atualizacoes: mover versao antiga para pasta "revision" -- Responsavel: Gabriela -- Ferramenta: Google Drive
3. Substituir pelo novo documento -- Responsavel: Gabriela -- Ferramenta: Google Drive
4. Comunicar equipe de Budget sobre atualizacao [inferido - processo manual e falho] -- Responsavel: Gabriela -- Ferramenta: [manual, sem ferramenta padronizada]

**Inputs:** Projetos finalizados ou revisados
**Outputs:** Documentos atualizados acessiveis no Drive
**Observacoes:** Dificuldade de encontrar versao mais atualizada em drives compartilhados e uma dor recorrente. Software em desenvolvimento promete versionamento automatico com notificacao.

## Dores e Problemas Conhecidos
- **CPUs da Lakeshore nao rodam os programas de arquitetura**: pouca potencia de video; Candida e Gabriela usam computadores pessoais
- **Compilacao manual da lista de takeoff**: resultados do BlueBeam compilados manualmente em Word (processo lento e propenso a erros)
- **Funcao de integracao do BlueBeam nao utilizada**: funcao paga para linkar com planilhas nunca foi explorada
- **Equipe de projetos trabalha isolada**: pouca interacao com outros setores
- **Volatilidade do takeoff para customs**: clientes mudam definicoes durante obra (tile em vez de vinil, etc.)
- **Mudancas de takeoff nao notificam automaticamente equipe de budget**: falta de integracao entre setores
- **Takeoff deveria ser feito no inicio da obra com PM e supervisores**: atualmente e tardio no processo
- **Nomenclatura de itens nao correspondente entre fornecedores diferentes**: CAS Creed vs CMEX requer mapeamento manual
- **Dependencia de projeto de engenharia finalizado antes do takeoff**: pode atrasar todo o fluxo
- **3.500 itens para atualizar manualmente quando modelos mudam**: necessidade de mecanismo de duplicacao/template

## Dependencias
- **Recebe de:** Engenheiro externo -> projeto executivo (PDF); Escritorio de Projetos (Camila) -> floor plan, design book, spec sheet; Sub de trusses -> trusses layout (necessario para takeoff preciso)
- **Entrega para:** Orcamento/Budget (Felipe, Pedro, Ana Helena) -> quantidades de materiais para cotacao e budget; Compras/Purchasing (Brenda) -> lista de materiais para compra; Scheduling (Mauricio) -> informacoes de materiais e quantidades a partir da fase de blocos; Permits -> floor plan e documentos para aplicacao de permit

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- [Catalogo de Dores](07_CATALOGO_DORES.md)
- [Fluxo Spec Home](05_FLUXO_SPEC_HOME.md)
- [Fluxo Custom Home](06_FLUXO_CUSTOM_HOME.md)
- [Glossario de Termos](03_GLOSSARIO.md)
- **Departamentos relacionados:**
  - [Escritorio de Projetos](dept_escritorio_projetos.md) — fornece floor plan, design book, spec sheet
  - [Orcamento](dept_orcamento.md) — recebe quantidades de materiais para cotacao e budget
  - [Compras](dept_compras.md) — recebe lista de materiais para compra
  - [Scheduling](dept_scheduling.md) — recebe informacoes de materiais e quantidades
  - [Permits](dept_permits.md) — recebe floor plan e documentos para aplicacao de permit

## Key Glossary Terms

> Terms from [Glossario de Termos](03_GLOSSARIO.md) most relevant to the Takeoff department.

- **Take-Off (Takeoff)** / **Levantamento Quantitativo**: Detailed material quantity survey from project plans -- central to budget and purchasing
- **Cost Code** / **Codigo de Custo**: Numeric code categorizing each cost type/service -- organizes takeoff items sequentially
- **BlueBeam** / **BlueBeam (software)**: Engineering software for measuring areas, volumes, and quantities from PDF plans
- **Cubic Yard** / **Jarda Cubica**: Volume unit for concrete (1 cu yd = ~0.76 m3) -- base for concrete cost calculation
- **Square Foot (sq ft)** / **Pe Quadrado**: Area unit (1 sq ft = ~0.093 m2) -- base for cost-per-area estimates
- **Stocked** / **Em Estoque**: Material in Lakeshore warehouse available for immediate distribution
- **Non-stock** / **Material Nao-estocado**: Material purchased for specific project, not in regular inventory
- **Quoted** / **Cotado**: Material/service requiring vendor quotation -- different from stocked and by-sub items
- **By Sub** / **Fornecido pelo Subcontratado**: Material provided directly by the sub (e.g., drywall sub supplies material + labor)
- **Enable Vendor Takeoff** / **Habilitar Takeoff pelo Fornecedor**: Software feature transferring takeoff responsibility to vendor
- **Vendor Takeoff** / **Levantamento pelo Fornecedor**: When vendor does their own quantity survey from plans (e.g., foundation, precast)
- **BID** / **Proposta de Preco**: Price proposal from vendor -- takeoff feeds the bidding process with accurate quantities

## AI-Assisted Takeoff (Batch 3)

### Gabriela's Use of AI and Software Tools

From Batch 3 interviews (24/09/2025), Gabriela Medeiros described how the takeoff team uses AI and specialized software to assist with quantity estimation:

**ChatGPT for Estimation:**
- Used as a calculation assistant for quantity estimation, not as a replacement for manual verification
- Helps with unit conversion (e.g., square feet to square meters, cubic yards to cubic feet)
- Assists in interpreting complex engineering drawings and calculating volumes
- Gabriela uses it alongside Software Globin for cross-verification of quantities

**Software Globin Workflow:**
1. Import construction plans (PDFs from engineer) into Globin
2. Software auto-detects certain quantities from the drawings (areas, lengths, counts)
3. Gabriela performs manual review of every auto-detected quantity -- no blind trust in software output
4. Cross-reference Globin results with BlueBeam measurements for accuracy
5. Final quantities compiled manually into Word document (the compilation step is the bottleneck)

**Common Estimation Errors and Correction Process:**
- **Scale calibration errors**: If BlueBeam calibration uses wrong reference dimension, all measurements are proportionally wrong. Must re-calibrate and re-measure.
- **Omitted items**: Complex floor plans may cause overlooked areas (e.g., closet interiors, covered porches). Review against spec sheet catches these.
- **Unit mismatch**: Concrete quoted in cubic yards, blocks in units, drywall in square feet -- conversion errors are common when compiling the final Word list.
- **Correction protocol**: When an error is found post-compilation, the old takeoff goes to "revision" folder, new corrected version replaces it. No automatic notification to Budget team (manual gap).

### Spec vs Custom Takeoff Differences
- **Spec homes**: Takeoff done once per model, rarely revised. Template quantities reused across all houses of that model. Only updated when model design changes (e.g., new Palmer elevation).
- **Custom homes**: Every project requires a unique takeoff from scratch. Client changes during construction (tile instead of vinyl, different countertop material) require partial re-takeoff of affected categories only.

## Vendor Takeoff Validation (Batch 5)

### Cross-Reference Internal vs Vendor Quantities

From Batch 5 interviews (12/03/2026 - 23/03/2026), the team described how vendor takeoffs are validated against internal quantities:

**Vendor Takeoff Process:**
1. Item marked as "Enable Vendor Takeoff" in the software -- transfers responsibility to vendor
2. Vendor receives project plans and performs their own quantity survey
3. Vendor returns with a total price (not always itemized)
4. Internal team compares vendor's total against internal estimate for reasonableness

**CAS Creed vs CMEX Nomenclature Challenge:**
- CAS Creed (CAS CR) provides takeoff for foundation and precast materials
- CMEX provides competing price tables using completely different item names
- Example: CAS Creed item "8x8x16 regular" may correspond to CMEX item "Standard CMU Block 8-inch"
- Team must manually map item-by-item between the two nomenclature systems to compare prices
- This is a fully manual process currently -- no equivalence table exists in the system

**Tolerance Thresholds for Quantity Differences:**
- **Under 10% variance**: Accepted as normal (different subs count differently, e.g., block quantities)
- **10-15% variance**: Flagged for review by Budget team (Felipe/Pedro) -- may indicate different measurement methodology
- **Over 15% variance**: Escalated to Samuel Torres for decision -- vendor may be measuring incorrectly or internal takeoff may have errors
- **Zero-tolerance items**: Foundation concrete quantities must match exactly (structural safety requirement)

**Escalation When Discrepancy Exceeds 10%:**
1. Takeoff team (Gabriela) documents the discrepancy with both quantities and measurement methodology
2. Budget team (Pedro Henrique) contacts the vendor for clarification on their methodology
3. If vendor cannot justify the difference, internal takeoff prevails
4. If vendor's methodology is superior (e.g., they use specialized software for their material), adopt their quantity
5. Samuel Torres makes final call on disputed quantities above 15% variance

---

## BuilderTrend Job 455 -- Real Data

### Job 455 Cost Codes and Material Categories
Job 455 used the standard 19 cost code structure. The following material quantities are directly relevant to takeoff:

**Foundation Materials (Cost Code 5)**:
- REBAR #5 x 20' GR.40 (ASTM A615): 31 units
- REBAR DOWEL #5 4'x1': 59 units
- 2-BAR CHAIR: 100 units
- Red Tape 48mm x 36yd: 4 units
- POLY 6 MIL (vapor barrier): included

**Precast (Cost Code 5.5)**:
- LINTEL-U 8X8X4-6: 7 units
- 37" SILL WIND RESIST FLUSH: 7 units
- #5 GR 60 REBAR 20-0: 19 units
- #5 GR 60 DOWEL 1-0X9-0: 59 units
- #5 GR 60 CORNER BAR 2-6X2-6: 9 units
- FORMMAT LINTEL SCRN 6"X100': 3 units

**Masonry (Cost Code 8)**: Blocks from Cemex ($5,713), lintel concrete from Del Zotto ($1,693)

**Roofing (Cost Code 9)**:
- Trusses: Truss Direct LLC ($6,500)
- Lumber: 84 Lumber Company LP ($6,177)
- Architectural Shingles: 2,722.88 sqft

**Windows (Cost Code 10)**: $22,368 -- largest single trade on Job 455
- Single-Hung Window 36"x62" vinyl white: 7 units
- Single-Hung Window 52"x62" vinyl white: included
- Entry Door 36"x96" Right Hand: 1 unit
- Sliding Glass Door 72"x80": 1 unit

**Doors (Cost Code 11)**:
- Interior Door 32"x80" LH: 4 units
- Interior Door 32"x80" RH: 4 units (1 fire-rated)
- Bifold Closet 24"x80": 3 units
- Bifold Closet 30"x80": 6 units
- Baseboard: 512 linear feet
- Window Sill: 48 linear feet
- Casings Doors: 544 linear feet
- Lock Knob: 6, Passage Knob: 2, Conventional Stop Door: 9

**Plumbing Fixtures (Cost Code 6)**:
- Toilet: 2, Bath Sink: 3, Bath Faucet: 3, Mirror: 3
- Bathtub Freestanding: 1, Kitchen Sink: 1, Shower: 1

**Electrical Fixtures (Cost Code 7)**:
- Exterior Coach Light: 3
- Recessed Light: 18
- Vanity Light: 3
- Pendant Light: 3
- Vintage Lamp: 13

**Finishing (Cost Code 13)**:
- Wall Tile Shower: 179 sqft, Floor Tile Shower: 14.25 sqft
- Countertop: 76.15 sqft, Backsplash: 24 sqft
- Engineered Wood Flooring: 1,544.9 sqft
- Cabinets & Countertop: $6,978 (ONYX GRANITE)
- Vinyl material: $2,808 (AMERICAN STORE LLC)

**Exterior (Cost Code 14)**:
- Driveway Pouring: 18 cubic yards
- Brackets 16"x14": 4, Shutters 12"x63": 2

### Job 455 Vendor Takeoff Examples
| Material | Vendor Who Did Takeoff | Internal Cross-Check |
|----------|----------------------|---------------------|
| Foundation/Precast | Cast Crete (8 items) / Cemex (12 items) | Internal BlueBeam measurement |
| Trusses | Truss Direct LLC | Engineering package from truss engineer |
| Blocks | Cemex | Gabriela's Globin + ChatGPT estimation |

### PO Categories Mapped to Takeoff Cost Codes
| Takeoff Category | PO Count (est.) | Total Cost |
|-----------------|-----------------|------------|
| Pre-construction (survey, plans) | 7 | ~$3,240 |
| Land prep | 5 | ~$2,510 |
| Structural materials | 5 | ~$21,783 |
| Finishing materials | 9+ | ~$5,300 |
| Fixtures/hardware | 6+ | ~$2,400 |
| Landscaping | 4+ | ~$800 |
| Labor services | 10+ | Various |
| Utilities/fees | 8 | Various |

## CPM Construction Sequence -- Takeoff Touchpoints

### Material Timing Dependencies from CPM
1. **Foundation Material**: Ordered after UP Inspection scheduled; must arrive AFTER UP Inspection approval. If UP fails, verify order status to avoid theft risk.
2. **Trusses Manufacturing Request**: ETA = Foundation Material ETA + 2 weeks; never request for Monday delivery
3. **Blocks**: Must arrive 2 days AFTER slab pouring (concrete cure time -- materials stored on slab)
4. **Lumber**: Should be delivered to back of property to reduce theft risk
5. **Trim Set Material**: Must arrive during final Cabinets/Granite phase, BEFORE Trim Set starts. House must have Garage Door + Electronic Locker first (theft protection)
6. **Tile Material / Vinyl Material**: Must arrive before Tile/Vinyl labor is scheduled (CPM FASE 4)
7. **Plumbing Trim Material / Electric Trim Material**: Delivery timed to match trim phase scheduling

### CPM Sub-Phase Groups Affecting Takeoff Sequencing
| Sub-Phase | Materials to Quantify Together |
|-----------|-------------------------------|
| 2.1 (Early roughs) | Plumbing rough, AC rough, electrical rough -- all inspection-gated |
| 2.2 (Interior finish) | Cabinets/Granite, Plumbing Trim, Drywall Texture |
| 3.1 (Exterior finish) | Stucco, Shingles, Exterior Paint |
| 3.2 (Interior finish) | Interior Paint, Tile, Vinyl |

## Const App Integration

### Take-Off Module in Const App
- **URL**: /quotation/take_off
- **Model 1774 Stats**: 19 cost codes, 33 services, 74 components
- **Supply Types**: Stocked (27 items), Quoted (6 items), By Sub (10 items)
- **Plans Completed**: 17/16 (status: IN PROGRESS)
- **Living Area**: 1,774 sqft

### Relevant Service Catalog Codes for Takeoff
| Code | Service | Nature | Procurement |
|------|---------|--------|-------------|
| FND-001 | Foundation Material | Material | Stocked |
| MAS-001 | Blocks | Material | Stocked |
| MAS-002 | Precast | Material | Quoted |
| ROF-001 | Trusses | Material | Quoted |
| ROF-002 | Lumber | Material | Stocked |
| ROF-007 | Shingles | Material | Stocked |
| WIN-001 | Windows and Exterior Doors | Material | Quoted |
| WIN-002 | Windows Material | Material | Stocked |
| DOR-001 | Interior Doors and Trim Set Material | Material | Stocked |
| FIN-004 | Insulation | Material | Stocked |
| FIN-007 | Flooring | Material | Stocked |
| FIN-008 | Tile Material | Material | Stocked |
| FIN-009 | Vinyl Material | Material | Stocked |
| FIN-012 | Cabinets and Countertop | Material | Stocked |
| PLM-002 | Plumbing Fixtures | Material | Stocked |
| ELC-002 | Electrical Fixtures | Material | Stocked |
