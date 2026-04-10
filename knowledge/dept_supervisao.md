# Supervisao / Field - Lakeshore Development

## Visao Geral
- **Missao:** Acompanhar e garantir a qualidade da execucao dos servicos em campo, verificando obras diariamente, resolvendo problemas operacionais, apoiando a equipe de scheduling e garantindo que os servicos estejam conforme especificacoes antes de liberar pagamento
- **Lider:** Moises - Supervisor / Gerente
- **Equipe:**
  - Joao Paulo Valenca (cpm19@lakeshoredevelopmentfl.com) - Supervisor
  - Daniel - Supervisor (casas fase avancada/warranty)
  - Charles - Monitor (novo)
  - Luigi - Monitor (mais experiente)
- **Departamentos relacionados:** Scheduling, Financeiro, Inspecao, Warranty, Compras, Budget/Takeoff, QPS (Quality Performance Standards)

## Processos

### Processo 1: Rotina Diaria de Supervisao
- **Objetivo:** Acompanhar o progresso de todas as casas sob responsabilidade, identificar problemas e priorizar acoes corretivas
- **Responsavel principal:** Joao Paulo Valenca
- **Frequencia:** Diaria
- **Ferramentas:** Dashboard de Rost (painel de acompanhamento), Citros Yocala (ferramenta de acompanhamento), Planilha de acompanhamento (filtros por modelo e condado), Builder Trend (duvidas pontuais)

**Passo a passo:**
1. Checar lista de reports -- prioridade #1 do dia (obras podem estar paradas) -- Responsavel: Joao Paulo -- Ferramenta: Dashboard de Rost
2. Checar inspecoes reprovadas -- precisam ser resolvidas imediatamente -- Responsavel: Joao Paulo -- Ferramenta: Dashboard de Rost
3. Usar dash de acompanhamento -- filtrar por modelo e condado, ordenar do mais antigo -- Responsavel: Joao Paulo -- Ferramenta: Planilha de acompanhamento
4. Verificar status de cada casa usando ferramenta Citros Yocala -- Responsavel: Joao Paulo -- Ferramenta: Citros Yocala
5. Identificar proximo passo para cada casa baseado nos processos ja feitos -- Responsavel: Joao Paulo -- Ferramenta: [analise operacional]
6. Criar rotas de visita tentando atender o maximo de casas por dia -- Responsavel: Joao Paulo -- Ferramenta: [planejamento de rota]
7. Apoiar schedule team quando necessario (dar "empurraozinho" dependendo do operador) -- Responsavel: Joao Paulo -- Ferramenta: WhatsApp, Telefone

**Inputs:** Dashboard com status de casas; lista de reports; inspecoes reprovadas; notificacoes de Scheduling
**Outputs:** Problemas identificados e encaminhados; verificacoes de campo realizadas; apoio ao Scheduling
**Observacoes:** Nao trabalham mais com rotas fixas -- trabalho baseado em lista de casas e demandas. Nao consegue ver 50+ casas por dia pelo volume.

### Processo 2: Verificacao de Servicos e Controle de Qualidade
- **Objetivo:** Verificar in loco se os servicos executados pelos subcontratados estao conforme especificacoes antes de liberar para pagamento ou inspecao
- **Responsavel principal:** Joao Paulo Valenca / Monitores (Charles, Luigi)
- **Frequencia:** Diaria (por servico concluido)
- **Ferramentas:** Builder Trend (checklist), Fotos, Visita presencial

**Passo a passo:**
1. Receber notificacao ou verificar que servico foi concluido por sub -- Responsavel: Supervisor/Monitor -- Ferramenta: Slack, WhatsApp
2. Visitar obra para inspecao visual do servico -- Responsavel: Supervisor/Monitor -- Ferramenta: Visita presencial
3. Verificar conformidade com especificacoes -- Responsavel: Supervisor/Monitor -- Ferramenta: [conhecimento tecnico]
4. Se conforme: preencher checklist done no Builder Trend (GATILHO DE PAGAMENTO) -- Responsavel: Monitor -- Ferramenta: Builder Trend
5. Se nao conforme: notificar Scheduling para rework com o sub -- Responsavel: Supervisor -- Ferramenta: WhatsApp, Slack

**Inputs:** Servico executado pelo sub; especificacoes do projeto
**Outputs:** Checklist done (libera pagamento) ou notificacao de rework
**Observacoes:** ALERTA CRITICO: Checklist done = gatilho de pagamento. Sub pago nao volta para arrumar. Novos monitores precisam ser treinados sobre esse impacto. Inputs dos monitores com falhas historicas (falta de conhecimento resultava em dados incorretos).

### Processo 3: Calculo de Loads e Verificacao de Fundacao
- **Objetivo:** Calcular os loads (cargas de terra) necessarios para a fundacao e verificar se a elevacao do pad esta correta
- **Responsavel principal:** Supervisores
- **Frequencia:** Por casa (na Fase 1)
- **Ferramentas:** Equipamento de campo (medicao), Builder Trend

**Passo a passo:**
1. Apos stake house, ir ao local para calculo de loads -- Responsavel: Supervisor -- Ferramenta: Equipamento de campo
2. Medir e calcular quantidade de material necessario -- Responsavel: Supervisor -- Ferramenta: Equipamento de medicao
3. Informar Scheduling sobre quantidade de loads -- Responsavel: Supervisor -- Ferramenta: WhatsApp
4. Apos entrega dos loads e pad, verificar se elevacao esta correta (avaliacao qualitativa) -- Responsavel: Supervisor -- Ferramenta: Visita presencial

**Inputs:** Stake house concluido; dados topograficos
**Outputs:** Calculo de loads para Scheduling; aprovacao de elevacao do pad
**Observacoes:** GARGALO CRITICO: Demora no calculo por falta de equipamentos especificos. Workaround: solicitar fotos dos loads entregues para pedir pad antecipadamente.

### Processo 4: Resolucao de Problemas em Campo
- **Objetivo:** Resolver problemas operacionais que surgem durante a construcao, coordenando com subs e departamentos internos
- **Responsavel principal:** Joao Paulo Valenca / Moises
- **Frequencia:** Diaria (sob demanda)
- **Ferramentas:** WhatsApp, Telefone, Builder Trend

**Passo a passo:**
1. Identificar problema durante visita ou por notificacao -- Responsavel: Supervisor/Monitor -- Ferramenta: Visita presencial, Slack
2. Avaliar gravidade e impacto no cronograma -- Responsavel: Supervisor -- Ferramenta: [analise operacional]
3. Contatar sub responsavel para correcao -- Responsavel: Supervisor -- Ferramenta: WhatsApp, Telefone
4. Coordenar com Scheduling para reagendamento se necessario -- Responsavel: Supervisor -- Ferramenta: WhatsApp
5. Acompanhar resolucao e registrar no Builder Trend -- Responsavel: Supervisor -- Ferramenta: Builder Trend
6. Para problemas graves: escalar para Moises ou Samuel -- Responsavel: Supervisor -- Ferramenta: WhatsApp

**Inputs:** Problemas identificados em campo; notificacoes de inspecoes reprovadas
**Outputs:** Problemas resolvidos; registros de resolucao; reagendamentos quando necessario
**Observacoes:** Distancia geografica + volume de casas dificulta resolucao rapida. Supervisores autorizados a solicitar reparos, mas frequentemente nao criam PO (causando problema para Financeiro).

## Dores e Problemas Conhecidos
- **Ferramentas unilaterais**: Dashboards sao somente leitura, nao permitem anotacoes ou interacao
- **Falta de visualizacao em timeline/barra de progresso**: Com cores indicativas (vermelho=atrasado, amarelo=em progresso, verde=concluido)
- **Inconsistencia de dados no Kanban anterior**: Kanban 1 e 2 falharam por problemas de consistencia
- **Inputs dos monitores com falhas**: Falta de conhecimento resultava em dados incorretos (ex: marcar problema de software como problema de telhado)
- **Inputs duplicados**: Internet ruim causa duplicacao de dados
- **Fotos nao sobem**: 99% das vezes as fotos anexadas nao sobem completamente
- **Internet ruim no campo**: Dificulta uso de qualquer sistema pesado
- **Volume de casas vs tempo**: Nao consegue olhar 50+ casas no dia
- **Supervisores solicitam reparos mas nao criam PO**: Causa problema no Financeiro (invoices sem PO)
- **Comunicacao campo-escritorio deficiente**: Field deveria participar da revisao de projetos

## Dependencias
- **Recebe de:** Scheduling -> informacoes de agendamento, servicos a verificar; Inspecao -> resultados de inspecoes (aprovadas/reprovadas); QPS (Don/Fortine) -> padroes de qualidade
- **Entrega para:** Scheduling -> confirmacao de elevacao do pad, calculo de loads, apoio operacional; Financeiro -> checklist done (gatilho de pagamento); Inspecao -> verificacao previa antes de agendar inspecao; Warranty -> verificacao de reparos em casas (Daniel)

---

## Guia de Construcao (Fonte: Drive Lakeshore)

### Doc-Box — Documentos Obrigatorios no Lote

Todo projeto de construcao deve ter um doc-box instalado na frente do terreno antes do inicio das obras. A caixa deve estar visivel, acessivel e nao pode obstruir a locomocao de trabalhadores ou o desembarque de materiais. Uma placa "PRIVATE PROPERTY" deve ser fixada no mesmo suporte.

**Documentos dentro do doc-box (Poinciana):**

| Qtd | Documento | Descricao |
|-----|-----------|-----------|
| 1 copia | NOC / Notice of Commencement | Proprietario autoriza o General Contractor a construir |
| 2 copias | Energy Calculation | Calculos tecnicos de fluxo de ar e refrigeracao (1 com carimbo do county, 1 sem) |
| 2 copias | Truss Engineering | Planta das tesoueiras do telhado (1 com carimbo, 1 sem) |
| 1 copia | Site Plan (Survey) | Esboco tecnico com limites do terreno e da construcao |
| 2 copias | Floor Plan | Planta com todas as fases da casa (1 com carimbo, 1 sem) |
| 1 copia | DBPR | Descricoes tecnicas dos materiais usados na construcao |
| 1 copia | Building Permit | Permissao do county para construir |
| 1 copia | Bora Care | Documento tecnico do tratamento contra cupim nas madeiras |

**Regra de organizacao:**
- NOC, Survey e Bora Care: pregados na parede interna do doc-box
- Energy Calc, Truss Engineering, Floor Plan e DBPR (com carimbos): dentro de pasta plastica (para o inspetor)
- Copias sem carimbo: dentro do doc-box para uso dos empreiteiros

---

### Sequencia de Construcao — Visao Geral

| Etapa | Nome | Descricao Resumida |
|-------|------|--------------------|
| 1 | Set Doc-Box | Instalar caixa de documentos na frente do lote |
| 2 | Portable | Solicitar banheiro quimico antes da chegada das equipes |
| 3 | Stake the Lot | Surveyor instala estacas para delimitar os limites da propriedade |
| 4 | Clearing of the Lot | Remocao de arvores, vegetacao e entulho (pneus ficam com Lakeshore) |
| 5 | Stake House and Elevation | Surveyor demarca esquadrejamento da casa e define elevacao do terreno |
| 6 | Request 811 DIG | Sunshine 811 demarca redes subterraneas (agua, esgoto, energia, gas) |
| 7 | Fill and Grading | Contratista coloca/remove terra e compacta o solo |
| 8 | Wood Dumpster | Instalar cercado de plywood para armazenar entulho inicial |
| 9 | Schedule Compact Test | Empresa credenciada certifica compactacao do solo; emite certificado para doc-box |
| 10 | Hub & Tack | Surveyor marca entradas e saidas da casa no pad compactado |
| 11 | Forms | Contratista de concretagem instala estacas e tabuas conforme planta |
| 12 | Underground Plumbing | Encanamento de subsolo (agua quente/fria/esgoto); pressao 60-120 PSI |
| 13 | Underground Plumbing Inspection | Inspetor verifica tubulacao, conexoes, espuma de protecao e pressao |
| 14 | Sewer Tap Inspection | Inspetor verifica tubulacao de esgoto ate tanque septico ou rede publica |
| 15 | Slab Preparation | Cobrir tubulacoes, instalar plastico de isolamento, ferragem e red caps |
| 16 | Electrical Underground | Eletricista instala conduite para a ilha da cozinha durante prep do slab |
| 17 | Slab Inspection | Inspetor verifica isolamento, aterramento e ferragem |
| 18 | Slab Pouring | Concretagem do contrapiso (Cemex + bombeamento + equipe de acabamento) |
| 19 | Block Setting | Construcao das paredes de bloco (necessita agua disponivel no lote) |
| 20 | Lintel Inspection | Inspetor verifica juncao de ferragem do slab com colunas e viga de amarracao |
| 21 | Layout for Trusses | Framing marca posicionamento dos straps no topo das paredes |
| 22 | Lintel Pouring | Preenchimento de colunas e vigas; fixacao dos straps em concreto fresco |
| 23 | TUG Meter (Meter Can) Installation | Eletricista instala caixa metalica para medidor de energia |
| 24 | Trusses and Full Framing | Instalacao do madeiramento do telhado, paredes e divisorias |
| 25 | TUG Inspection | Inspetor verifica instalacao correta do meter can |
| 26 | Wall Sheathing Inspection | Inspetor verifica parte triangular do telhado (gable em madeira) |
| 27 | Roof Sheathing Nail Off | Inspetor verifica plywood, presilhas, pregos e integridade do telhado |
| 28 | Dry-in & Flashings | Contratista de roof instala manta termica sobre o plywood |
| 29 | Rough HVAC | Instalacao de tubulacao de ar condicionado e exaustores |
| 30 | Set Windows and Exterior Doors | Instalacao de janelas e portas externas |
| 31 | Rough Plumbing | Tubulacao interna (agua quente/fria, esgoto, ventilacao); pressao 60-120 PSI |
| 32 | Felt Paper and Lathe Installation | Stucco instala esquadrias de fixacao e trim externo |
| 33 | Rough Electrical | Instalacao eletrica interna (quadro, tomadas, spots, sensores, campainha, TV) |
| 34 | Roof Shingles Installation | Instalacao das telhas de shingle |
| 35 | Stucco Finishing | Reboco de todas as paredes externas com massa cimenticia e chapisco |
| 36 | Rough-Framing Inspection | Inspetor verifica madeiramento, tesoueiras, straps, bolts e red heads |
| 37 | Rough-Mechanical Inspection | Inspetor verifica rede de tubos de HVAC conforme energy calculation |
| 38 | Rough-Electrical Inspection | Inspetor verifica sistema eletrico completo conforme projeto |
| 39 | Rough-Plumbing Inspection | Inspetor verifica sistema hidraulico; pressao 60-120 PSI |
| 40 | Insulation Installation | Instalacao de insulation nas paredes e placas de ventilacao do attico |
| 41 | Drywall Installation | Instalacao de drywall (areas molhadas recebem Durock); emassamento e textura |
| 42 | Interior Painting | Pintura interna |
| 43 | Exterior Painting | Pintura externa |
| 44 | Tile Installation | Instalacao de piso e azulejo |
| 45 | Soffit Installation | Instalacao de beiral de aluminio para proteger madeira externa do telhado |
| 46 | Cabinets & Granite | Instalacao de gabinetes da cozinha e banheiros com granito |
| 47 | Rough Grade & Culvert | Preparacao do solo para driveway; instalacao do tubo de drenagem (culvert) |
| 48 | Driveway Cut | Madeiramento para concretagem da driveway |
| 49 | Driveway Pre-Pour Inspection | Inspetor verifica layout e culvert conforme plano |
| 50 | Door Trims & Baseboard | Instalacao de portas, fechaduras, rodapes, sanca da ilha e window seal |
| 51 | HVAC Trim Set | Instalacao de grades de ar, termostato, exaustores e maquinas interna/externa |

---

### Responsabilidades de Campo — Pontos Criticos

- **Doc-box caido ou no chao**: Equipe Lakeshore deve reinstalar e reposicionar imediatamente
- **Agua no lote no Block Setting**: Lakeshore deve providenciar acesso a agua caso nao exista no terreno
- **Banheiro quimico**: Deve estar disponivel antes da chegada de qualquer equipe; empresa responsavel pela manutencao e remocao
- **Compact Test**: Certificado deve ficar disponivel no doc-box para o inspetor
- **Bathtub Protection**: Equipe Lakeshore instala capa protetora na banheira para evitar danos ate o final da obra
- **Wood Spray Treatment**: Certificado de aplicacao de produto contra cupim deve ser deixado no lote para o inspetor
- **Pneus no terreno**: Contratista de clearing NAO remove pneus — responsabilidade da Lakeshore
- **Checklist done no Builder Trend**: GATILHO DE PAGAMENTO — marcar somente apos verificacao rigorosa; sub pago nao volta para correcao

---

## Descricao de Cargo Formal (Fonte: Drive Lakeshore)

### Field Monitor

- **Setor:** Field — Monitor
- **Local de trabalho:** Campo (obras)
- **Objetivo do cargo:** Garantir que a casa seja entregue dentro do prazo de 4 meses, atendendo os criterios de qualidade exigidos pela empresa
- **Principais responsabilidades:**
  - Identificar problemas relacionados ao dia a dia da obra
  - Realizar rota e acompanhar o andamento dos processos
  - Gerar reports quando o servico nao estiver dentro do padrao determinado pela empresa
  - Realizar registros fotograficos e atualizar os sistemas
  - Identificar se o servico foi concluido ou nao
  - Executar checklist de conformidade de processos

---

### Field Supervisor

- **Setor:** Field — Supervisor
- **Local de trabalho:** Campo (obras)
- **Objetivo do cargo:** Garantir que a casa seja entregue dentro do prazo de 4 meses, atendendo os criterios de qualidade exigidos pela empresa
- **Principais responsabilidades:**
  - Identificar e resolver problemas relacionados ao dia a dia da obra
  - Gerenciar reports referentes as obras
  - Registrar problemas e causas (FMEA)
  - Acompanhar inspecoes e reinspecoes
  - Treinar monitores (parcialmente)
  - Controlar qualidade da obra
  - Atualizar os sistemas
  - Realizar medicoes (ex.: abertura de portas e janelas)
  - Executar levantamento (calculo de materiais necessarios para servicos essenciais: loads, pad)
  - Executar Building Final — realizar avaliacao e solicitar ao setor de inspecao
  - Identificar criticidade de algumas etapas

---

### Checklists de Fase

#### Final Construction Check (P3 — Pre-Inspecao Final de Construcao)

Checklist aplicado pelo supervisor antes de solicitar a inspecao Building Final.

**1. Geral**
- Casa esta limpa
- Vinyl instalado corretamente
- Tiles instalados corretamente
- Armarios sem rachaduras ou arranhoes
- Rodapes bem instalados, sem brechas
- Drywall 100% fechado (sem buracos ou marcas de reparo)
- Prateleiras instaladas
- Espelhos instalados simetricamente
- Sem rachaduras no piso da garagem
- Sem rachaduras no driveway, calcada ou patio
- Grama instalada e sendo irrigada
- Garbage disposal instalado e funcionando

**2. Eletrico**
- Todas as luzes funcionando
- Luzes do banheiro centralizadas com espelho e torneira
- Interruptores de energia funcionando
- Electric Trim sem rachaduras
- Tomadas funcionando
- Detectores de fumaca instalados e funcionando
- Detectores de monoxido de carbono instalados e funcionando

**3. Hidraulico / Plumbing**
- Todos os plumbing trims instalados
- Agua quente funcionando
- Banheira sem danos
- Todas as torneiras bem instaladas e funcionando
- Descarga funcionando
- Ralos sem entupimento

**4. AC**
- Unidade de AC limpa (superior e inferior)
- Filtro de AC novo
- Todos os AC trims instalados
- AC funcionando

**5. Portas e Janelas**
- Fechadura eletronica instalada e funcionando (porta da frente)
- Todos os rodapes e molduras instalados
- Todas as portas em bom estado
- Todas as janelas abrindo corretamente
- Porta de correr de vidro abrindo corretamente e com fechadura
- Chaves da porta de correr disponiveis
- Todas as janelas e porta de correr com tela
- Sem rachaduras ou arranhoes em janelas ou porta de correr
- Todas as portas internas com macanetas e batedor de porta
- Todos os bifolds bem instalados e abrindo corretamente
- Porta da garagem para a casa devidamente vedada
- Porta da garagem funcionando; controle remoto e interruptor funcionando

---

#### Final House Check (P4 — Vistoria Final da Casa)

Checklist aplicado pelo supervisor na vistoria final antes da entrega ao cliente.

**1. Geral**
- Casa limpa
- Vinyl e tiles instalados corretamente
- Armarios sem rachaduras ou arranhoes
- Rodapes bem instalados
- Drywall 100% fechado
- Prateleiras e espelhos instalados
- Sem rachaduras no piso da garagem, driveway, calcada ou patio
- Paredes pintadas sem manchas
- Eletrodomesticos instalados e funcionando
- Garbage disposal instalado e funcionando

**2. Eletrico**
- Todas as luzes funcionando
- Luzes do banheiro centralizadas
- Interruptores e tomadas funcionando
- Electric Trim sem rachaduras
- Detectores de fumaca e monoxido de carbono instalados e funcionando

**3. AC**
- Unidade de AC limpa, filtro novo, AC funcionando

**4. Hidraulico / Plumbing**
- Agua quente funcionando; banheira sem danos
- Todas as torneiras bem instaladas
- Descarga funcionando; ralos sem entupimento
- Sem vazamentos em tubulacoes ou conexoes

**5. Portas e Janelas**
- Fechadura eletronica instalada e funcionando (porta da frente)
- Suporte de elevacao da porta da frente instalado
- Todos os rodapes e molduras instalados
- Todas as portas em bom estado; janelas abrindo corretamente
- Porta de correr: abrindo, com fechadura, chaves disponiveis, tela, sem rachaduras
- Persianas (shutters) instaladas corretamente
- Portas internas com macanetas e batedores
- Bifolds bem instalados e abrindo corretamente
- Porta da garagem para a casa vedada; garagem funcionando com controle remoto e interruptor
- Porta de vidro do box instalada
- Borracha de vedacao das portas e janelas instalada

**6. Jardim**
- Jardim da frente concluido

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- [Catalogo de Dores](07_CATALOGO_DORES.md)
- [Fluxo Spec Home](05_FLUXO_SPEC_HOME.md)
- [Fluxo Custom Home](06_FLUXO_CUSTOM_HOME.md)
- [Glossario de Termos](03_GLOSSARIO.md)
- **Departamentos relacionados:**
  - [Scheduling](dept_scheduling.md) — fornece informacoes de agendamento; recebe confirmacoes de campo
  - [Inspecao](dept_inspecao.md) — recebe resultados de inspecoes; envia verificacao previa de qualidade
  - [Financeiro](dept_financeiro.md) — envia checklist done como gatilho de pagamento
  - [Warranty](dept_warranty.md) — Daniel verifica reparos em casas de warranty

## CPM Construction Sequence Reference

The CPM flowchart defines all inspection and quality control points that Supervisao must verify in the field.

**Quality Control Points:**
- **QC1 (Quality Control 1):** Can be performed with Final Touches, on the FIRST day. Covers pre-final-inspection verification.
- **QC2 (Quality Control 2):** Should be performed with Final Touches, on the LAST day. Final quality gate before Building Final Inspection.

**Pre-Inspection Verification:** Before any county inspection, Supervisao performs field verification. The Inspection Validation Sub-System (see cpm_subsystems.md) defines the full state machine: pre-inspection checklist -> validation -> scheduling -> result -> rework if needed.

**Critical Inspection Dependencies for Field Checks:**
- Framing Inspection: requires ALL Rough inspections approved + Dry In + Windows/Doors
- Insulation Inspection: requires Insulation + Shingles + Windows completed
- Building Final: requires Final Plumbing + Final Electric + Final AC + Final Driveway + Blown-in Insulation + Blower Door Test + Appliances

**Security Verification:** Ensure Garage Door + Electronic Locker installed before Trim Set Material arrives (theft protection).

**Full reference:** [cpm_construction_sequence.md](cpm_construction_sequence.md) | [cpm_subsystems.md](cpm_subsystems.md)

---

## Key Glossary Terms

> Terms from [Glossario de Termos](03_GLOSSARIO.md) most relevant to the Supervisao (Field Supervision) department.

- **Rough (Plumbing/Electric/AC)** / **Instalacao Bruta**: Pre-finish installation within walls -- supervisor verifies quality before inspection
- **QPS (Quality Performance Standards)** / **Padroes de Qualidade**: Company quality procedures and standards -- Don and Fortine control quality
- **Punch List** / **Lista de Pendencias**: Items needing correction before delivery -- identified during final walkthrough by supervisor
- **Checklist Done** / **Checklist Concluido**: Supervisor completion confirmation -- PAYMENT TRIGGER for subcontractor invoice processing
- **Daily Logs** / **Registros Diarios**: Daily activity records with photos and notes per project in BuilderTrend -- central tracking document
- **Superintendent** / **Superintendente/Supervisor de Obras**: Person responsible for direct field supervision of construction
- **Compact Test** / **Teste de Compactacao**: Soil compaction test -- supervisor confirms elevation is correct before allowing compact test
- **Loads** / **Cargas de Terra**: Earth loads calculated and delivered by supervisors after stake house -- CRITICAL BOTTLENECK due to equipment shortage
- **Backcharge** / **Cobranca Retroativa**: Charge to sub for rework caused by their error -- supervisor documents deficiency
- **RFI (Request for Information)** / **Solicitacao de Informacao**: Formal clarification request about project specifications -- used when plans are unclear
- **Submittal** / **Submissao/Aprovacao de Material**: Document from sub for material approval before use -- ensures correct materials
- **Assignment** / **Tarefa/Atribuicao Diaria**: Daily task set assigned to supervisors and field teams -- they pick up materials based on this

---

## BuilderTrend Job 455 -- Real Data (Supplement)

### Supervisors on Job 455
| Supervisor | Phases | Checklists |
|-----------|--------|------------|
| Francisco Castillo / Eddye Pereira | Land Prep through Roughs | 28 checklists (Mar-Jun) |
| Jaaziel Santos | Finishing through Final | 22 checklists (Jun-Jul) |
| Daniel Consorte | QPS Inspector | FCC phases, walkthrough reports |

### Supervisor Checklist Sequence on Job 455
Land Prep (12 checklists): Clear Lot -> Stake House -> Loads/Pad -> Compact Test -> Hub/Tack -> Doc-box -> Form -> Underground Plumbing -> Water Service -> Slab Prep -> Electric Underground -> Slab Pouring

Masonry & Roofing (5): Masonry Assembly -> Lintel Pouring -> Framing -> Fascia -> Roof

Roughs (13): Windows -> Plumbing/AC/Electric Rough -> Lath -> Stucco -> Tub/Shower Pan -> Sewer Connection -> Insulation -> Termite Treatment -> Electric Meter -> Blow-in Insulation

Finishing (6): Interior Paint -> Driveway Form Up -> Garage Door -> Driveway Pouring -> Tile -> Vinyl

Trim (5): AC Trim -> Cabinets -> Trim Plumbing -> Trim Set -> Electric Trim

Final (5): Final Grade -> Final Paint -> Final Checklist -> Sod/Final Dirt -> Final Clean

### Quality Control on Job 455
- Daniel Consorte conducted FCC (Final Construction Check) phases
- Owner walkthrough (FCC4) on Sep 9, 2025
- 0 change orders = clean execution with no scope disputes

## CPM Construction Sequence -- Supervision Deep Dive

### Quality Control Points in CPM
| QC Activity | Timing | Description |
|-------------|--------|-------------|
| Quality Control 1 | With Final Touches (FIRST day) | First quality sweep |
| Quality Control 2 | With Final Touches (LAST day) | Final quality sweep |
| FCC | After Building Final Inspection | Final Construction Check |
| Internal Walkthrough | Before Client Walkthrough | Company internal review |
| Client Walkthrough | After Internal Walkthrough | Formal handover |

### Inspection Validation Sub-System -- Supervisor Role
Supervisors play a key role in the Inspection Validation sub-system:
1. **Pre-inspection validation**: Supervisor validates work quality BEFORE scheduling county inspection
2. **Rework coordination**: If validation fails, supervisor schedules rework with original sub
3. **Re-validation**: After rework, supervisor re-validates before re-scheduling inspection
4. **Status tracking**: `{INSPECTION} + INSPECTION VALIDATED` vs `{INSPECTION} + INSPECTION DISAPPROVED`
5. **Rework flow**: `{PRE-INSPECTION PROCESS} + REWORK SCHEDULED` -> `REWORK CHECKLIST DONE`

### Critical Dependencies for Supervisors from CPM
- Verify Underground Electrical was actually completed before proceeding to Slab Prep
- Verify external activities (Septic Cover, Stucco) finished before Driveway
- Always double-check ALL prerequisites for Building Final Inspection
- Ensure Loads quantity is informed by Supervisor before scheduling
- Monitor that Termite Treatment happens BEFORE insulation

## Const App Integration (Supplement)

### Verification Module
- **Pending Verifications**: Review and verify completed services (Pending, Site Visits Today, Photo Review, Failed, Verified)
- **Site Visits**: Plan and manage site visits for service verification; route optimization coming soon
- Supervisors are the primary users of the verification module -- they confirm service completion

### Rework Module
- **Rework Queue**: Manage inspection items sent for rework (Pending Assignment, Sent to Handymen)
- **Handymen Kanban Board**: Assign reworks to handymen, track progress with drag-and-drop
- **Completed History**: Permanent record of all completed reworks with duration tracking
