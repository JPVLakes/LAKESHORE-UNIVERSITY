# Utilities (Utilidades) - Lakeshore Development

## Visao Geral

- **Missao:** Coordenar todos os servicos de utilidades (agua, esgoto, energia e gas) para os projetos da Lakeshore, desde a verificacao de disponibilidade ate a instalacao de medidores e transferencia de contas ao proprietario. Gerenciar a interacao com concessionarias de cada condado e monitorar instalacoes em campo.
- **Lider:** Dandara Souza - Utilities
- **Equipe:** [inferido] Dandara como responsavel principal, com suporte de monitores de campo
- **Departamentos relacionados:** Permits, Financeiro, Client Relations, Scheduling, Supervisores/Monitores, Core Craft (Services)

## Processos

### Processo 1: Verificacao de Disponibilidade de Agua e Esgoto

- **Objetivo:** Identificar sistemas disponiveis de agua e esgoto para cada novo projeto e comunicar custos extras quando aplicavel
- **Responsavel principal:** Dandara Souza
- **Frequencia:** A cada novo jobsite criado no Builder Trend
- **Ferramentas:** Planilha de Utilities, Builder Trend (Daily Logs, campos customizados), Slack, E-mail

**Passo a passo:**
1. Receber notificacao de novo jobsite criado no BT (via Slack) -- Responsavel: Dandara -- Ferramenta: Slack
2. Identificar casa, endereco, companhias de agua/esgoto/energia -- Responsavel: Dandara -- Ferramenta: Planilha de Utilities
3. Solicitar UAL (Utilities Availability Letter) por e-mail a companhia -- Responsavel: Dandara -- Ferramenta: E-mail
4. Registrar data de solicitacao e recebimento -- Responsavel: Dandara -- Ferramenta: Planilha de Utilities
5. Analisar disponibilidade de **agua** (5 opcoes):
   - **Disponivel (Standard)**: conexao normal, paga taxa, aguarda medidor
   - **Informacao nao disponivel**: requer pagamento para verificar (raro)
   - **Beneficiado (Benef)**: extensao de linha pronta, custo extra -> client hold
   - **Extension**: extensao necessaria, custo alto -> client hold (pode desistir)
   - **Poco (Well)**: sem acesso a agua, instalar poco -> custo extra
   -- Responsavel: Dandara -- Ferramenta: Planilha de Utilities
6. Analisar disponibilidade de **esgoto** (4 opcoes):
   - **Gravity**: sistema publico por gravidade (raro em Marion)
   - **Septic**: sistema proprio (mais comum em Marion), sem custo extra
   - **Nitrogenio**: septic mais eficiente, custo extra -> client hold
   - **LPS**: sistema em Charlotte County (meio termo)
   -- Responsavel: Dandara -- Ferramenta: Planilha de Utilities
7. Registrar informacoes em Daily Logs com tags especificas -- Responsavel: Dandara -- Ferramenta: Builder Trend
8. Registrar nos campos customizados dos jobs (companhias e sistemas) -- Responsavel: Dandara -- Ferramenta: Builder Trend
9. Se custo extra: notificar Slack para Client Relations -> contato com cliente -> aprovacao -> notificar Financeiro -> pagamento -- Responsavel: Dandara -- Ferramenta: Slack

**Inputs:** Notificacao de novo jobsite, endereco do projeto
**Outputs:** UAL recebida, sistema de agua/esgoto definido, client hold se aplicavel
**Observacoes:** Cada combinacao de condado e companhia tem regras diferentes. Informacao sobre sistema (septico ou esgoto publico) deve chegar automaticamente a equipe de Permits. Triplo registro atual: planilha + Daily Logs + campos customizados do BT.

### Processo 2: Processo de Energia (Abertura de Conta e Underground)

- **Objetivo:** Coordenar abertura de conta de energia, determinar tug side, e acompanhar instalacao de fiacao subterranea e medidor eletrico
- **Responsavel principal:** Dandara Souza
- **Frequencia:** A cada novo projeto (gatilho: permit recebido)
- **Ferramentas:** Sites das companhias (DUC, FPL, CICLE, WEC), Planilha de Utilities, Builder Trend, Slack, E-mail

**Passo a passo:**
1. Receber notificacao de permit recebido (canal Slack) -- Responsavel: Dandara -- Ferramenta: Slack
2. Identificar companhia de energia via sites das companhias -- Responsavel: Dandara -- Ferramenta: Sites (DUC, FPL, CICLE, WEC)
3. Abertura de conta (varia por companhia):
   - CICLE/Recitrus: preencher formularios, pegar assinatura, abrir conta por e-mail apos second draw received
   - DUC: portal online, prazos longos, abrir conta assim que permit recebido
   - FPL: portal online (similar a DUC)
   - WEC: pagamento por ligacao
   -- Responsavel: Dandara -- Ferramenta: Sites das companhias / E-mail
4. Registrar data de "open account" -- Responsavel: Dandara -- Ferramenta: Planilha de Utilities
5. Invoice de abertura (CICLE e WEC cobram) -> encaminhar ao financeiro -> atualizar PO -- Responsavel: Dandara -- Ferramenta: E-mail / Builder Trend
6. Determinar **Tug Side** (lado da caixa eletrica):
   - CICLE: sempre lado da garagem
   - DUC/FPL/WEC: questionar engenheiro da companhia
   -- Responsavel: Dandara -- Ferramenta: E-mail
7. Informar tug side ao Scheduling (RF Electric) -- Responsavel: Dandara -- Ferramenta: Slack/E-mail
8. Apos aprovacao da Tug Inspection (notificacao Slack): informar companhia por e-mail para agendar underground electric -- Responsavel: Dandara -- Ferramenta: E-mail / Slack
9. Schedule no Daily Logs com prazo de 3 semanas e entrada na rota dos monitores -- Responsavel: Dandara -- Ferramenta: Builder Trend
10. Underground Electric instalado: verificar invoice (se custo > $1.000 acima do budget -> client hold) -- Responsavel: Dandara -- Ferramenta: Planilha / Slack
11. Instalacao do Electric Meter (na maioria junto com underground; DUC: separado, apos underground + invoice pago + house numbers instalados) -- Responsavel: Dandara -- Ferramenta: E-mail / Builder Trend

**Inputs:** Notificacao de permit, informacoes da companhia de energia
**Outputs:** Conta de energia aberta, tug side definido, underground electric instalado, medidor eletrico instalado
**Observacoes:** Informacao de tug side e crucial para scheduling (RF Electric). Se instalar no lado errado, custo adicional. Prazos das companhias sao incertos (especialmente DUC).

### Processo 3: Instalacao do Medidor de Agua (Water Meter)

- **Objetivo:** Acompanhar pagamento de construction charges e instalacao do medidor de agua
- **Responsavel principal:** Dandara Souza
- **Frequencia:** A cada projeto com agua disponivel
- **Ferramentas:** Planilha de Utilities, Builder Trend (Daily Logs), E-mail

**Passo a passo:**
1. Verificar pagamento das construction charges pelo financeiro -- Responsavel: Dandara -- Ferramenta: Planilha / E-mail
2. Agendar no Daily Logs como "schedule" para water meter installation -- Responsavel: Dandara -- Ferramenta: Builder Trend
3. Prazo medio: 1 mes apos pagamento das construction charges -- Responsavel: Dandara
4. Entrada na rota dos monitores (1x por semana apos 1 mes) -- Responsavel: Dandara -- Ferramenta: Builder Trend
5. Confirmar instalacao do medidor -- Responsavel: monitores de campo -- Ferramenta: Builder Trend

**Inputs:** Construction charges pagas, informacoes da companhia de agua
**Outputs:** Medidor de agua instalado e confirmado
**Observacoes:** Medidores as vezes instalados sem notificacao ou roubados. Monitoramento presencial necessario.

### Processo 4: Gerenciamento de Septic (Sistema Septico)

- **Objetivo:** Coordenar instalacao e inspecao do sistema septico quando necessario
- **Responsavel principal:** Dandara Souza
- **Frequencia:** A cada projeto com sistema septico (comum em Marion County)
- **Ferramentas:** E-mail, Builder Trend, Planilha de Inspections

**Passo a passo:**
1. Verificar se e septic convencional ou nitrogenio (manual) -- Responsavel: Dandara -- Ferramenta: Planilha de Utilities
2. Gatilho: aprovacao da inspecao de Roof Assembly (notificacao Slack) -- Responsavel: Dandara -- Ferramenta: Slack
3. Verificar com supervisor se lote tem stakes (piquetes de demarcacao); se nao tem, acionar surveyor para remarcar (custo extra) -- Responsavel: Dandara -- Ferramenta: Slack/WhatsApp
4. Solicitar servico por e-mail:
   - Marion (convencional): solicitar a Alisbird
   - Marion (nitrogenio): solicitar a Howard (preco menor)
   - Citrus: outra empresa (faz tudo no mesmo dia)
   -- Responsavel: Dandara -- Ferramenta: E-mail
5. Criar PO e registrar datas -- Responsavel: Dandara -- Ferramenta: Builder Trend
6. Acompanhar instalacao e conexao:
   - Alisbird: faz conexao como cortesia
   - Howard: nao faz conexao -> acionar Plumber (Colano)
   -- Responsavel: Dandara -- Ferramenta: E-mail / Builder Trend
7. Inspecoes do Septic:
   - DOH (Dept. Saude): inspetor privado (soil engineer); sub envia notificacao por e-mail
   - Conexao: tubulacao deve estar totalmente exposta; se nao, acionar Services (Core Craft) para expor
   -- Responsavel: Dandara -- Ferramenta: E-mail / Builder Trend
8. Apos aprovacao DOH: pode cobrir, mantendo conexao exposta para segunda inspecao -- Responsavel: Dandara
9. Pegar assinatura do owner (via Client Relations) para inspetor privado -- Responsavel: Dandara (via CR) -- Ferramenta: E-mail
10. Salvar Septic Permit no Builder Trend -- Responsavel: Dandara -- Ferramenta: Builder Trend

**Inputs:** Informacao de sistema septico, aprovacao de roof assembly, stakes do lote
**Outputs:** Sistema septico instalado, inspecionado e aprovado, septic permit salvo
**Observacoes:** Processo do septic esta crescendo com mais etapas (stakes, assinatura do owner, inspecoes mais rigorosas). Necessidade de proposed site plan feito por soil engineer.

### Processo 5: Fechamento de Contas (Account Closing)

- **Objetivo:** Transferir contas de utilities para o nome do proprietario apos venda da casa
- **Responsavel principal:** Dandara Souza
- **Frequencia:** A cada casa vendida/fechada
- **Ferramentas:** E-mail, Planilha de Utilities

**Passo a passo:**
1. Receber informacao de venda da casa (closing) -- Responsavel: Dandara -- Ferramenta: [inferido] Slack/E-mail
2. Verificar se contas estao no nome da Lakeshore -- Responsavel: Dandara -- Ferramenta: Planilha de Utilities
3. Cancelar energia (simples) -- Responsavel: Dandara -- Ferramenta: Sites das companhias / E-mail
4. Cancelar agua (requer documento + assinatura) -- Responsavel: Dandara -- Ferramenta: E-mail

**Inputs:** Informacao de closing da casa
**Outputs:** Contas transferidas/canceladas
**Observacoes:** [inferido] Processo entra no radar 5 dias apos closing checklist. Desenvolvimento dessa funcionalidade no software foi adiado.

### Processo 6: Monitoramento de Contas Pos-Instalacao

- **Objetivo:** Acompanhar contas mensais de energia e agua das casas em construcao e gerenciar pagamentos
- **Responsavel principal:** Dandara Souza / Bruna Jonair Carvalho (Financeiro)
- **Frequencia:** Mensal
- **Ferramentas:** Planilha de Utilities, Sites das companhias, E-mail

**Passo a passo:**
1. Apos instalacao dos medidores: contas mensais comecam a chegar -- Responsavel: Dandara/Bruna -- Ferramenta: Sites/E-mail
2. Casas abertas (em construcao): pagamento direto pela Lakeshore -- Responsavel: Bruna -- Ferramenta: Sites das companhias
3. Casas fechadas sem pendencias: contatar proprietario sobre pagamento -- Responsavel: Bruna -- Ferramenta: E-mail
4. Se proprietario nao responde e conta acumula: OS liga para proprietario; em caso critico, Bruna paga e cria invoice -- Responsavel: Bruna/Cintia -- Ferramenta: E-mail

**Inputs:** Faturas de energia e agua
**Outputs:** Pagamentos efetuados, invoices criados para proprietarios inadimplentes
**Observacoes:** Faturas chegam por multiplas fontes: sites das companhias, e-mail, correspondencia escaneada pelo escritorio. Fernanda solicitou inclusao do valor de cada fatura para monitoramento de variacoes.

## Dores e Problemas Conhecidos

- **Triplo registro**: planilha + Daily Logs + campos customizados do BT -- mesma informacao inserida em 3 lugares
- **Dificuldade de obter informacoes das companhias**: ma vontade, informacao dificil; medidores instalados sem notificacao ou roubados
- **Informacoes dispersas**: precisa consultar varias planilhas e sistemas para encontrar supervisor, dados da casa, etc.
- **Processo do septic crescendo**: mais etapas, inspecoes mais rigorosas
- **Variabilidade por condado e companhia**: cada combinacao tem regras diferentes
- **Comunicacao fragmentada**: WhatsApp, Slack, e-mail, BT, planilha - varios canais
- **Falta de previsibilidade**: prazos das companhias sao incertos (especialmente DUC)
- **Retrabalho com tug side**: se instalar no lado errado, custo adicional significativo
- **Multiplas fontes de faturas**: site, e-mail, correspondencia fisica - dificulta centralizacao
- **Portal Alex Shore com problemas**: apos migracao, nao consegue acessar, pagando faturas uma a uma

## Dependencias

- **Recebe de:**
  - Builder Trend / Slack: notificacao de novo jobsite (gatilho para agua/esgoto)
  - Permits: notificacao de permit recebido (gatilho para energia), permit number
  - Financeiro: pagamento de invoices, construction charges, atualizacao de POs
  - Supervisores/Monitores: verificacao em campo (medidores, stakes, conexoes)
  - Core Craft (Services): remocao de dumpster quando bloqueia tug, exposicao de tubulacao
  - Surveyor: remarcar stakes do lote
  - Soil Engineer: proposed site plan e septic permit
  - Client Relations: aprovacao do cliente para custos extras

- **Entrega para:**
  - Permits: informacao sobre sistema de agua/esgoto (septic vs gravity) que impacta documentacao
  - Client Relations: informacoes de custos extras para comunicar ao cliente (client holds)
  - Financeiro: invoices de abertura de conta, POs
  - Scheduling: informacao de tug side para RF Electric
  - Campo/Supervisores: informacoes sobre instalacoes agendadas

---

## Descricao de Cargo Formal (Fonte: Drive Lakeshore)

### Coordenador de Utilities

- **Setor:** Utilities & Inspections — Utilities
- **Descricao geral:** Responsavel pela abertura e fechamento de contas de energia, agua e esgoto. Acompanhamento de processos, solicitacao de instalacao do septico, dos medidores de agua e de energia.
- **Principais responsabilidades e processos:**
  - Checar a companhia de agua, esgoto e energia para cada projeto
  - Solicitar Utility Availability Letter (UAL) para companhia de agua e esgoto
  - Sinalizar possivel custo extra em casos de extension, benefiting, Well e nitrogen
  - Solicitar Tug Side para companhia de energia
  - Acompanhar instalacao do medidor de agua
  - Abertura da conta de energia apos o Permit ser issued
  - Avisar a companhia que U.P. (Underground Plumbing inspection) foi agendado (SECO)
  - Encaminhar invoice de abertura de conta para o financeiro
  - Encaminhar invoice de Underground Electric para o financeiro; sinalizar possivel custo extra
  - Enviar e-mail para a companhia de energia quando o TUG Inspection for aprovado
  - Acompanhar as datas para instalacao do underground electric e electrical meter
  - DUKE: checar se os numeros da casa foram instalados e solicitar o electrical meter
  - Solicitar a instalacao do septic quando a inspecao do roof assembly for agendada
  - A depender da empresa instaladora, solicitar a conexao do septic para a empresa de plumbing
  - Solicitar a cobertura do septic quando houver aprovacao nas inspecoes (DOH e Building Department)
  - Solicitar instalacao do Well quando necessario apos a concretagem do slab
  - Solicitar teste de qualidade da agua quando o poco estiver em funcionamento
  - Fechar contas quando a casa for vendida

---

## Procedimentos Operacionais Padrao (Fonte: Drive QPS)

Os SOPs abaixo detalham as etapas formais, empresas, formularios, taxas e condicoes especificas de cada tipo de utility. Complementam os processos resumidos acima com precisao operacional extraida dos manuais oficiais do departamento.

---

### SOP-UAL: Utility Availability Letter

**Responsavel:** Departamento de Utilities
**Gatilho:** Verificacao diaria da aba Contracts na Planilha Lakeshore — nova casa identificada

**Passo a passo:**

1. Identificar nova casa na aba Contracts (endereco e parcel)
2. Enviar e-mail de solicitacao da UAL para a MCU com endereco e parcel
3. Marcar check no campo de solicitacao da letter na aba de Utilities da Planilha Lakeshore
4. Ao receber a UAL, disponibilizar em todos os meios obrigatorios:
   - Pasta da casa no Drive: upload da letter
   - Pasta da casa no BT: upload da letter
   - Schedule no BT: preencher Water Availability, Sewer Availability, datas de solicitacao e recebimento
   - Aba de Utilities na Planilha Lakeshore: preencher campos de Water/Sewer Availability + check de recebimento
   - Slack canal Permit: enviar informacoes de Water Availability e Sewer Availability
   - Canva Utilities Red Flags (setor Permit): preencher para casos especiais de sewer (nitrogen, gravity) e water (well com possibilidade de variance, extension com possibilidade de waiver, benefitting)
5. Verificar, em paralelo com a UAL, a companhia de energia via Interactive Map (pesquisa pelo parcel) e registrar na aba de Utilities da Planilha Lakeshore

**Casos especiais identificados pela UAL que geram Red Flag:**
- Water: Well (lote sem acesso a agua publica), Extension, Benefitting
- Sewer: Nitrogen, Gravity

---

### SOP-WATER: Agua (Marion County Utilities)

**Responsavel:** Departamento de Utilities (formularios e acompanhamento), Permit (assinaturas), Financeiro (pagamentos), Field (confirmacao de servicos), Subs (agendamento)

#### Cenario A — Standard Connection

1. UAL confirma standard connection e processo de permit iniciado
2. MCU envia invoice de construction charges para o departamento de Permit
3. Apos pagamento pelo Financeiro, prazo estimado de **3 a 6 meses** para instalacao do water meter (variavel: necessidade ou nao de tap)
4. Instalacao confirmada via Daily Logs do Field ou por e-mail/ligacao ao county
5. Atualizar data no BT (Schedule) e na aba de Utilities da Planilha Lakeshore
6. Verificar se a inspecao do Septic DOH esta com pendencia de water line:
   - Water meter nao instalado: aguardar instalacao
   - Water meter instalado: solicitar instalacao da water line ao depto de Subs e informar data prevista ao Field

#### Cenario B — Benefitting Parcel

- Mesmo fluxo da Standard Connection
- Diferenca: invoice das construction charges inclui valor adicional referente ao benefitting

#### Cenario C — Well (Poco)

**C.1 — Lote menor que 0,5 ha (requer Variance)**

1. Verificar tamanho do lote no site Property Appraiser de Marion County
2. Sendo menor que 0,5 ha, aplicar para Variance junto ao DOH por e-mail
3. Montar pacote PDF de aplicacao na seguinte sequencia obrigatoria:
   - Formulario de aplicacao (2 partes): preencher a primeira parte; enviar ambas ao Permit para coleta de assinatura do representante da empresa ou do proprietario
   - Denial letter: solicitar ao soil engineering por e-mail
   - Septic permit: localizado nos documentos da casa no BT
   - Mapa do lote: gerar PDF via Interactive Map com identificacao do parcel number + subdivision
4. Enviar pacote ao DOH por e-mail
5. DOH retornara solicitando pagamento via Credit Card Authorization no valor de **$200**
   - Preencher o formulario e enviar ao Financeiro para assinatura do responsavel da Lakeshore
   - Apos pagamento, enviar comprovante ao DOH e ao Financeiro
6. DOH enviara e-mail com data da reuniao de avaliacao (participacao facultativa, recomendada em casos de atraso)
7. Se aprovado na reuniao (ou apos recebimento da approval letter): solicitar instalacao do Well por e-mail para a empresa **Bryans Pump**
8. Comunicar data prevista de instalacao via WhatsApp ao Field
9. Confirmar instalacao (Field); atualizar aba de Utilities da Planilha Lakeshore e BT
10. Solicitar retorno do inspetor privado por e-mail para finalizar a inspecao do Septic DOH (caso esteja com essa pendencia); registrar resultado na aba de Inspections da Planilha Lakeshore

**C.2 — Lote maior que 0,5 ha**

1. Verificar tamanho do lote no Property Appraiser
2. Solicitar instalacao do Well diretamente por e-mail para a empresa **Bryans Pump** (sem necessidade de Variance)
3. Comunicar data prevista ao Field via WhatsApp
4. Confirmar instalacao (Field); atualizar aba de Utilities e BT
5. Solicitar retorno do inspetor privado por e-mail para finalizar a inspecao do Septic DOH; registrar resultado na aba de Inspections

#### Cenario D — Extension

1. UAL retorna com opcao de extension
2. Informar departamento de Permit via Slack; casa fica On Hold ate decisao do proprietario

**D.1 — Waiver (condicao especifica: Marion Oaks 07 e 10 com connection distance = 0)**

1. MCU envia por e-mail os documentos para aplicacao de waiver (formulario + mapa do local)
2. Preencher o formulario e enviar ao Permit para coleta de assinatura do proprietario
3. Enviar formulario assinado + mapa ao Department of Development Review (DDR)
4. Ligar para o DDR para efetuar pagamento da application fee: **$300**
5. DDR enviara convite para reuniao de decisao (participacao opcional)
6. Resultado positivo: MCU envia Conditional Waiver Acceptance Letter + invoice de **$5.000** (valor nao inclui construction charges)
7. Solicitar cheque ao Financeiro e entregar pessoalmente ao MCU

**D.2 — Extension (demais casos)**

1. Proprietario decide continuar; MCU envia formulario de aplicacao para a Lakeshore
2. Preencher o formulario e enviar ao Permit para impressao
3. Reunir pacote de documentos:
   - Formulario preenchido (impresso)
   - Print do site Property Appraiser de Marion County
   - Se owner for empresa: W9 (requisitar a empresa), copia do registro no Sunbiz
   - Cheque de pagamento no valor de **$275** (application fee)
4. Solicitar cheque ao Financeiro
5. Entregar pacote completo (formulario + documentos + cheque) ao MCU

#### Tabela de Taxas — Water

| Situacao | Taxas |
|---|---|
| Standard | Construction charges |
| Benefitting | Construction charges + valor benefitting |
| Waiver | Application fee $300 + Advanced extension $5.000 + Construction charges |
| Extension | Application fee $275 + ~$100/pe + Construction charges |
| Variance (Well) | Application fee $200 (sem construction charges — sem conexao publica) |

**Composicao das Construction Charges (valores usuais: $2.069, $2.549 ou $2.769):**
- Water Meter Installation 5/8" x 3/4": **$360**
- Capital Charges — Residential Water (per ERC): **$1.659**
- Service Tap Fee:
  - No tap: **$0**
  - Short tap: **$480**
  - Long tap: **$610**
- Para benefitting parcel: valor correspondente acrescido ao total acima

---

### SOP-SEPTIC: Esgoto Septico (Marion County)

**Responsavel:** Departamento de Utilities (agendamentos e inspecoes), Field (confirmacoes), Subs (conexoes e water line)
**Gatilho:** Solicitacao da inspecao de Roof Assembly pelo Field

**Empresas envolvidas:**
- **Leesburg**: empresa de septic — envia solicitacao de inspecao DOH por e-mail e pode ou nao fazer conexao no mesmo momento
- **Rowand**: empresa de septic — nao faz a conexao; confirmacao chega por e-mail apos instalacao

#### Etapa 1 — Solicitacao de Instalacao

1. Aguardar solicitacao da inspecao de Roof Assembly pelo Field
2. Enviar e-mail para as empresas **Leesburg** e **Rowand** com: lista de casas, enderecos, parcels, septic permits correspondentes e ordem de prioridade de instalacao
   - Septic permit localizado na pasta da casa no BT ou no Drive
3. Ao receber confirmacao, enviar data estimada de instalacao ao Field

#### Etapa 2 — Instalacao e Inspecoes por Empresa

**Leesburg — com conexao realizada:**
1. Leesburg solicita inspecao DOH (inspetor privado) por e-mail; confirmar servico com o Field
2. Conexao feita: solicitar inspecao de Sewer Septic via grupo de WhatsApp Inspections Request
3. Apos resultado da inspecao DOH + resultado da inspecao Sewer Septic: enviar e-mail a Leesburg para realizar o cover

**Leesburg — sem conexao:**
1. Leesburg solicita inspecao DOH; confirmar com Field — conexao nao realizada
2. Solicitar instalacao da conexao ao depto de Subs; enviar data estimada ao Field
3. Apos confirmacao do Field: solicitar inspecao de Sewer Septic via WhatsApp Inspections Request
4. Resultado da inspecao DOH recebido por e-mail: solicitar adiamento do cover ate resultado do Sewer Septic estar disponivel
5. Com ambos os resultados: solicitar cover por e-mail

**Rowand:**
1. E-mail de confirmacao de instalacao recebido: solicitar instalacao da conexao ao depto de Subs; enviar data estimada ao Field
2. Apos confirmacao do Field: solicitar inspecao de Sewer Septic via WhatsApp + solicitar inspecao DOH por e-mail
3. Com os resultados prontos: colocar empresa em copia no e-mail de resultado — empresa agenda o cover

#### Etapa 3 — Resultados da Inspecao DOH

- **Aprovacao:** inspetor privado envia e-mail com resultado ao DOH (Lakeshore em copia) com documentacao oficial; aguardar resultado no site do county (sinalizado por e-mail); inserir resultado na aba de Inspections da Planilha Lakeshore
- **Aprovacao parcial (pendencia de water line):** inspetor envia aprovacao parcial por e-mail; confirmar previsao de instalacao do water meter com MCU; apos instalacao, solicitar ao depto de Subs agendamento da water line; quando instalada, enviar e-mail ao inspetor privado solicitando retorno para conferencia e aprovacao final
- **Reprovacao:** inspetor envia e-mail com ajustes necessarios para a empresa instaladora e para a Lakeshore
- **Resultado parcial:** inserir no Daily Logs do BT e comunicar ao responsavel do Field; aguardar novo e-mail do inspetor ao DOH com documentacao oficial; acompanhar resultado no site do county

---

### SOP-ENERGIA: Energia Eletrica (Seco e Duke)

**Responsavel:** Departamento de Utilities (abertura de conta, acompanhamento, datas), Permit (assinaturas), Financeiro (pagamentos), Field (confirmacoes)
**Determinacao da companhia:** pesquisar parcel no site Interactive Map no momento da solicitacao da UAL

#### Cenario A — Seco

1. Registrar "Seco" na aba de Utilities da Planilha Lakeshore
2. Enviar e-mail a Seco solicitando o TUG Side
3. Aguardar aviso do setor de Permit (via grupo Slack) sobre aplicacao do permit para entao enviar informacao do TUG Side ao surveyor para elaboracao do site plan
4. Quando Permit informa via WhatsApp que o status do permit e "Issued": enviar e-mail a Seco solicitando abertura de conta
5. E-mail de abertura de conta deve conter formulario de cadastro preenchido com:
   - Detalhes da localizacao (parcel)
   - Tipo de servico: Temporary Service Underground, Permanent Service TUG
   - Total HVAC square footage (mesmo numero do modelo da casa)
   - Number of A/C Units, size and tons
   - Main Panel Size
   - Permit number
   - Data estimada de termino da obra (considerar 3 meses a partir do e-mail)
   - Enviar formulario ao Permit para coleta de assinatura da Lakeshore antes do envio
   - Anexar site plan (com septic), localizado na pasta da casa no BT
6. Seco retornara invoice de membership application: encaminhar ao Financeiro
   - Taxa atual: **$465** (composta por $355 de deposito + $110 de fee de conexao)
7. Seco encaminhara caso a engenheiro para visita local e elaboracao do design do underground electric
8. Invoice do Underground Electric + Electric Meter sera enviado por e-mail (prazo de chegada: ~2 meses); encaminhar ao Financeiro para pagamento
   - Valor varia conforme distancia ao poste e disponibilidade de poste na regiao (normalmente abaixo de $1K, podendo chegar a $9.500)
9. Resultado positivo da TUG Inspection: enviar resultado por e-mail a Seco
   - Invoice deve estar pago antes do agendamento do UE
10. Underground Electric (UE) agendado; Electric Meter usualmente instalado no mesmo dia do UE
11. Confirmar instalacao via Daily Logs (input do Field) ou e-mail a Seco solicitando datas
12. Atualizar datas no Schedule do BT e na aba de Utilities da Planilha Lakeshore

#### Cenario B — Duke

1. Registrar "Duke" na aba de Utilities da Planilha Lakeshore
2. Aguardar aprovacao do permit para abertura de conta
3. Abrir conta via Builder Portal: https://builderportal.duke-energy.app/home
   - Preencher com dados da aba de Utilities da Planilha Lakeshore
4. Duke enviara 3 e-mails sequenciais:
   - E-mail 1: confirmacao de cadastro
   - E-mail 2: work order
   - E-mail 3: formulario adicional — preencher com dados da aba de Utilities e enviar com Site Plan (com septic, localizado na pasta da casa no BT)
5. Duke confirmara recebimento e encaminhara caso a engenheiro para visita local e elaboracao do design do underground electric
6. Engenheiro enviara TUG Side por e-mail apos a visita
7. Se a propriedade nao tiver poste no limite do terreno: engenheiro requisitara marcacao do terreno
   - Encaminhar pedido ao Field; apos marcacao, enviar e-mail de confirmacao ao engenheiro responsavel
8. Duke enviara invoice do Underground Electric + Property Damage and Release and Liability Waiver:
   - Invoice: encaminhar ao Financeiro para pagamento
   - Formulario waiver: preencher e enviar ao Permit para assinatura da Lakeshore
9. Resultado positivo da TUG Inspection: enviar e-mail ao engenheiro responsavel informando aprovacao
   - Invoice deve estar pago antes do agendamento
10. Agendamento do Electric Meter: ligar para Duke Energy no telefone **866-372-4663** informando resultado da inspecao e solicitando agendamento
    - Condicao obrigatoria: casa deve ter os numeros do endereco instalados
    - Se a casa tiver mais de um TUG: todos devem estar identificados com numero e unidade
11. Confirmar instalacao via Daily Logs (input do Field) ou ligacao para a Duke
12. Atualizar datas no Schedule do BT e na aba de Utilities da Planilha Lakeshore

---

## Transferencia de Contas (Fonte: Drive Lakeshore)

Procedimentos oficiais para transferencia e abertura de contas de utilities em nome do proprietario apos o fechamento. O prazo padrao e de 5 dias a partir da notificacao para evitar interrupcao do servico.

---

### Agua — Marion County Utilities

**Contato:** utilities@marionfl.org
**Prazo:** 5 dias para evitar interrupcao do servico

**Documentos necessarios:**
- Service Agreement (formulario de deposito e contrato de servico — preenchido e assinado)
- Letter of Guarantee (necessaria quando conta e aberta em nome de empresa)
- Copia do passaporte do titular
- Prova de propriedade: pagina do Property Appraiser, escritura de garantia ou settlement statement

**Como preencher o Service Agreement:**
- Business Name
- Tax ID / EIN number
- Service Address e Parcel ID
- Indicar se o solicitante e Owner ou Tenant
- Telefone e e-mail de contato
- Assinatura do Primary Applicant e data

**Como preencher a Letter of Guarantee (para contas em nome de empresa):**
- Owner/Manager: nome do responsavel
- Business Name: nome da empresa
- Property Address: endereco do imovel
- Date e Sign: data e assinatura do responsavel

**Template de e-mail sugerido:**
```
Subject: Request to Set up Water Account

Hello,
This is [NOME] from [EMPRESA].
I would like to set up the account for the following property under my company's name.
Attached are the documents you might need.
Property Address: [ENDERECO]
I kindly ask you to confirm once the account has been successfully set up.
Thank you in advance for your attention to this matter.
Best regards,
```

---

### Agua — Citrus County Utilities

**Contato:** WaterResources@citrusbocc.com
**Prazo:** 5 dias para evitar interrupcao do servico

**Documentos necessarios:**
- Application for Water and/or Sewer Service (formulario preenchido e assinado)
- Pagina do Property Appraiser mostrando propriedade no nome do solicitante

**Como preencher o Application Form:**
- Utility Service Address, City, State, ZIP
- Utility Account Holder Name(s)
- Business Accounts — EIN Number (se aplicavel)
- Date Requesting Service(s) To Be Turned On
- Customer's Signature(s): Print / Sign

**Template de e-mail sugerido:**
```
Subject: Request to Set up Account

Hello,
This is [NOME] from [EMPRESA].
I would like to set up the account for the following property under my company's name.
Attached are the documents you might need.
Property Address: [ENDERECO]
I kindly ask you to confirm once the account has been successfully set up.
Thank you in advance for your attention to this matter.
Best regards,
```

---

### Energia — SECO Energy

**Contato:** Portal online SECO Energy – New Service Connection Portal / telefone: 352-793-3801
**Observacao:** Mesmo com solicitacao online, um representante entrara em contato para verificacao de identidade

**Passo a passo:**
1. Acessar o portal e buscar o endereco completo do imovel no campo "Search for Your New Service Address"
2. Selecionar "I'm a new customer" e preencher nome completo (ou nome da empresa)
3. Informar Data de Nascimento e SSN (ou EIN para conta empresarial); Driver's License opcional
4. Informar numero de telefone valido; definir endereco de correspondencia
5. Informar e-mail, confirmar, marcar "I'm not a robot" e clicar em Continue
6. Verificar o e-mail recebido da SECO Energy SmartHub e clicar em "Verify Account" para confirmar a conta e definir senha
7. Decidir sobre Equifax Utility Score Check:
   - "Yes": SECO verifica credito (SSN ou EIN) para avaliar isencao de deposito (nao garante isencao)
   - "No": SECO nao verifica credito; deposito inicial obrigatorio para abertura da conta

---

### Energia — Duke Energy

**Contato:** 877-372-8477 (ligacao obrigatoria — solicitacao nao pode ser feita por terceiros)
**Observacao:** Apenas o novo titular da conta pode falar com a Duke Energy e autorizar a ativacao

**Documentos / informacoes que podem ser solicitados:**
- Numero da carteira de motorista
- Numero do Social Security (SSN)
- Numero do passaporte
- Numero de identificacao da empresa (EIN)

**Nota operacional:** O titular pode comparecer ao escritorio da Lakeshore para receber suporte durante a ligacao, porem a comunicacao com a Duke deve ser feita exclusivamente pelo proprio titular por razoes de seguranca.

---

## Operational Detail (from Interviews)

### 4 Water Availability Types

When a new jobsite is created, Dandara checks the Utilities Availability Letter (UAL) to determine the water source. There are 4 types of water availability:

1. **City water (Municipal connection)** -- Standard municipal water connection. Requires payment of impact fee to the county. Dandara requests meter installation from the utility company. Most straightforward option with predictable costs and timeline.

2. **Well water (Private well)** -- No municipal water access; a private well must be drilled on the property. Requires separate well permits from the county and a water quality test before occupancy. Significant cost extra that triggers a client hold through Client Relations. Common in rural areas of Marion County.

3. **Community well (Shared well system)** -- A shared well system managed by an HOA or community association. Connection fees vary by community. Less common but found in some planned developments. HOA manages maintenance and water quality.

4. **Reclaimed water (Irrigation only)** -- Non-potable water for irrigation purposes only, delivered through purple pipe (industry standard color for reclaimed water). Separate system from potable water. Available in some newer developments. Cannot be used for drinking, cooking, or bathing.

### 4 Sewage Types

The sewage system determination is critical because it affects permit documentation, inspection requirements, and costs:

1. **City sewer (Municipal connection)** -- Public gravity-based sewer system. Requires payment of sewer impact fee. Connection handled by the utility company. Rare in Marion County but more common in urban areas of Citrus and Charlotte counties.

2. **Septic (On-site system)** -- Private septic tank and drain field installed on the property. Most common system in Marion County. Requires a perc test (soil percolation test) to determine suitability. Must maintain setback distance from any well on the property. Inspected by the Department of Health (DOH) inspector, not the county building inspector.

3. **Advanced Treatment Unit / ATU (Compact septic)** -- Also called "nitrogen removal" system. A more efficient septic variant required near water bodies or in environmentally sensitive areas. Higher cost than standard septic, triggering a client hold. Produces cleaner effluent to protect waterways.

4. **STEP system (Septic Tank Effluent Pumping)** -- Used in low-pressure sewer areas (LPS), primarily in Charlotte County. A hybrid between septic and municipal -- each property has a septic tank, but effluent is pumped to a shared treatment facility. Sometimes called "LPS" in internal documents.

### Portal Access Issues

County portals used for utility and permit lookups frequently change URLs. Some require login credentials. Accela-based portals (Marion County, Citrus County) are generally more reliable and stable. Lake County portal has intermittent downtime. When portals are down, Dandara must call the county directly for status updates, which significantly slows the process.

### Document Receipt from 3 Sources

Utilities receives critical documents from three distinct sources, each with different delivery methods and timelines:

1. **County portal** -- Permits, approvals, inspection results. Accessed via county-specific websites. Marion and Citrus use Accela portals; Charlotte uses a different system.
2. **Utility company** -- Connection letters, meter set dates, UAL (Utilities Availability Letter). Received via email. Each company has different response times (Duke Energy vs Seco vs FPL).
3. **Engineering firm** -- Load calculations, site plans, septic designs. Received via email from contracted engineers. Average turnaround: 5-7 days for standard items.

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- [Catalogo de Dores](07_CATALOGO_DORES.md)
- [Fluxo Spec Home](05_FLUXO_SPEC_HOME.md)
- [Fluxo Custom Home](06_FLUXO_CUSTOM_HOME.md)
- [Glossario de Termos](03_GLOSSARIO.md)
- **Departamentos relacionados:**
  - [Permits](dept_permits.md) — recebe notificacao de permit; fornece informacao sobre agua/esgoto
  - [Financeiro](dept_financeiro.md) — paga invoices e construction charges
  - [Client Relations](dept_client_relations.md) — recebe aprovacao do cliente para custos extras; fornece client holds
  - [Scheduling](dept_scheduling.md) — recebe informacao de tug side para RF Electric
  - [Core Craft](dept_core_craft.md) — remove dumpster para liberar tug; expoe tubulacao para inspecao

## Key Glossary Terms

> Terms from [Glossario de Termos](03_GLOSSARIO.md) most relevant to the Utilities department. (10 terms -- file near size limit)

- **UAL (Utilities Availability Letter)** / **Carta de Disponibilidade de Utilidades**: First step in utilities process -- defines available water/sewer options for the lot
- **Impact Fee** / **Taxa de Impacto**: County fee for infrastructure impact of new construction -- blocks Final Electric in Marion
- **Construction Charges** / **Taxas de Construcao**: Fees paid to county or utility company during construction -- usually within first draw
- **Septic** / **Sistema Septico**: Private sewage treatment system when no public sewer access -- conventional and nitrogen types
- **DOH (Department of Health)** / **Departamento de Saude**: Agency that inspects septic systems via delegated private soil engineer
- **Underground Electric** / **Fiacao Eletrica Subterranea**: Underground wiring from transformer to house electrical box -- triggers client hold if cost > $1,000 over budget
- **Tug Side** / **Lado da Caixa Eletrica**: Side of house for electrical panel installation -- critical info for RF Electric scheduling
- **LPS (Low Pressure System)** / **Sistema de Baixa Pressao**: Sewage system specific to Charlotte County -- mid-cost between septic and gravity
- **Client Hold** / **Paralisacao por Conta do Cliente**: Work stoppage notified to client due to extra cost (e.g., water line extension, nitrogen septic)
- **Drain** / **Drenagem**: House drainage system -- requires completed roughs and roof penetrations before inspection

---

## BuilderTrend Job 455 -- Real Data

### Utility Details on Job 455
| Utility | Provider | System | Monthly Cost |
|---------|----------|--------|-------------|
| Water | Marion County Utilities | Standard (municipal connection) | $13.50/month |
| Energy | SECO Energy | Standard | $43-$129/month |
| Sewer | Septic Tank | DOH-Marion approved | One-time: $4,600 (Leesburg Septic) |

### Utility Costs on Job 455
| Service | Vendor | Total Cost | Bills |
|---------|--------|-----------|-------|
| Electric | Seco Energy | $563.20 | 9 bills (May 2025 - Mar 2026) |
| Water | Marion County Utilities | $537.64 | 8 bills (Sep 2025 - Mar 2026) |
| Portable Toilet | WC America LLC | $612.39 | 4 bills |
| Sewer Connection | Leesburg Septic, INC | $4,600 | 1 bill |
| Septic Plan | Rapid Septic Consulting | $600 | 1 PO |
| Septic Inspection | Rapid Septic Consulting | $150 | 1 bill |
| **Total Utility Cost** | -- | **~$7,063** | -- |

### Water Cost Anomaly
October 2025 water bill was $456.64 (vs normal $13.50/month) -- likely construction water usage or connection fees during active construction.

### UAL (Utility Availability Letter) on Job 455
- UAL requested: Dec 18, 2024
- UAL received: Dec 20, 2024 (3 days)
- Responsible: Leonardo Fortini (Utilities department)
- Daily Log tag: #UT - UTILITIES AVAILABILITY LETTER CHECKLIST DONE

### Custom Fields in BuilderTrend for Job 455
- Energy Company: SECO
- Water Company: Marion County Utilities
- Water System: Standard
- Sewer System: Septic Tank
- Tug Side: Right

## CPM Construction Sequence -- Utilities Touchpoints

### Utility Activities in CPM FASE 1-3
| CPM Activity | Description | Timing |
|-------------|-------------|--------|
| WATER METER INSTALL | Company installs water meter | Early in process (variable -- utility company) |
| WATER LINE | Usually done with Underground Plumbing | FASE 2 (Foundation) |
| WATER SERVICE INSPECTION | Marion only (similar to Citrus Final Utilities) | FASE 4 |
| TUG INSTALL | Electrical meter can installation | After Framing (FASE 3) |
| TUG INSPECTION | Inspector verifies meter can | After TUG Install |
| SEPTIC INSTALL | Septic system installation | FASE 3 |
| DOH INSPECTION | Department of Health septic inspection | After Septic Install |
| SEPTIC COVER | Cover septic after DOH approval | After DOH approval |
| SEPTIC CONNECTION | Marion only | After Septic Cover |
| SEWER SEPTIC INSPECTION | Marion only | After Septic Connection |
| (COMPANY) UNDERGROUND ELECTRICAL | Utility company installs underground | FASE 4 |
| ELECTRICAL METER | Company installs; up to 3 days after Company UG | FASE 4 (variable) |

### County-Specific Utility Differences
| Aspect | Marion County | Citrus County |
|--------|--------------|---------------|
| Water Service Inspection | Yes | No (covered by Final Utilities) |
| Final Utilities Inspection | No | Yes (checks water line + meter) |
| Sewer Septic Inspection | Yes | No |
| DOH Inspection | No | Yes |
| Pre-Power Inspection | No | Yes |
| Nitrogen Septic | After Rough Electric | Standard |

### Critical Utility Dependencies from CPM
1. Dumpster must be removed before TUG install (CoreCraft dependency)
2. Dumpster must be removed to expose tubulation for septic inspection
3. Water Meter should already be installed by finish phase
4. Electrical Meter requires house painted externally with house number (variable date)
5. For Nitrogen Septic: must wait until after Rough Electric (needs electrical connection)

## Const App Integration

### Utility Module in Const App
- **Configurations**: 27 utility configurations across 7 categories:
  - Water System Types: Community Water, Municipal Water, Private Well
  - Sewage System Types: Advanced Septic, Disposal Septic, Gravity Sewer, Septic Tank
  - Energy Companies: FPL, Duke Energy, TECO
  - Water Companies: Broward County Water, JEA, Miami-Dade Water & Sewer, Toho Water Authority
  - Sewage Companies: County Wastewater Dept, Municipal Sewer
  - Additional Applications: Backflow Prevention, Capacity Letter, Demand Letter, DEP Permit, Grease Trap Letter, Well Permit
  - Septic Document Types: Perc Test Certificate, Septic Permit, Site Plan Acknowledgment

- **Water & Sewage Tracking**: Track UAL requests, water/sewage system types, additional documents per contract
- **Energy Tracking**: Track energy company assignments and costs for contracts with issued permits
- **Service Monitoring**: Track service execution status (Electric Connection, Sewer Connection, Water Connection, Water Usage)
- **Septic Documents**: Track document collection for projects with Septic Tank systems
- **Account Closing**: Track water and energy bill transfer status for project closure

### Utility Service Codes
| Code | Service |
|------|---------|
| UTL-001 | Water |
| UTL-002 | Sewage |
| UTL-003 | Energy |
| UTL-004 | Electric Connection |
| UTL-005 | Sewer Connection |
| UTL-006 | Water Connection |
| LTV-001 | Electric Connection (Lot) |
| LTV-002 | Sewer Connection (Lot) |
| LTV-003 | Water Connection (Lot) |
| LTV-004 | Water Usage |
