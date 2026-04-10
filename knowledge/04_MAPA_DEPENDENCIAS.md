# Mapa de Dependencias Interdepartamentais - Lakeshore Development

## Visao Geral

Este documento consolida as dependencias entre todos os 15 departamentos operacionais da Lakeshore Development. Os dados foram extraidos das secoes "## Dependencias" de cada arquivo departamental. O objetivo e oferecer uma visao unica de quem depende de quem, o que e trocado em cada relacao e onde ocorrem os pontos criticos de handoff.

Departamentos cobertos: Orcamento, Compras, Financeiro, Scheduling, Supervisao, Inspecao, Warranty, Takeoff, Permits, Land Acquisition, Client Relations, Utilities, Core Craft, RH, Escritorio de Projetos.

---

## Matriz de Dependencias

Legenda das celulas:
- **DOC** = Documento (planta, relatorio, planilha, contrato)
- **INFO** = Informacao operacional (status, confirmacao, dado)
- **APROV** = Aprovacao (autorizacao, checklist, liberacao)
- **$** = Transacao financeira (pagamento, PO, invoice)
- **-** = Sem dependencia direta identificada

Linhas = Departamento que **entrega**. Colunas = Departamento que **recebe**.

| Entrega / Recebe | Orcamento | Compras | Financeiro | Scheduling | Supervisao | Inspecao | Warranty | Takeoff | Permits | Land | Client Relations | Utilities | Core Craft | RH | Esc. Projetos |
|-----------------|-----------|---------|------------|------------|------------|----------|----------|---------|---------|------|-----------------|-----------|------------|-----|---------------|
| **Orcamento** | - | DOC | DOC/$ | INFO | - | - | - | - | - | - | - | - | - | - | - |
| **Compras** | - | - | $/INFO | INFO | - | - | - | - | - | - | - | - | DOC | - | - |
| **Financeiro** | - | - | - | INFO | - | INFO | $ | - | $ | - | INFO | $ | - | INFO | - |
| **Scheduling** | - | INFO | INFO | - | INFO | INFO | - | - | - | - | - | - | INFO | - | - |
| **Supervisao** | - | - | APROV | INFO | - | APROV | INFO | - | - | - | - | - | - | - | - |
| **Inspecao** | - | - | INFO | INFO | INFO | - | INFO | - | - | - | - | INFO | - | - | - |
| **Warranty** | - | - | $ | - | - | - | - | - | - | - | INFO | - | - | - | - |
| **Takeoff** | DOC | DOC | - | INFO | - | - | - | - | DOC | - | - | - | - | - | - |
| **Permits** | - | - | $ | - | DOC | - | - | - | - | - | INFO | INFO | - | - | DOC |
| **Land** | - | - | - | - | - | - | - | DOC | DOC | - | - | - | - | - | DOC |
| **Client Relations** | - | - | APROV | - | - | - | INFO | - | DOC | - | - | APROV | - | - | - |
| **Utilities** | - | - | $ | INFO | - | - | - | - | INFO | - | INFO | - | INFO | - | - |
| **Core Craft** | - | DOC | $ | - | - | - | - | - | - | DOC | - | INFO | - | - | - |
| **RH** | - | - | INFO | - | - | - | - | - | - | - | - | - | - | - | - |
| **Esc. Projetos** | DOC | DOC | - | - | DOC | - | - | DOC | DOC | - | INFO | - | - | - | - |

---

## Detalhamento por Departamento

### Orcamento / Budget

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Escritorio de Projetos (Camila) | Takeoff, design book, specification sheet, floor plans | DOC |
| Takeoff (Gabriela) | Quantidades de materiais para cotacao e calculo de custo | DOC |
| Permits | Definicao de full MAP, condado | INFO |
| Client Relations (Camila) | Definicao de allowance, by owner, upgrades | INFO |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Compras (Brenda) | Base para compras de materiais (lista e valores) | DOC |
| Scheduling | Budget como referencia para pedidos de material | INFO |
| Financeiro | Valores de referencia de POs e budgets | $ |
| Contratos (Bruna) | Cotacoes selecionadas como base para contratos | DOC |

**Pontos de handoff criticos:**
- Takeoff deve estar pronto antes do orcamento; atrasos geram bloqueio em cadeia
- Budget customizado deve estar fechado antes de assinar contrato com cliente
- Budget nao notifica automaticamente equipe de compras quando takeoff muda

---

### Compras / Purchasing

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Orcamento/Budget | Takeoff e budget como base para compras | DOC |
| Escritorio de Projetos | Takeoff, specification sheet | DOC |
| Scheduling | Agendamento de servicos e pedidos de entrega | INFO |
| Field/Supervisao | Compras emergenciais com cartao corporativo | $ |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Financeiro | Replicacao no Builder Trend, rateio de materiais, invoices | $/INFO |
| Scheduling | Materiais disponiveis no armazem | INFO |
| Core Craft | Materiais para entregas de appliances e outros | DOC |
| Field/Obra | Materiais para construcao | DOC |

**Pontos de handoff criticos:**
- Takeoff inconsistente gera compras erradas (problema recorrente)
- Saidas de material do armazem precisam ser registradas com destino por casa

---

### Financeiro (Contas a Pagar + Receber)

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Scheduling | Confirmacao de servico realizado (checklist done) para liberar pagamento | APROV |
| Orcamento/Budget | Valores de referencia de POs e budgets | $ |
| Compras | Registro de compras, rateio de materiais | INFO |
| Contratos (Bruna) | Atualizacoes contratuais de valores | DOC |
| Permits (Cacia) | Notificacao de contrato assinado, taxas de permit | INFO |
| Utilities (Dandara) | Contas de utilities para pagamento, invoices | $ |
| Field | Recibos de compras emergenciais | INFO |
| C-Level (Leo, Samuel, Moises) | Aprovacoes de pagamento, confirmacao de valores | APROV |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Fornecedores/Subs | Pagamentos processados | $ |
| C-Level | Relatorios financeiros (DRE, balanco, T99) | DOC |
| Quickbooks | Registros contabeis e conciliacao | INFO |
| Permits | Pagamento do permit e builders risk | $ |
| Utilities | Pagamento de invoices de abertura de conta | $ |

**Pontos de handoff criticos:**
- Checklist done do Scheduling e o gatilho de pagamento a subs — falha aqui = pagamento indevido ou atraso
- Notificacao de contrato assinado (Permits -> Financeiro) aciona draws de contas a receber
- Aprovacao de Leo e obrigatoria para qualquer pagamento sair

---

### Scheduling

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Supervisores/Monitores | Confirmacao de elevacao, calculo de loads, verificacao de servicos | INFO/APROV |
| Financeiro | Draws (liberacao financeira para avancar na obra) | INFO |
| Permits | Liberacao para inicio de construcao | APROV |
| Budget/Takeoff | Informacoes de materiais e quantidades | INFO |
| Compras/Warehouse | Materiais disponiveis no armazem | INFO |
| Client Relations | Informacoes de customizacao do cliente | INFO |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Financeiro | Confirmacao de servico realizado (checklist done) para pagamento | APROV |
| Supervisao | Informacoes de agendamento para acompanhamento | INFO |
| Inspecao | Solicitacoes de inspecao (via Slack) quando servico concluido | INFO |
| Compras | Pedidos de material | INFO |

**Pontos de handoff criticos:**
- Primeiro e segundo draws do Financeiro sao gatilhos de liberacao de fases 1 e 2
- Survey Received (Permits) e a tag que indica nova casa disponivel para o scheduler
- Checklist done e marcado pelo monitor — erro aqui dispara pagamento indevido

---

### Supervisao / Field

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Scheduling | Informacoes de agendamento, servicos a verificar | INFO |
| Inspecao | Resultados de inspecoes (aprovadas/reprovadas) | INFO |
| QPS (Don/Fortine) | Padroes de qualidade a verificar | DOC |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Scheduling | Confirmacao de elevacao do pad, calculo de loads, apoio operacional | INFO |
| Financeiro | Checklist done (gatilho de pagamento ao sub) | APROV |
| Inspecao | Verificacao previa de qualidade antes de agendar inspecao | APROV |
| Warranty | Verificacao in loco em casas em periodo de garantia (Daniel) | INFO |

**Pontos de handoff criticos:**
- Calculo de loads e um gargalo critico: falta de equipamento atrasa toda a fase 1
- Checklist done precisa ser criterioso — sub pago nao volta para arrumar
- Supervisores frequentemente solicitam reparos sem criar PO, causando problema no Financeiro

---

### Inspecao

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Scheduling | Solicitacoes de inspecao (canal Slack) quando servico esta concluido | INFO |
| Supervisao/Field | Verificacao previa de qualidade antes de agendar inspecao | APROV |
| Financeiro | Pagamento de fees e impact fees que desbloqueiam inspecoes | $ |
| Permits | Status de holds, permit number para agendamento | INFO |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Scheduling | Resultados (aprovada = proximo passo; reprovada = rework) | INFO |
| Supervisao | Notificacao de reprovacoes para resolucao em campo | INFO |
| Financeiro | Informacao de fees necessarias para reinspecao | INFO |
| Warranty | Inspecoes finais aprovadas (CO) necessarias para closing | INFO |

**Pontos de handoff criticos:**
- Impact fees do Financeiro bloqueiam Final Electric em Marion — dependencia critica
- Hold de inspecao para toda a casa ate resolucao — nao ha notificacao automatica de remocao
- Frame inspection e o ponto mais critico da Fase 2: exige todos os roughs aprovados

---

### Warranty / Closing

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Client Relations (CR) | Autorizacao para corte de grama em casas fechadas | APROV |
| Financeiro | Pagamento quando garantia do sub expira | $ |
| Supervisores (Daniel) | Verificacao in loco em casas de warranty | INFO |
| Data Loggers/Monitores | Relato de necessidade de corte de grama | INFO |
| QPS (Don/Fortine) | Padroes de qualidade para verificacao | DOC |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Subs | Encaminhamento de solicitacoes de reparo | INFO |
| Financeiro | POs de reparos e cortes de grama | $ |
| Client Relations | Status de reparos para comunicacao com cliente | INFO |
| Taylane (interno) | Casas prontas para venda apos reparos de closing | APROV |

**Pontos de handoff criticos:**
- Data de inicio da garantia = data de ocupacao/venda (nao mais a partir do CO)
- Sub pago durante construcao tem prazo proprio de garantia (1 ano a partir do fim do servico) — conflito com regra da empresa
- Reparos sem valores fixos — sub descobre extensao no local

---

### Takeoff

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Engenheiro externo | Projeto executivo (PDF) | DOC |
| Escritorio de Projetos (Camila) | Floor plan, design book, spec sheet | DOC |
| Sub de trusses | Trusses layout necessario para takeoff preciso | DOC |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Orcamento/Budget (Felipe, Pedro, Ana Helena) | Quantidades de materiais para cotacao e budget | DOC |
| Compras/Purchasing (Brenda) | Lista de materiais para compra | DOC |
| Scheduling (Mauricio) | Informacoes de materiais e quantidades a partir da fase de blocos | INFO |
| Permits | Floor plan e documentos para aplicacao de permit | DOC |

**Pontos de handoff criticos:**
- Takeoff depende do projeto executivo finalizado pelo engenheiro — pode atrasar toda a cadeia
- Mudancas de takeoff nao notificam automaticamente o Budget — risco de orcamento desatualizado
- Para customs: cada mudanca do cliente requer novo takeoff

---

### Permits / Documentacao

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Financeiro | Pagamento do permit e builders risk | $ |
| Escritorio de Projetos (Camila) | Floor plans e dados do projeto | DOC |
| Utilities (Dandara) | Informacao sobre sistema de agua/esgoto (septic vs gravity) | INFO |
| Surveyors (subs) | Survey e documentacao base | DOC |
| Subs de energia e engenharia | Energy calculations, trusses | DOC |
| Client Relations | Assinatura do cliente para NOC | DOC |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Campo/Supervisores | Pasta com documentos stamp aprovados para construcao | DOC |
| Client Relations | Status de permits para informar clientes | INFO |
| Utilities | Permit number e informacoes do projeto | INFO |
| Financeiro | Solicitacao de pagamento de permits e builders risk | $ |

**Pontos de handoff criticos:**
- Survey e prerequisito obrigatorio para todos os demais documentos de permit
- Pagamento do Financeiro e necessario antes de emitir permit — bloqueador de campo
- Informacao de sistema septico/gravity de Utilities impacta documentacao necessaria

---

### Land Acquisition / Land Development

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Clientes/Mercado | Leads e oportunidades de terrenos | INFO |
| Engenheiros civis | Projetos de infraestrutura | DOC |
| Prefeitura | Aprovacao de permits de land development | APROV |
| Subcontratados | Execucao de site work | INFO |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Building/Construcao vertical | Area com infraestrutura completa pronta para construir casas | INFO |
| Escritorio de Projetos | Informacoes do terreno para desenvolvimento de plantas | INFO |
| Permits | Dados do land development que impactam permits de construcao | DOC |

**Pontos de handoff criticos:**
- Entrega do terreno com infraestrutura completa e o handoff mais critico: marca transicao de land para building
- Infraestrutura subterranea (esgoto, agua, ruas) deve estar aprovada antes do inicio de construcao vertical

---

### Client Relations

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Scheduling Team | Informacoes sobre etapas e prazos das casas | INFO |
| Supervisores/PMs | Informacoes de campo, status da obra | INFO |
| Financeiro | Atualizacao do budget, revisao de valores | INFO |
| Utilities (Dandara) | Informacoes de custos extras (client holds) | INFO |
| Permits | Status de permits para informar clientes | INFO |
| Todos os setores | Informacoes diversas conforme demanda | INFO |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Clientes | Informacoes de status, respostas a duvidas, comunicacao de custos | INFO |
| Close Team | Projetos na fase de entrega | INFO |
| Financeiro | Aprovacao de custos extras pelo cliente | APROV |
| Utilities | Confirmacao de aprovacao do cliente para custos extras | APROV |
| Permits | Assinatura do cliente para NOC e outros documentos | DOC |

**Pontos de handoff criticos:**
- CR e o unico ponto de contato com cliente — informacoes imprecisas geram atritos
- Aprovacao do cliente para custos extras (client holds) bloqueia prosseguimento de Utilities
- Upgrades do cliente podem se perder se nao registrados e acompanhados no Builder Trend

---

### Utilities

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Builder Trend / Slack | Notificacao de novo jobsite (gatilho para agua/esgoto) | INFO |
| Permits | Notificacao de permit recebido (gatilho para energia), permit number | INFO |
| Financeiro | Pagamento de invoices, construction charges | $ |
| Supervisores/Monitores | Verificacao em campo de medidores, stakes, conexoes | INFO |
| Core Craft (Services) | Remocao de dumpster, exposicao de tubulacao para inspecao | INFO |
| Client Relations | Aprovacao do cliente para custos extras | APROV |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Permits | Informacao sobre sistema de agua/esgoto (septic vs gravity) | INFO |
| Client Relations | Informacoes de custos extras para comunicar ao cliente (client holds) | INFO |
| Financeiro | Invoices de abertura de conta, POs | $ |
| Scheduling | Informacao de tug side para RF Electric | INFO |
| Campo/Supervisores | Informacoes sobre instalacoes agendadas | INFO |

**Pontos de handoff criticos:**
- Tug side errado = custo adicional significativo — informacao critica para o Scheduling
- Permit recebido (de Permits) e o gatilho para abertura de conta de energia
- Client hold de extensao de agua/esgoto pode paralisar o projeto se cliente recusar pagar

---

### Core Craft

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Scheduling Team | Principal solicitante de servicos (via Slack) | INFO |
| Supervisores | Solicitacoes pontuais e urgencias | INFO |
| Land Development | Servicos especificos de terreno | INFO |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Financeiro | Invoices para pagamento (via sistema Zorro) | $ |
| Compras | Invoices de appliances | DOC |
| Land Development | Servicos de terreno executados | INFO |
| Utilities | Remocao de dumpster para liberacao de tug, exposicao de tubulacao | INFO |
| Campo/Supervisores | Servicos concluidos (limpeza, preparacao, materiais) | INFO |

**Pontos de handoff criticos:**
- Dumpster impede servicos de tug install e septic install — coordenacao com Utilities essencial
- Valores de servicos frequentemente indefinidos antes da execucao — retrabalho financeiro
- CUT sem remocao de material gerava atraso na sequencia de servicos

---

### Recursos Humanos (RH)

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Todos os setores | Lideres agendam PTOs e sick days de seus liderados via Google Calendar | INFO |
| Administracao | Informacoes de contratacao, datas de inicio, contratos especiais | DOC |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Todos os setores | Informacao de saldo de PTOs e sick days | INFO |
| Financeiro | Informacoes de faltas e ausencias para folha de pagamento | INFO |
| Lideres | Visibilidade sobre disponibilidade de suas equipes | INFO |

**Pontos de handoff criticos:**
- Agendamentos de dias passados nao notificam automaticamente — dependente do lider avisar manualmente
- Lider pode agendar PTO sem verificar saldo disponivel — falta controle visivel

---

### Escritorio de Projetos (Design Office)

**Recebe de:**
| Origem | O que recebe | Tipo |
|--------|-------------|------|
| Clientes | Solicitacoes de projetos custom, preferencias, aprovacoes | INFO |
| CEO (Bernardo) e Leo | Decisoes de portfolio, aprovacao de budgets | APROV |
| Engenheiros externos | Projeto executivo (retorno para takeoff) | DOC |

**Entrega para:**
| Destino | O que entrega | Tipo |
|---------|--------------|------|
| Budget/Orcamento (Samuel) | Plantas, spec sheets, design books para criacao de budgets | DOC |
| Permits (Cassia/Kaio) | Floor plans para aplicacao de permits | DOC |
| Execucao (Cris) | Contrato assinado + todos documentos para inicio da obra | DOC |
| Client Relations | Informacoes de projeto para comunicacao com clientes | INFO |
| Purchasing/Compras | Quantidades do takeoff para compras | DOC |
| Field/Supervisores | Plantas atualizadas e especificacoes | DOC |

**Pontos de handoff criticos:**
- Planta arquitetonica e o documento raiz — tudo depende dela (budget, permits, takeoff, compras)
- Mudancas de planta durante a obra nao sao bem comunicadas para campo e PMs — risco alto
- Pre-contrato com cliente nao tem tracking formal — projetos podem se perder

---

## Pontos de Handoff Criticos (Consolidado)

Os handoffs a seguir representam os pontos de maior risco de atraso ou perda de informacao no fluxo operacional da Lakeshore.

| # | Handoff | De | Para | Por que e critico |
|---|---------|-----|------|-------------------|
| H-01 | Checklist Done (servico concluido) | Supervisao/Monitores | Financeiro / Scheduling | Gatilho direto de pagamento. Marcacao incorreta = pagamento indevido, sub nao volta para arrumar |
| H-02 | Liberacao de Draws | Financeiro | Scheduling | Bloqueio por fase: 1o draw libera ate Robintec; 2o draw libera resto da Fase 1; 4o draw libera Fase 2. Obra para sem draw |
| H-03 | Survey Received (tag BT) | Permits | Scheduling | Sem essa tag, Scheduling nao sabe que nova casa existe. Casa fica em espera indefinida |
| H-04 | Planta Arquitetonica | Escritorio de Projetos | Budget / Permits / Takeoff / Compras | Documento raiz. Atraso ou versao errada contamina toda a cadeia downstream |
| H-05 | Takeoff de Materiais | Takeoff (Gabriela) | Budget / Compras | Base quantitativa para orcamento e compras. Revisoes sem notificacao geram dados desatualizados |
| H-06 | Aprovacao de Permit | Permits | Campo / Scheduling / Financeiro | Sem permit, construcao nao pode comecar em condados exigentes (ex: Citrus). Documentos stamp devem chegar ao campo |
| H-07 | Notificacao de Contrato Assinado | Permits | Financeiro | Aciona cobranca de draws. Atraso na notificacao = atraso no fluxo de recebimento |
| H-08 | Resultado de Inspecao | Inspecao | Scheduling / Supervisao | Aprovacao = proximo passo. Reprovacao = rework. Holds param toda a casa sem aviso automatico de remocao |
| H-09 | Informacao de Tug Side | Utilities | Scheduling | Critico para RF Electric. Instalacao no lado errado = custo adicional e reagendamento |
| H-10 | System de Agua/Esgoto (Septic/Gravity) | Utilities | Permits | Define documentacao necessaria para o permit. Ausencia desta informacao atrasa aplicacao |
| H-11 | Client Hold (custo extra) | Utilities / Permits | Client Relations | Cliente deve aprovar custo extra antes de prosseguir. Sem aprovacao, servico fica parado |
| H-12 | Calculo de Loads | Supervisao | Scheduling | Gargalo na Fase 1. Falta de equipamento atrasa pad, compact test e form em sequencia |
| H-13 | Inspecoes Finais Aprovadas (CO) | Inspecao | Warranty / Closing | Sem CO, casa nao pode ser entregue. Impact fees do Financeiro podem bloquear Final Electric |
| H-14 | Entrega de Terreno (Land -> Building) | Land Acquisition | Scheduling / Permits / Escritorio de Projetos | Transicao formal: land development encerra, building comeca. Infraestrutura subterranea deve estar aprovada |
| H-15 | Aprovacao de Budget pelo Cliente (Custom) | Escritorio de Projetos + Budget | Client Relations | Sem aprovacao, nao ha contrato. Ciclo todo do custom home depende desta aprovacao |

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Organograma](01_ORGANOGRAMA.md)
- [Inventario de Ferramentas](02_INVENTARIO_FERRAMENTAS.md)
- [Glossario de Termos](03_GLOSSARIO.md)
- [Fluxo Spec Home](05_FLUXO_SPEC_HOME.md)
- [Fluxo Custom Home](06_FLUXO_CUSTOM_HOME.md)
- [Catalogo de Dores](07_CATALOGO_DORES.md)
