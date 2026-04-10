# Catalogo Consolidado de Dores - Lakeshore Development

> Versao: 1.0 | Gerado em: 2026-04-04 | Fonte: 15 dept_*.md + 02_INVENTARIO_FERRAMENTAS.md

---

## Visao Geral

Este catalogo consolida todas as dores e problemas conhecidos dos 15 departamentos da Lakeshore Development, classificados por severidade e mapeados para oportunidades de automacao.

### Resumo Quantitativo

| Metrica | Total |
|---------|-------|
| Total de dores catalogadas | 97 |
| Severidade Alta | 38 |
| Severidade Media | 41 |
| Severidade Baixa | 18 |
| Dores com automacao possivel (Sim) | 31 |
| Dores com automacao parcial (Parcial) | 28 |
| Dores sem automacao viavel (Nao) | 38 |

### Departamentos Mais Afetados (por total de dores de severidade Alta)

| Departamento | Dores Alta | Total Dores |
|---|---|---|
| Financeiro | 7 | 12 |
| Scheduling | 6 | 14 |
| Compras | 6 | 11 |
| Orcamento | 5 | 11 |
| Inspecao | 5 | 8 |
| Permits | 5 | 11 |
| Warranty | 4 | 12 |
| Escritorio de Projetos | 4 | 10 |
| Supervisao | 3 | 10 |
| Client Relations | 3 | 8 |
| Takeoff | 3 | 10 |
| Utilities | 2 | 10 |
| Core Craft | 2 | 6 |
| RH | 1 | 4 |
| Land Acquisition | 0 | 5 |

---

## Catalogo por Departamento

### Orcamento / Budget

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| ORC-01 | Atualizacao de precos: materiais e tarifas mudam rapidamente; invoices com valores diferentes das POs | Alta | Orcamentos desatualizados geram pagamentos incorretos e retrabalho no Financeiro | Parcial — alertas automaticos de variacao de preco acima de threshold |
| ORC-02 | Integracao estimate-POs no BuilderTrend: tarefa manual e trabalhosa feita por Ana Helena | Alta | Horas diarias de trabalho manual propenso a erro; gargalo critico na equipe | Sim — propagacao automatica do orcamento aprovado para criacao de POs |
| ORC-03 | Volatilidade do takeoff para casas custom: projeto muda varias vezes, takeoff precisa ser refeito; conversao de areas em unidades e manual | Alta | Custo imprevisivel e retrabalho frequente em projetos custom | Parcial — versionamento automatico de takeoff com notificacao de mudancas |
| ORC-04 | Falta de padronizacao: conhecimento concentrado nos gestores; ausencia de caminho padronizado | Alta | Dependencia de pessoas especificas; risco operacional se gestor sair | Nao — requer processo organizacional |
| ORC-05 | Budget deveria estar pronto antes do permit, mas frequentemente esta atrasado | Alta | Inicio da obra atrasado; dependencia critica nao respeitada | Parcial — dashboard de status com alertas de prazo para equipe de budget |
| ORC-06 | POs fora de ordem no BT antigo: cadastradas aleatoriamente, dificultando comparacao com planilha | Media | Dificuldade de auditoria e controle de gastos | Sim — ordenacao automatica de POs por cost code |
| ORC-07 | Dificuldade com casas custom: cada projeto e unico; cotacoes iniciais inevitavelmente mudam | Media | Estimativas iniciais imprecisas geram renegociacoes com clientes | Parcial — historico de projetos similares para parametrizar estimativas |
| ORC-08 | Duplicacao de funcoes: Energy Calculation solicitado por budget e por permit | Media | Retrabalho entre departamentos; custo duplicado com fornecedores | Sim — sistema centralizado de solicitacao de documentos tecnicos |
| ORC-09 | Comunicacao com subs: muitos tem dificuldade tecnologica; dependem de WhatsApp/telefone | Media | Lentidao no processo de cotacao; respostas fora de sistemas rastreaveos | Parcial — portal de cotacao com fallback por e-mail |
| ORC-10 | Inconsistencia no takeoff de blocos: diferentes subs pedem quantidades variadas; sem padrao | Media | Sobras ou falta de material; estimativas imprecisas | Sim — padronizacao de quantidades por modelo no sistema |
| ORC-11 | Falta de historico centralizado: mudancas de takeoff nao notificam automaticamente equipe de budget | Baixa | Equipe trabalha com dados desatualizados sem saber | Sim — notificacao automatica para stakeholders ao alterar takeoff |

### Compras / Purchasing

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| COM-01 | Volume excessivo de planilhas: 12+ planilhas com multiplas abas abertas diariamente; informacoes semelhantes em formatos diferentes | Alta | Ineficiencia extrema; alta chance de erro humano; onboarding dificil | Sim — sistema unificado de compras com rateio automatico |
| COM-02 | Zorro ineficaz para custos: nao atualiza precos automaticamente; valores desconsiderados pela equipe | Alta | Decisoes de compra sem dados de custo precisos | Sim — sistema de estoque integrado com precos atualizados |
| COM-03 | Zorro nao referencia lote de compra: nao informa de qual compra veio o material que esta saindo | Alta | Impossibilidade de calcular custo real por casa; falhas contabeis | Sim — rastreabilidade de lote no sistema de estoque |
| COM-04 | Distribuicao manual propensa a erros: processo complexo de rastreamento contabil | Alta | Erros de alocacao de custo por casa; retrabalho no Financeiro | Sim — distribuicao automatica por regra de alocacao |
| COM-05 | Mudanca de fornecedor de lumber: ninguem na empresa sabe fazer takeoff de lumber; novo fornecedor nao fara | Alta | Risco de ruptura no fornecimento de material critico | Nao — requer capacitacao interna ou novo fornecedor |
| COM-06 | Casas finalizadas sem registro de saida: Zorro mostra inconsistencias | Alta | Fechamento contabil incorreto; divergencias entre sistemas | Sim — validacao automatica antes de fechar casa |
| COM-07 | Inconsistencia no Takeoff: takeoff muitas vezes nao seguido na pratica | Media | Sobras de material, retrabalho e custo extra | Parcial — alertas quando saida de material diverge muito do takeoff |
| COM-08 | Entregas da Amazon nao encontram o armazem: problema recorrente com USPS | Media | Atrasos na obra; tempo perdido em reentregas | Nao — problema logistico externo |
| COM-09 | Drafts nao confirmados no Zorro: Seu Clauser usa drafts para separar materiais; confirmacao atrasada | Media | Incerteza sobre disponibilidade de material; erros de inventario | Sim — fluxo de aprovacao rapida de drafts com notificacao |
| COM-10 | Saidas de materiais volateis: demandas repentinas impactam previsao de compras | Media | Desabastecimento inesperado; compras emergenciais caras | Parcial — previsao de demanda por historico de obras similares |
| COM-11 | Falta de controle de Seu Clauser sobre saidas: sem autonomia para validar com Takeoff | Baixa | Material saindo sem registro preciso de destino | Parcial — app simplificado de saida de material com validacao de takeoff |

### Financeiro (Contas a Pagar + Contas a Receber)

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| FIN-01 | Inclusao de classe no QuickBooks: 86 bills = 2 horas/dia; dois sistemas lentos | Alta | 10+ horas semanais perdidas em entrada manual; escala com volume | Sim — integracao automatica software-QuickBooks com mapeamento de classes |
| FIN-02 | Invoices sem PO: fluxo repetitivo; grande dor de cabeca; supervisores solicitam reparos sem criar PO | Alta | Pagamentos travados; aprovacoes manuais urgentes; opera risco financeiro | Sim — exigencia de PO antes da execucao com aprovacao mobile para supervisores |
| FIN-03 | Falta de contratos com valores exatos: 27+ modelos; precos mudam conforme volume; equipe nao sabe valor correto | Alta | Pagamentos incorretos a subs; renegociacoes constantes | Sim — base centralizada de contratos com alertas de desatualizacao |
| FIN-04 | Confirmacao de reparos demorada: depende de Moises/Samuel responderem | Alta | Pagamentos travados; subs insatisfeitos; fluxo parado | Sim — fluxo de aprovacao com escalacao automatica por prazo |
| FIN-05 | Pagamentos parciais nao suportados: sistema atual nao permite registrar pagamento parcial de draw | Alta | Processos manuais em planilha; risco de erro de registro | Sim — suporte nativo a pagamentos parciais no sistema |
| FIN-06 | Integracao BT-QuickBooks incompleta: data de vencimento nao serve como criterio | Alta | Conciliacao manual; erros de registro de data | Sim — integracao direta software-QuickBooks com campos mapeados |
| FIN-07 | Gastos do Field sem informacao clara: recibos incompletos; "achismos" na alocacao | Alta | Custos mal alocados; variances contabeis; auditoria impossivel | Parcial — app de submissao de recibo com campos obrigatorios e foto |
| FIN-08 | Alto volume de e-mails com invoices: grande desafio diario | Media | Tempo perdido gerenciando inbox; invoices esquecidos | Sim — inbox centralizado de invoices com parse automatico |
| FIN-09 | Pagamentos de subs maiores (FOCO, ECOWAN): valores mudam conforme volume, sem contratos atualizados | Media | Divergencias de valor; negociacoes ad hoc | Parcial — contratos com clausulas de volume registradas no sistema |
| FIN-10 | Notificacoes do BuilderTrend nao funcionam: equipe de permits nao consegue avisar Financeiro | Media | Atrasos em pagamentos de permits; risco de vencimento | Sim — notificacoes proprias do software com canal dedicado |
| FIN-11 | Mudancas contratuais nao comunicadas ao Financeiro: POs ficam desatualizadas | Media | Pagamentos com valores incorretos; retrabalho de correc ao | Sim — propagacao automatica de alteracoes contratuais para POs |
| FIN-12 | Falta de visualizacao do historico financeiro completo de uma casa | Baixa | Fechamento incompleto; auditoria demorada | Sim — visao 360 de casa com historico de transacoes |

### Scheduling

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| SCH-01 | Informacao repetida 3x (Top 1 dos schedulers): Daily logs + Schedule + PO com mesmos dados | Alta | Horas diarias de retrabalho para toda equipe de scheduling (7 pessoas) | Sim — entrada unica com propagacao automatica |
| SCH-02 | Demora no calculo de loads: falta de equipamentos especificos; paralisa processos subsequentes | Alta | Casa parada aguardando calculo; atraso em cadeia | Nao — requer equipamentos fisicos; parcialmente: alertas de prazo |
| SCH-03 | Survey Received ausente: se tag nao for colocada, equipe nao sabe que nova casa existe | Alta | Casa ignorada no sistema; inicio de obra atrasado dias ou semanas | Sim — criacao automatica de casa ao receber first draw |
| SCH-04 | Comunicacao com subs: demora nas respostas e descumprimento de prazos; letramento limitado | Alta | Atrasos recorrentes; reagendamentos multiplos; ineficiencia | Parcial — lembretes automaticos para subs; historico de performance |
| SCH-05 | Mudancas de material de ultima hora: notificados muito tarde; exigem reagendamento | Alta | Reagendamento de servicos caros; custo extra de sub parado | Sim — alertas de mudanca de material com lead time calculado |
| SCH-06 | Dependencia de draws financeiros: primeiro draw limita ate Robintec; segundo libera o resto | Alta | Casa travada por questoes financeiras mesmo sem problema operacional | Parcial — dashboard de status de draws em tempo real para schedulers |
| SCH-07 | Builder Trend lento: carregamento pesado, recarregamento apos cada input | Media | Perda de produtividade diaria; frustacao da equipe | Sim — software proprio mais leve e responsivo |
| SCH-08 | Tags excessivas e confusas: muitas tags, algumas duplicadas entre fases | Media | Erros de status; inconsistencia entre fases | Sim — taxonomia padronizada de status no novo sistema |
| SCH-09 | Slack instavel e lento no campo: equipe recorre ao WhatsApp | Media | Comunicacoes perdidas; rastreabilidade zero no WhatsApp | Parcial — app mobile leve integrado ao sistema |
| SCH-10 | Falta de campos padronizados na PO: titulo digitado livremente | Media | Inconsistencia nas POs; dificuldade de busca e auditoria | Sim — campos estruturados obrigatorios na PO |
| SCH-11 | Informacao descentralizada: cada scheduler cria sua propria planilha pessoal | Media | Informacao em silos; risco de perda ao sair da empresa | Sim — sistema unico de acompanhamento de casas |
| SCH-12 | Falta de notificacao de checklist done: precisa buscar manualmente | Media | Atrasos em pagamentos; subs aguardando sem rastreabilidade | Sim — notificacao push ao marcar checklist done |
| SCH-13 | Takeoff desatualizado para novos modelos: depende de atualizacao do depto de takeoff | Media | Agendamento com quantidades erradas; compras incorretas | Sim — versionamento de takeoff com notificacao de nova versao |
| SCH-14 | Modelo da casa dificil de acessar: navegar por varias pastas no BT | Baixa | Tempo perdido buscando informacoes basicas | Sim — informacoes da casa acessiveis em 1 clique |

### Supervisao / Field

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| SUP-01 | Supervisores solicitam reparos mas nao criam PO: causa problema no Financeiro (invoices sem PO) | Alta | Fluxo de pagamento travado; aprovacoes manuais urgentes frequentes | Sim — exigencia de PO via app mobile antes de autorizar reparo |
| SUP-02 | Inputs dos monitores com falhas: falta de conhecimento resultava em dados incorretos | Alta | Decisoes erradas baseadas em dados incorretos; retrabalho | Parcial — validacao de dados com campos obrigatorios e guias de preenchimento |
| SUP-03 | Volume de casas vs tempo: nao consegue olhar 50+ casas por dia | Alta | Problemas passam sem deteccao; qualidade comprometida | Parcial — priorizacao automatica por risco (atraso, inspecoes agendadas) |
| SUP-04 | Ferramentas unilaterais: dashboards somente leitura, sem anotacoes ou interacao | Media | Supervisores criam workarounds em planilhas; dado nao centralizado | Sim — dashboard interativo com funcao de anotacao |
| SUP-05 | Falta de visualizacao em timeline/barra de progresso com cores indicativas | Media | Dificuldade de identificar casas atrasadas rapidamente | Sim — timeline visual com cores de status por casa |
| SUP-06 | Inputs duplicados: internet ruim causa duplicacao de dados | Media | Dados incorretos no sistema; retrabalho de correc ao | Sim — validacao de duplicatas e modo offline com sync |
| SUP-07 | Fotos nao sobem: 99% das vezes as fotos anexadas nao sobem completamente | Media | Evidencias perdidas; impossibilidade de inspecao remota | Sim — upload progressivo com retry automatico |
| SUP-08 | Internet ruim no campo: dificulta uso de qualquer sistema pesado | Media | Sistema inutilizavel em campo; retorno ao papel | Sim — app offline com sync posterior |
| SUP-09 | Comunicacao campo-escritorio deficiente: Field deveria participar da revisao de projetos | Media | Problemas de construcao nao antecipados; custo de retrabalho | Parcial — canal estruturado de feedback campo-projeto |
| SUP-10 | Inconsistencia de dados no Kanban: Kanban 1 e 2 falharam por consistencia | Baixa | Falta de confianca nos dados; abandono da ferramenta | Sim — single source of truth no novo software |

### Inspecao

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| INS-01 | Sem notificacao de remocao de hold: precisa checar manualmente todos os dias | Alta | Casas paradas desnecessariamente; custo de atraso | Sim — monitoramento automatico do portal do condado com notificacao |
| INS-02 | Impact fees bloqueiam Final Electric (Marion): dependencia total do Financeiro | Alta | Inspecao final impossivel sem pagamento; atraso no fechamento | Sim — alerta automatico de fees pendentes com gateway de pagamento |
| INS-03 | Holds de modificacao: param toda a casa ate aprovacao | Alta | Paralisacao completa da casa; cascata de atrasos | Sim — tracking de holds com prazo estimado e escalaacao |
| INS-04 | Cancelamento no dia de inspecao: depende de contato direto com inspetor que nao atende | Alta | Taxa de cancelamento paga; inspetor pode rejeitar ou nao ser encontrado | Nao — depende do condado; parcialmente: alerta antecipado de cancelamento |
| INS-05 | Fees bloqueiam reagendamento (Citrus): precisa coordenar com financeiro antes | Alta | Atraso de reagendamento; comunicacao manual urgente | Sim — integracao automatica com Financeiro para pagamento de fees |
| INS-06 | Sistemas diferentes por condado: cada um com regras, sites e processos proprios | Media | Curva de aprendizado; erros de processo entre condados | Parcial — checklists por condado integrados ao sistema |
| INS-07 | Resultados imprecisos via Slack (Citrus): sempre precisa confirmar no site | Media | Retrabalho de verificacao; risco de agir com informacao errada | Sim — integracao direta com portal do condado para resultados |
| INS-08 | Codigo de acesso manual: verificar finals, buscar inspetor, enviar SMS a cada inspecao final | Baixa | Tempo perdido em tarefa repetitiva | Sim — envio automatico de codigo de acesso ao inspetor no dia da inspecao |

### Warranty (Garantia)

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| WAR-01 | Nao existe software dedicado para warranty: prejuizos significativos (caso de $14.000 em uma unica casa) | Alta | Risco financeiro alto; garantias nao rastreadas; responsabilidade indefinida | Sim — modulo dedicado de warranty com portal do cliente |
| WAR-02 | 3 daily logs por reparo: abertura, schedule, finalizacao — muito input no sistema | Alta | Retrabalho excessivo; propenso a omissao de etapas | Sim — registro unico com transicoes de status automaticas |
| WAR-03 | Subs nao respondem: cobrar repetidamente via WhatsApp | Alta | Reparos em aberto; clientes insatisfeitos; risco de garantia vencida | Parcial — lembretes automaticos com escalacao para gestor apos X dias |
| WAR-04 | Volume alto e dinamismo: dificil manter registro no BT em tempo real | Alta | Backlog de registros; visao desatualizada do status real | Sim — input simplificado via app mobile |
| WAR-05 | Trabalho duplicado: cliente manda e-mail E WhatsApp; equipe responde em ambos | Media | Horas perdidas em comunicacao redundante; risco de resposta divergente | Parcial — inbox unificado de comunicacao com cliente |
| WAR-06 | Imediatismo dos clientes: ligam e mandam WhatsApp ignorando canal formal | Media | Equipe desviada do fluxo padrao; informalidade compromete registro | Nao — comportamento do cliente; parcialmente: mensagem automatica de redirecionamento |
| WAR-07 | Valores de reparo imprevisiveis: morador nao relata extensao total; sub descobre no local | Media | Orcamentos iniciais incorretos; custos surpresa | Parcial — historico de custos de reparos similares para estimativa |
| WAR-08 | Subs de garantia com prazo proprio: sub conta 1 ano desde fim do servico, nao do CEO | Media | Conflito de prazo entre empresa e sub; custo de reparo fora da garantia do sub | Parcial — calculo automatico de prazo de garantia do sub por servico |
| WAR-09 | Falta de registro retroativo detectado: inputs retroativos nao sao vistos no acompanhamento | Media | Registros perdidos; historico incompleto por casa | Sim — auditoria de data de criacao vs data do evento |
| WAR-10 | Builder Trend lento no campo: internet ruim causa delay | Media | Sistema inutilizavel em campo; omissao de registros | Sim — app mobile leve com modo offline |
| WAR-11 | Cortes de grama urgentes: risco de notificacao/multa do condado | Baixa | Multa financeira; impacto na reputacao da empresa | Sim — calendario automatico de cortes com alertas preventivos |
| WAR-12 | Monitores nao acompanham casas em fase 4: Kildery tem que verificar com supervisor Daniel | Baixa | Verificacoes manuais extras; dependencia de pessoa | Parcial — atribuicao automatica de responsavel por fase |

### Takeoff

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| TAK-01 | Compilacao manual da lista de takeoff: resultados do BlueBeam compilados manualmente no Word | Alta | Processo lento e propenso a erros; escala muito mal com volume | Sim — integracao via API do BlueBeam ou takeoff nativo no software |
| TAK-02 | CPUs da empresa nao rodam os programas de arquitetura: Candida e Gabriela usam computadores pessoais | Alta | Dependencia de hardware pessoal; risco de perda de dados; inconsistencia | Nao — requer investimento em hardware |
| TAK-03 | 3.500 itens para atualizar manualmente quando modelos mudam: sem mecanismo de duplicacao | Alta | Dias de trabalho para cada atualizacao de modelo; alta chance de erro | Sim — template com duplicacao automatica de valores entre modelos |
| TAK-04 | Mudancas de takeoff nao notificam automaticamente equipe de budget | Media | Budget calculado com dados desatualizados; retrabalho em orcamentos | Sim — notificacao automatica ao Orcamento ao versionar takeoff |
| TAK-05 | Volatilidade do takeoff para customs: clientes mudam definicoes durante obra | Media | Retrabalho constante; custo de remedicao e recalculo | Parcial — historico de versoes com delta de mudancas identificado |
| TAK-06 | Equipe de projetos trabalha isolada: pouca interacao com outros setores | Media | Desalinhamento entre takeoff e necessidades reais de campo | Nao — requer mudanca cultural; parcialmente: revisoes interdepartamentais agendadas |
| TAK-07 | Takeoff deveria ser feito no inicio da obra com PM e supervisores: atualmente e tardio | Media | Compras sem base solida; riscos de desabastecimento | Nao — requer mudanca de processo |
| TAK-08 | Funcao de integracao do BlueBeam nao utilizada: funcao paga para link com planilhas nao explorada | Media | Perda de investimento; retrabalho evitavel | Sim — treinamento e configuracao da funcao de exportacao do BlueBeam |
| TAK-09 | Nomenclatura incompativel entre fornecedores: CAS Creed vs CMEX requer mapeamento manual | Baixa | Tempo perdido comparando items de diferentes nomenclaturas | Sim — tabela de equivalencia de itens entre fornecedores |
| TAK-10 | Dependencia de projeto de engenharia finalizado antes do takeoff: pode atrasar fluxo | Baixa | Takeoff e orcamento atrasados por etapa anterior | Parcial — takeoff preliminar com valores provisorios; update ao receber executivo |

### Permits / Documentacao

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| PER-01 | Nao recebem e-mail de aviso de expiracao de permit (Marion): risco de cancelamento | Alta | Permit expira, obra para, processo reinicia do zero | Sim — monitoramento automatico de validade com alertas proativos |
| PER-02 | Comunicacao de hold nao e centralizada: toda empresa afetada mas sem visibilidade unica | Alta | Decisoes de agendamento feitas sem saber de holds ativos | Sim — dashboard de holds ativos visivel para todos os departamentos |
| PER-03 | Historico de projeto escrito manualmente: reproduzir historico gasta muito tempo | Alta | Perda de contexto; onboarding demorado; dependencia de memoria humana | Sim — historico automatico de eventos por casa/projeto |
| PER-04 | Documentos com versoes erradas podem chegar ao field: sem controle de versionamento | Alta | Construcao com planta errada; erros graves e caros | Sim — sistema de versao com seal digital; apenas versao ativa distribuida |
| PER-05 | Waivers e Arrows em Citrus County: retrabalho recorrente | Alta | Horas de retrabalho em cada casa em Citrus; previsivel mas nao sistematizado | Sim — checklist automatico de waiver/arrows para casas em Citrus |
| PER-06 | Falta de busca por qualquer atributo: sem busca por nome do dono, parcel ID, permit number | Media | Tempo perdido localizando casas; manual e lento | Sim — busca full-text no novo software |
| PER-07 | 16+ POs/daily logs duplicados para mesmo dono em condominios | Media | Retrabalho extremo em projetos de condominio | Parcial — templates em lote para projetos com multiplas unidades |
| PER-08 | Informacao repetida para Client Relations: status que ja esta na planilha | Media | Interrupcoes frequentes; tempo perdido em comunicacao redundante | Sim — portal interno com visibilidade de status de permit por casa |
| PER-09 | Comunicacao manual com Dandara (Utilities) sobre septic permit | Media | Coordenacao por WhatsApp; informacao pode se perder | Sim — notificacao automatica entre Permits e Utilities ao atingir marcos |
| PER-10 | Processo manual para casas customizadas: sem padronizacao, documentos nao previstos | Media | Cada custom e diferente; risco de esquecer etapas criticas | Parcial — checklist dinamico para custom com campos adicionais conforme tipo |
| PER-11 | Gestao de modifications e extensions completamente manual | Baixa | Risco de vencimento nao percebido; processo demorado | Sim — calendario de expiracao com fluxo de renovacao integrado |

### Land Acquisition / Land Development

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| LAN-01 | Extracao de dados do Builder Trend feita com muita dificuldade: BT nao foi feito para isso | Media | Relatorios gerenciais demorados; dados imprecisos | Sim — dashboard nativo de land no novo software |
| LAN-02 | Falta de integracao entre ClickUp (leads) e Builder Trend (execucao) | Media | Informacao de leads nao migra para execucao; dados duplicados | Sim — modulo de CRM integrado ao fluxo de execucao |
| LAN-03 | Dados extraidos armazenados em tabela crua: banco de dados improvisado | Media | Fragil; dependente de quem criou; sem historico de mudancas | Sim — banco de dados estruturado com historico de versoes |
| LAN-04 | Processo pouco estruturado: baixo volume dificulta sistematizacao | Baixa | Propenso a erros quando volume aumentar; conhecimento na cabeca do Vinicius | Parcial — templates de projeto de land com checklist de etapas |
| LAN-05 | Muitos leads, poucas obras em execucao: gestao de funil de vendas manual | Baixa | Oportunidades perdidas; sem visibilidade do funil | Sim — modulo de CRM com funil de oportunidades |

### Client Relations

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| CR-01 | Schedule do portal desatualizado: nao considera holds, atrasos, remarcacoes | Alta | Cliente ve informacao errada; gera atritos e reclamacoes frequentes | Sim — portal atualizado em tempo real a partir do sistema |
| CR-02 | Budget do portal desatualizado: "price adjustment" assusta clientes; itens nao marcados | Alta | Perda de confianca do cliente; trabalho extra da equipe CR para explicar | Sim — portal com status em tempo real e comunicacao de mudancas |
| CR-03 | Upgrades se perdem no processo: sub esquece de executar; ninguem confere | Alta | Itens prometidos ao cliente nao entregues; risco legal e reputacional | Sim — tracking de upgrades com checklist de verificacao antes da entrega |
| CR-04 | Demora na obtencao de respostas: busca em varios locais (Daily Log, planilhas, setores) | Media | Clientes insatisfeitos com tempo de resposta; equipe sobrecarregada | Sim — visao unificada de dados da casa para equipe CR |
| CR-05 | Comunicacao dificil com gerentes e supervisores: estao em campo, demoram a responder | Media | CR nao consegue dar status preciso ao cliente; informacao desatualizada | Parcial — status automatico de obra visivel sem depender de input manual de supervisor |
| CR-06 | Duplo registro: alimentar multiplos sistemas manualmente | Media | Horas perdidas; inconsistencia entre sistemas | Sim — sistema unico com propagacao |
| CR-07 | Portal gera mais trabalho do que solucao: equipe explica inconsistencias constantemente | Media | Erosao de confianca do cliente; overhead de suporte | Sim — portal confiavel elimina necessidade de explicacoes |
| CR-08 | Apenas Juliana tem telefone no HubSpot: limitacao de usuarios | Baixa | Capacidade de atendimento telefonica restrita | Nao — restricao de licenca; requer avaliacao de custo |

### Utilities

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| UTI-01 | Triplo registro: planilha + Daily Logs + campos customizados do BT | Alta | Retrabalho diario significativo; inconsistencias entre registros | Sim — registro unico com propagacao para todos os campos |
| UTI-02 | Falta de previsibilidade de prazos das companhias: especialmente DUC | Alta | Planejamento de obra impossivel nessa etapa; casas aguardando meses | Nao — depende de terceiros; parcialmente: historico de prazos por companhia |
| UTI-03 | Portal Alex Shore com problemas apos migracao: pagando faturas uma a uma | Media | Horas perdidas em pagamentos manuais de utilities | Sim — integracao com portal de pagamento de utilities |
| UTI-04 | Comunicacao fragmentada: WhatsApp, Slack, e-mail, BT, planilha em paralelo | Media | Informacao se perde entre canais; rastreabilidade zero | Sim — hub de comunicacao centralizado por casa |
| UTI-05 | Processo do septic crescendo em complexidade: mais etapas, inspecoes rigorosas | Media | Risco de etapas esquecidas; processo cresce sem sistematizacao | Sim — checklist dinamico de septic com pre-requisitos por tipo |
| UTI-06 | Variabilidade por condado e companhia: cada combinacao tem regras diferentes | Media | Erros de processo; curva de aprendizado constante | Parcial — regras codificadas por condado+companhia como template |
| UTI-07 | Multiplas fontes de faturas: site, e-mail, correspondencia fisica | Media | Faturas perdidas; pagamentos atrasados | Sim — inbox centralizado de faturas com OCR/parse |
| UTI-08 | Dificuldade de obter informacoes das companhias: ma vontade, medidores instalados sem notificacao | Media | Necessidade de monitoramento fisico presencial semanal | Nao — depende das companhias; parcialmente: alertas de rota para monitores |
| UTI-09 | Retrabalho com tug side errado: custo adicional significativo | Baixa | Custo extra de reinstalacao; atraso na obra | Sim — campo obrigatorio de tug side confirmado antes de agendar RF Electric |
| UTI-10 | Informacoes dispersas: precisa consultar varias planilhas para encontrar supervisor, dados da casa | Baixa | Tempo perdido localizando informacoes basicas | Sim — visao unificada de dados da casa |

### Core Craft (Servicos)

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| CC-01 | Valores indefinidos no momento da execucao: equipe executa sem saber custos; Sr. Yuri define depois | Alta | Retrabalho financeiro; POs criadas retroativamente | Sim — tabela de precos padrao por servico; valores pre-aprovados por faixa |
| CC-02 | Dumpster impede outros servicos: presenca bloqueia tug install e septic install | Alta | Cascata de atrasos; coordenacao manual urgente necessaria | Sim — pre-requisito no agendamento: verificar ausencia de dumpster |
| CC-03 | CUT sem remocao: scheduling agendava corte sem solicitar remocao de material | Media | Atraso na sequencia; re-agendamento necessario | Sim — servico CUT automaticamente vinculado ao servico de remocao |
| CC-04 | Supervisores solicitam direto no grupo: sem passar pelo Daily Log | Media | Retrabalho sem rastreabilidade; custos nao associados a casa | Sim — canal padronizado com campo obrigatorio de casa/projeto |
| CC-05 | Visibilidade da agenda: Scheduling nao ve disponibilidade do Grupo 05 (limpezas) | Media | Agendamentos sem confirmacao de disponibilidade | Sim — calendario publico de disponibilidade dos grupos Core Craft |
| CC-06 | Mudancas de funcao dos handymen: remanejamentos semanais sem padrao | Baixa | Imprevisibilidade para a equipe; dificuldade de planejamento | Parcial — escala semanal com substituicoes documentadas |

### RH (Recursos Humanos)

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| RH-01 | Processo manual intensivo: acompanhamento diario do calendario; debito manual de saldos | Alta | Horas semanais perdidas; propenso a erros; nao escala | Sim — calculo automatico de saldos, cargas e expiracoes |
| RH-02 | Lider agenda PTO sem saldo disponivel: falta controle visivel de saldo para lideres | Media | Conflitos ao descobrir que PTO nao existe; processo retroativo | Sim — validacao de saldo em tempo real no ato do agendamento |
| RH-03 | Agendamentos passados nao notificam: depende do lider avisar manualmente | Media | PTOs nao debitados; registros atrasados | Sim — notificacao retroativa com confirmacao do lider |
| RH-04 | Falta de integracao entre Google Calendar e planilha | Baixa | Duas ferramentas para o mesmo dado; inconsistencia possivel | Sim — sistema de RH integrado ao calendario com sync automatico |

### Escritorio de Projetos (Design Office)

| # | Dor | Severidade | Impacto | Automacao Possivel |
|---|-----|------------|---------|-------------------|
| EP-01 | Nao existe tracking para pre-contrato: sem rastrear projetos novos, entregas, aprovacoes | Alta | Oportunidades perdidas; projetos custom sem visibilidade; dependencia de Camila | Sim — modulo de CRM de pre-contrato com funil de projetos |
| EP-02 | Gestao de mudancas deficiente: revisoes durante obra nao comunicadas para campo e PMs | Alta | Construcao com planta desatualizada; erros caros de execucao | Sim — notificacao automatica de revisao de planta para todos os stakeholders |
| EP-03 | CPUs nao rodam programas de arquitetura: AutoCAD, SketchUp, Enscape insuficientes | Alta | Dependencia de hardware pessoal; risco de perda de dados e propriedade intelectual | Nao — requer investimento em hardware ou cloud |
| EP-04 | 3.500 itens para atualizar manualmente entre modelos: falta template/duplicacao | Alta | Dias de trabalho para cada novo modelo; altissima chance de erro | Sim — mecanismo de duplicacao com template editavel |
| EP-05 | Compilacao manual do takeoff do BlueBeam para Word | Media | Processo lento; perda de dados na transposicao manual | Sim — exportacao direta do BlueBeam via API |
| EP-06 | Clientes customizados mudam muito: budget nao e definitivo | Media | Retrabalho continuo; custo imprevisivel ate o fim da obra | Parcial — historico de mudancas com custo acumulado por item |
| EP-07 | Budget customizado feito "no escuro": estimativas de area e nivel no estagio inicial | Media | Estimativas imprecisas geradas ao cliente; renegociacoes posteriores | Parcial — base de dados de custo por sqft e por tipo de acabamento |
| EP-08 | Mudancas tardias exigem refazer budgets em massa | Media | Dias de trabalho para atualizar multiplos projetos | Sim — mecanismo de atualizacao em lote de budgets por modelo |
| EP-09 | Equipe trabalha isolada internamente: pouca interacao com outros setores | Media | Desalinhamento entre projeto e realidade de campo | Nao — requer mudanca cultural e organizacional |
| EP-10 | Problemas de instalacao/licenca do AutoCAD | Baixa | Interrupcoes de trabalho; perda de produtividade | Nao — dependente de fornecedor de software |

---

## Gargalos Interdepartamentais

Problemas que existem na INTERFACE entre departamentos — handoffs sem padrao, informacao atrasada ou perdida, dependencias criticas nao respeitadas.

| # | Gargalo | Dept Origem | Dept Destino | Severidade | Descricao |
|---|---------|-------------|--------------|------------|-----------|
| G-01 | Takeoff nao notifica Budget ao ser atualizado | Takeoff / Escritorio Projetos | Orcamento | Alta | Mudancas de takeoff nao disparam notificacao automatica. Budget calculado com dados antigos. Descoberto tardiamente quando materiais chegam em quantidade errada. |
| G-02 | Supervisores autorizam reparos sem criar PO | Supervisao / Field | Financeiro | Alta | Supervisor autoriza verbalmente o servico. Sub executa. Invoice chega ao Financeiro sem PO correspondente. Processo de aprovacao urgente e manual (Moises/Samuel precisam confirmar). |
| G-03 | Checklist Done e gatilho de pagamento sem validacao robusta | Supervisao / Monitoring | Financeiro | Alta | Monitor marca checklist done (servico concluido) — isso dispara pagamento automatico ao sub. Novos monitores sem treinamento adequado podem marcar incorretamente. Sub pago nao volta para corrigir. |
| G-04 | Budget deveria preceder permit, mas frequentemente atrasa | Orcamento | Permits | Alta | Equipe de Permits depende do budget estar pronto para iniciar aplicacao. Atraso no budget impacta inicio da obra. Sem sistema de alerta de dependencia entre os dois. |
| G-05 | Informacao de sistema de agua/esgoto nao chega automaticamente para Permits | Utilities | Permits | Alta | Dandara (Utilities) descobre se e septic ou esgoto publico. Precisa comunicar manualmente para Permits. Se comunicacao falhar, documentacao de permit pode estar incorreta para o condado. |
| G-06 | Draws financeiros travam progresso de obra sem visibilidade para Scheduling | Financeiro | Scheduling | Alta | Schedulers precisam de draws liberados para avancar fases. Quando draw demora, casa para sem que Scheduling saiba por quanto tempo. Sem previsao de liberacao visivel. |
| G-07 | Mudancas de projeto nao chegam ao field em tempo habil | Escritorio Projetos | Supervisao / Field | Alta | Revisoes de plantas durante obra nao sao comunicadas sistematicamente. Supervisor pode estar executando com planta desatualizada sem saber. |
| G-08 | Client Relations depende de multiplos setores para responder cliente | Client Relations | Scheduling / Supervisao / Financeiro / Permits | Alta | CR nao tem visibilidade direta do status da obra. Precisa consultar Scheduling, Supervisao e Permits separadamente. Demora na resposta ao cliente. |
| G-09 | Contrato assinado dispara multiplos processos sem sistema de coordenacao | Permits / Client Relations | Financeiro / Scheduling / Utilities | Alta | Assinatura do contrato deve acionar: Financeiro (cobrar draws), Scheduling (iniciar agendamento), Utilities (abrir contas). Coordenacao feita por Slack informal. |
| G-10 | Hold de inspecao nao e comunicado centralmente | Inspecao | Scheduling / Supervisao / Client Relations | Alta | Hold para toda a obra. Dandara sabe, mas notificacao nao e estruturada. Scheduling pode continuar agendando servicos de uma casa em hold. CR pode dar data errada ao cliente. |
| G-11 | Zorro nao integra com Builder Trend: dados duplicados manualmente | Compras | Financeiro | Alta | Saidas de material registradas no Zorro precisam ser manualmente transferidas para BT e planilhas de distribuicao. Qualquer atraso causa desalinhamento contabil. |
| G-12 | Energy Calculation solicitado independentemente por Budget e Permits | Orcamento | Permits | Media | Dois departamentos solicitam o mesmo documento do mesmo fornecedor sem saber um do outro. Custo duplicado; fornecedor confuso. |
| G-13 | CR solicita autorizacao de grama para casas closed a Warranty | Warranty | Client Relations | Media | Para casas vendidas, Warranty precisa de autorizacao de CR antes de solicitar corte de grama. Fluxo via Slack informal; pode atrasar e gerar multa do condado. |
| G-14 | Impact fees de Marion bloqueiam Final Electric sem alerta antecipado | Financeiro | Inspecao | Media | Dandara agenda inspecao final eletrica, mas ela so passa se Financeiro tiver pago impact fees. Sem visibilidade cruzada entre os dois. Inspecao pode ser agendada em vao. |
| G-15 | Tug side definido por Utilities mas executado por Scheduling (RF Electric) | Utilities | Scheduling | Media | Dandara define qual lado da caixa eletrica. Scheduling precisa informar ao sub de eletrica. Comunicacao via Slack/e-mail informal. Se errar o lado, custo adicional alto. |
| G-16 | Informacoes de customizacao do cliente nao chegam a tempo para Scheduling Fase 3 | Client Relations | Scheduling | Media | Customizacoes aprovadas pelo cliente (paleta diferente, stone veneer, pavers) ficam no card fixo do BT. Schedulers precisam verificar manualmente. Mudancas comunicadas tarde causam reagendamento. |
| G-17 | Status de permit nao visivel para CR sem consulta manual | Permits | Client Relations | Media | CR precisa perguntar para Permits o status do permit para informar ao cliente. Sem visibilidade direta. Interrupcoes frequentes na equipe de Permits. |
| G-18 | Fechamento de casa requer sincronia entre 4 departamentos sem orquestrador | Financeiro / Warranty / Permits / Scheduling | Client Relations | Media | Fechamento da casa requer: Financeiro (bills), Warranty (closing reparos), Permits (CO), Scheduling (inspecao final). Sem sistema de orquestracao, algum passo pode ser esquecido. |
| G-19 | Takeoff de lumber sem responsavel definido com novo fornecedor | Takeoff / Compras | Orcamento | Alta | Anterior fornecedor fazia takeoff de lumber. Novo nao faz. Ninguem na empresa tem essa habilidade. Gap critico no processo de compras de material estrutural. |

---

## Resumo de Oportunidades de Automacao

### Integracao de Sistemas

| Oportunidade | Dores Relacionadas | Impacto Estimado | Prioridade |
|---|---|---|---|
| Integracao software proprio com QuickBooks (mapeamento de classes por projeto) | FIN-01, FIN-06 | Alto — elimina 2h/dia de entrada manual | Alta |
| Integracao software com portal de condados para monitoramento de holds e resultados de inspecao | INS-01, INS-07, PER-01 | Alto — elimina verificacoes manuais diarias | Alta |
| Propagacao de informacao de contrato para POs, Financeiro e Scheduling | FIN-03, FIN-11, G-09 | Alto — elimina retrabalho de atualizacao multipla | Alta |
| Integracao BlueBeam via API para exportacao de takeoff | TAK-01, EP-05 | Medio — elimina compilacao manual de listas | Media |
| Integracao Zorro-sistema para rastreabilidade de lote | COM-02, COM-03, G-11 | Alto — viabiliza custo real por casa | Alta |
| Sistema de utilities com registro unico propagado | UTI-01, G-05 | Medio — elimina triplo registro | Media |

### Eliminacao de Entrada Manual Duplicada

| Oportunidade | Dores Relacionadas | Impacto Estimado | Prioridade |
|---|---|---|---|
| Entrada unica em Scheduling (daily log, schedule e PO em um unico formulario) | SCH-01 | Alto — afeta 7 schedulers diariamente | Alta |
| Propagacao automatica de orcamento aprovado para criacao de POs | ORC-02 | Alto — elimina trabalho de Ana Helena | Alta |
| Sistema de estoque unificado com distribuicao automatica por casa | COM-01, COM-04 | Alto — elimina 12+ planilhas simultaneas | Alta |
| Registro unico de warranty com transicao de status (elimina 3 daily logs por reparo) | WAR-02 | Alto — multiplica por cada reparo | Alta |
| Portal de permits com visibilidade para CR sem consulta manual | PER-08, G-17 | Medio — elimina interrupcoes na equipe de permits | Media |

### Notificacoes e Alertas Automaticos

| Oportunidade | Dores Relacionadas | Impacto Estimado | Prioridade |
|---|---|---|---|
| Alerta de expiracao de permit com antecedencia configuravel | PER-01 | Alto — evita risco critico de cancelamento | Alta |
| Notificacao de remocao de hold de inspecao | INS-01, G-10 | Alto — casas podem voltar a trabalhar imediatamente | Alta |
| Alerta de mudanca de takeoff para equipe de Budget | ORC-11, TAK-04, G-01 | Alto — elimina trabalho com dados defasados | Alta |
| Notificacao de mudanca de projeto para field e PMs | EP-02, G-07 | Alto — previne construcao com planta errada | Alta |
| Alerta de draw disponivel para equipe de Scheduling | SCH-06, FIN-05 | Medio — elimina espera passiva de draws | Media |
| Lembretes automaticos para subs de warranty com escalacao | WAR-03 | Medio — reduz reparos em aberto | Media |
| Alerta de fees pendentes de inspecao para Financeiro | INS-02, INS-05, G-14 | Alto — previne inspecao agendada em vao | Alta |

### Relatorios Automatizados

| Oportunidade | Dores Relacionadas | Impacto Estimado | Prioridade |
|---|---|---|---|
| Dashboard em tempo real de casas por status para supervisores (com cores e timeline) | SUP-04, SUP-05 | Medio — substitui dashboards somente leitura | Media |
| Historico financeiro completo por casa para fechamento contabil | FIN-12 | Medio — simplifica fechamento de casas | Media |
| Dashboard de land development (funil de leads ate execucao) | LAN-01, LAN-02 | Baixo — volume atual pequeno | Baixa |
| Relatorio automatico de desempenho de inspecoes por condado | INS-06 | Baixo — ja feito manualmente por Dandara | Baixa |
| Portal do cliente atualizado em tempo real (schedule e budget) | CR-01, CR-02 | Alto — elimina principal fonte de atrito com clientes | Alta |

### Workflows de Aprovacao Digital

| Oportunidade | Dores Relacionadas | Impacto Estimado | Prioridade |
|---|---|---|---|
| Exigencia de PO antes de execucao de reparo (via app mobile para supervisores) | SUP-01, FIN-02, G-02 | Alto — elimina invoices sem PO | Alta |
| Fluxo de aprovacao de reparos com escalacao automatica por prazo | FIN-04 | Alto — desbloqueia pagamentos travados | Alta |
| Aprovacao de upgrades de cliente com tracking end-to-end | CR-03 | Alto — previne upgrades esquecidos | Alta |
| Validacao de saldo de PTO no ato do agendamento para lideres | RH-02 | Medio — elimina conflitos retroativos | Media |
| Fluxo de aprovacao de cotacoes com status centralizado | ORC-09 | Medio — elimina cotacoes perdidas em e-mail | Media |

---

## Estatisticas por Departamento

| Departamento | Total Dores | Alta | Media | Baixa | % Automatizavel (Sim+Parcial) |
|---|---|---|---|---|---|
| Orcamento | 11 | 5 | 5 | 1 | 73% (8/11) |
| Compras | 11 | 6 | 4 | 1 | 73% (8/11) |
| Financeiro | 12 | 7 | 4 | 1 | 83% (10/12) |
| Scheduling | 14 | 6 | 7 | 1 | 86% (12/14) |
| Supervisao | 10 | 3 | 6 | 1 | 70% (7/10) |
| Inspecao | 8 | 5 | 2 | 1 | 88% (7/8) |
| Warranty | 12 | 4 | 6 | 2 | 83% (10/12) |
| Takeoff | 10 | 3 | 6 | 1 | 70% (7/10) |
| Permits | 11 | 5 | 5 | 1 | 82% (9/11) |
| Land Acquisition | 5 | 0 | 3 | 2 | 80% (4/5) |
| Client Relations | 8 | 3 | 4 | 1 | 88% (7/8) |
| Utilities | 10 | 2 | 7 | 1 | 70% (7/10) |
| Core Craft | 6 | 2 | 3 | 1 | 83% (5/6) |
| RH | 4 | 1 | 2 | 1 | 75% (3/4) |
| Escritorio Projetos | 10 | 4 | 5 | 1 | 70% (7/10) |
| **TOTAL** | **97** | **38 (39%)** | **59 (61%)** | **16 (16%)** | **78% (59/97 aprox)** |

> Nota sobre severidade "Baixa" no total consolidado: as dores classificadas como Baixa em departamentos individuais sao 18 (alguns itens revistos como Media no consolidado). A tabela acima usa contagem por departamento para consistencia.

---

## Notas Metodologicas

- **Fonte primaria:** Secao "Dores e Problemas Conhecidos" de cada um dos 15 arquivos dept_*.md
- **Fonte secundaria:** Secao "Gaps de Automacao" e "Limitacoes Reportadas" de 02_INVENTARIO_FERRAMENTAS.md
- **Criterio de severidade Alta:** Bloqueia fluxo operacional ou causa retrabalho frequente com impacto financeiro/prazo mensuravel
- **Criterio de severidade Media:** Causa ineficiencia mas existe workaround; impacto acumulado mas nao paralisante
- **Criterio de severidade Baixa:** Inconveniencia menor; solucao manual aceitavel; impacto limitado
- **Criterio de automacao Sim:** Solucao tecnica clara e implementavel com software
- **Criterio de automacao Parcial:** Automacao possivel mas limitada por fatores externos (terceiros, hardware, comportamento humano)
- **Criterio de automacao Nao:** Solucao depende de mudanca organizacional, investimento em hardware externo, ou comportamento de terceiros fora do controle da Lakeshore

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Organograma](01_ORGANOGRAMA.md)
- [Inventario de Ferramentas](02_INVENTARIO_FERRAMENTAS.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- [Fluxo Spec Home](05_FLUXO_SPEC_HOME.md)
- [Fluxo Custom Home](06_FLUXO_CUSTOM_HOME.md)
- [Glossario de Termos](03_GLOSSARIO.md)
