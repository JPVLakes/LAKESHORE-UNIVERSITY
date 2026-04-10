# Inventario de Ferramentas e Sistemas - Lakeshore Development

## Resumo
- Total de ferramentas identificadas: 24
- Categorias: Software de Gestao de Construcao, ERP/Financeiro, Gestao de Estoque, Planilhas/Produtividade, Comunicacao, Gestao de Projetos/Tarefas, Arquitetura/Engenharia, Inteligencia Artificial, Plataforma de Assinatura Digital, CRM, Navegadores/Portais Governamentais

## Ferramentas

### BuilderTrend (BT)
- **Categoria:** Software de Gestao de Construcao
- **Usuarios:** Praticamente todos os departamentos -- Scheduling (daily logs, POs, schedule), Financeiro (POs, bills, fechamento de casas), Supervisao (consultas pontuais), Client Relations (portal do cliente), Warranty (daily logs, tags), Compras (POs, BIs), Permits (armazenamento de documentos), Utilities (daily logs, campos customizados), Orcamento (templates, cronogramas), Core Craft (requests de servicos)
- **Finalidade:** Cronograma, POs (Purchase Orders), bills, templates de casas, comunicacao campo-escritorio, daily logs, schedule, portal do cliente (budget, fotos, invoices), documentos
- **Limitacoes Reportadas:**
  - Lento e pesado (carregamento demorado, recarrega pagina apos cada input)
  - Informacao repetida 3x (daily logs + schedule + PO com mesmos dados)
  - Navegacao confusa para informacoes basicas (modelo da casa requer navegar por pastas)
  - Falta de campos padronizados na PO (titulo digitado livremente)
  - Portal do cliente desatualizado (schedule e budget nao refletem realidade)
  - Tags excessivas e confusas, algumas duplicadas entre fases
  - Notificacoes nao funcionam adequadamente
  - Extracao de dados extremamente dificil (nao foi feito para BI)
  - Internet ruim no campo causa duplicacao/perda de dados
  - Nao suporta pagamentos parciais de draws
  - Duas instancias separadas (BT1 e BT2)
- **Status:** Em substituicao pelo software proprio da Lakeshore

### QuickBooks
- **Categoria:** ERP / Sistema Financeiro
- **Usuarios:** Financeiro (Iara, Rayff, Cinthia, Thabata), Ana Helena Torres
- **Finalidade:** Sistema gerencial financeiro, relatorios (DRE, balanco, T99), conciliacao bancaria, classificacao por projeto (classe CMER + numero da casa)
- **Limitacoes Reportadas:**
  - Inclusao de classe manual consome ~2 horas/dia para 86 bills
  - Sistema lento
  - Integracao incompleta com BuilderTrend (data de vencimento nao serve como criterio)
  - Processo manual de conciliacao
- **Status:** Em uso -- sera mantido com integracao futura ao software proprio

### Zorro
- **Categoria:** Software de Gestao de Estoque
- **Usuarios:** Klauser Silva (warehouse), Compras (Brenda, Marilia), Core Craft (Sales Lopes)
- **Finalidade:** Registro de entradas e saidas de material (Sales Orders), purchase orders, geracao de invoices (Core Craft)
- **Limitacoes Reportadas:**
  - Nao atualiza precos automaticamente
  - Nao referencia lote de compra (nao informa de qual compra veio o material que esta saindo)
  - Dificil rastrear purchase orders
  - Nao integra com outras ferramentas
  - Drafts nao confirmados geram incertezas
- **Status:** Em substituicao pelo software proprio

### Excel / Google Sheets (Planilhas)
- **Categoria:** Planilhas de Produtividade
- **Usuarios:** TODOS os departamentos -- cada pessoa cria suas proprias planilhas. Orcamento (budgets, cotacoes), Compras (12+ planilhas abertas diariamente: Purchase, IT dos Materiais, Distribuicao, Ordens Disponiveis), Financeiro (checklist de fechamento, pagamento diario), Scheduling (planilha pessoal de acompanhamento), Inspecao (controle por condado com formatacao condicional), Warranty (Kildery: multiplas abas de tracking), Utilities (controle de agua, esgoto, energia), Permits (tabela de controle), Deposito (controle pessoal de parafusos, cintas, plumbing), RH (PTOs e sick days), Core Craft (planilha de tags)
- **Finalidade:** Budgets, cotacoes, acompanhamento de processos, controle financeiro, tracking de casas, controle de inspecoes, monitoramento de utilities
- **Limitacoes Reportadas:**
  - Volume excessivo de planilhas (12+ simultaneas para Compras)
  - Informacoes semelhantes em formatos diferentes
  - Nao integrado entre departamentos
  - Duplicacao de esforco
  - Cada pessoa cria sua propria versao
  - Dados desestruturados, sem automacao
- **Status:** Em substituicao pelo software proprio

### ClickUp
- **Categoria:** Gestao de Projetos / Tarefas
- **Usuarios:** Orcamento (acompanhamento de atividades do setor), Camila Martins (tracking interno com equipe de projetos), Utilities (Dandara -- lembretes e anotacoes), Land Development (Vinicius -- gestao de leads), Mauricio (tarefas pendentes)
- **Finalidade:** Acompanhamento de atividades, progresso de codes/orcamentos/contratos, lembretes
- **Limitacoes Reportadas:**
  - Uso pessoal e nao padronizado entre departamentos
  - Giovana nao usa, prefere quadro/papel
  - Nao integrado com outros sistemas
- **Status:** Em substituicao pelo software proprio

### Slack
- **Categoria:** Comunicacao Interna
- **Usuarios:** Scheduling (comunicacao com monitores), Inspecao (canal de requests), Financeiro (recibos do Field), Utilities (notificacoes de Slack Bots), Core Craft (22 tipos de servicos com tags), Client Relations (canal RCRC)
- **Finalidade:** Comunicacao oficial interna, canais de notificacao (client hold, permit, etc.), Slack Bots para notificacoes automaticas
- **Limitacoes Reportadas:**
  - Instavel e lento
  - Internet limitada no campo impede uso adequado
  - Equipe recorre ao WhatsApp por ser mais leve e confiavel
  - Nao substituiu WhatsApp como pretendido
- **Status:** Em uso -- parcialmente substituido por hub de notificacoes no software proprio

### WhatsApp
- **Categoria:** Comunicacao
- **Usuarios:** TODOS os departamentos -- Scheduling (comunicacao com 90%+ dos subs), Core Craft (7 grupos de servicos), Warranty (cobrancas a subs, comunicacao com realtors), Client Relations (via HubSpot), Supervisao, Compras, Land Development (comunicacao com clientes)
- **Finalidade:** Comunicacao principal com subcontratados, pedidos urgentes, envio de documentos, solicitacao de servicos, grupos por tipo de servico
- **Limitacoes Reportadas:**
  - Nao formal, dificil de rastrear
  - Duplicidade de comunicacao (WhatsApp + e-mail + Slack)
  - Informacoes perdidas entre canais
  - Supervisores solicitam direto no grupo sem Daily Log
- **Status:** Em uso -- sera parcialmente integrado ao software proprio

### E-mail (Gmail)
- **Categoria:** Comunicacao Formal
- **Usuarios:** Todos os departamentos -- Financeiro (recebimento de invoices), Warranty (canal 100% formal), Permits (e-mail compartilhado da equipe), Orcamento (comunicacao com fornecedores), Compras (salvar informacoes de compras), Utilities (comunicacao com companhias)
- **Finalidade:** Recebimento de invoices, cotacoes, comunicacao formal com fornecedores e clientes, envio de contratos, envio de documentos de permit
- **Limitacoes Reportadas:**
  - Volume muito alto de e-mails com invoices
  - Cotacoes ficam presas ao e-mail individual (sem visibilidade do time)
  - Follow-up manual de cotacoes
- **Status:** Em uso -- parcialmente substituido por e-mails padronizados do software

### Google Drive
- **Categoria:** Armazenamento de Arquivos
- **Usuarios:** Projetos/Arquitetura (PDFs de plantas), Orcamento (arquivos de budget), Contratos (copias assinadas organizadas por pasta)
- **Finalidade:** Armazenamento de PDFs, plantas, contratos, documentos gerais
- **Limitacoes Reportadas:**
  - Organizacao manual
  - Sem versionamento automatico
  - Dificuldade de encontrar versao atualizada (Pedro Henrique: "pesquisei e apareciam 30.000 coisas")
  - Falta de centralizacao entre setores
- **Status:** Em uso -- backup automatico planejado

### BlueBeam
- **Categoria:** Software de Engenharia / Takeoff
- **Usuarios:** Arquitetura (Candida Tenorio, Gabriela Medeiros, equipe no Brasil)
- **Finalidade:** Quantificacao de materiais a partir de PDFs, takeoff de areas, volumes, quantidades
- **Limitacoes Reportadas:**
  - Funcao paga de link com planilhas nunca foi utilizada
  - Compilacao de resultados e manual (lista no Word)
  - CPUs da Lakeshore nao rodam adequadamente
- **Status:** Em uso -- possivel integracao futura via API

### AutoCAD
- **Categoria:** Software de Arquitetura
- **Usuarios:** Equipe de Projetos (Camila, Luana, equipe)
- **Finalidade:** Projeto arquitetonico, desenvolvimento de plantas
- **Limitacoes Reportadas:**
  - Problemas de instalacao/login
  - CPUs da empresa com pouca potencia de video
- **Status:** Em uso

### SketchUp
- **Categoria:** Modelagem 3D
- **Usuarios:** Equipe de Arquitetura (todos exceto Camila)
- **Finalidade:** Modelagem 3D de casas
- **Limitacoes Reportadas:**
  - CPUs nao rodam adequadamente
- **Status:** Em uso

### Enscape
- **Categoria:** Renderizacao 3D
- **Usuarios:** Victoria Vidal, Candida Tenorio, Henrique Lima
- **Finalidade:** Renderizacao de imagens 3D de projetos
- **Limitacoes Reportadas:**
  - CPUs insuficientes
- **Status:** Em uso

### Lumion
- **Categoria:** Renderizacao 3D Alternativa
- **Usuarios:** Henrique Lima (alternativa ao Enscape)
- **Finalidade:** Renderizacao alternativa
- **Limitacoes Reportadas:**
  - Mesmos problemas de hardware
- **Status:** Em uso

### Photoshop
- **Categoria:** Edicao de Imagem
- **Usuarios:** Gabriela Medeiros, Candida Tenorio
- **Finalidade:** Plantas humanizadas
- **Limitacoes Reportadas:**
  - Licenca compartilhada
- **Status:** Em uso

### Software Globin
- **Categoria:** Software de Calculo de Takeoff
- **Usuarios:** Equipe de Takeoff (Gabriela Medeiros)
- **Finalidade:** Calculo de areas, alturas, profundidades (desenho sobre planta)
- **Limitacoes Reportadas:**
  - Conversao de areas em unidades e manual (formulas a parte)
- **Status:** Em uso -- a definir substituicao

### HubSpot
- **Categoria:** CRM / Plataforma de Atendimento
- **Usuarios:** Client Relations (Juliana Theodoro, equipe)
- **Finalidade:** Atendimento ao cliente integrado (WhatsApp, ligacoes, e-mail)
- **Limitacoes Reportadas:**
  - Apenas Juliana tem telefone disponivel (limitacao de usuarios)
  - Ainda em fase de implementacao
- **Status:** Em implementacao

### Brokermint
- **Categoria:** Plataforma de Assinatura Digital
- **Usuarios:** Contratos (Bruna Botelho), Financeiro
- **Finalidade:** Envio de contratos para assinatura digital
- **Limitacoes Reportadas:**
  - Nenhuma reportada (funciona bem)
- **Status:** Em uso -- sera mantido inicialmente

### ChatGPT (IA)
- **Categoria:** Inteligencia Artificial
- **Usuarios:** Equipe de TI/Desenvolvimento (Luciano, Brendda, Evandro), Equipe de Takeoff (Gabriela)
- **Finalidade:** Auxilio na geracao de dados de takeoff, historias de usuario (GPT customizado "User Stories Expert"), coleta de requisitos
- **Limitacoes Reportadas:**
  - Risco de vazamento de historias de usuario (visivel para toda empresa na conta organizacional)
- **Status:** Em uso

### Power BI / Dashboards (Rost, Data Studio)
- **Categoria:** Business Intelligence
- **Usuarios:** Supervisao (Joao Paulo -- Dashboard de Rost), Scheduling (dashboard de construction data), QPS/Analytics (Diego, Rost)
- **Finalidade:** Paineis de acompanhamento, filtragem de dados, analise de tempo de construcao
- **Limitacoes Reportadas:**
  - Gambiarras necessarias para funcionar
  - Dados dispersos como fonte
  - Somente leitura (nao permitem anotacoes)
  - Inconsistencia de dados no Kanban
- **Status:** Em uso -- sera substituido por dashboards integrados no software proprio

### Citros Yocala / Tests
- **Categoria:** Acompanhamento Operacional
- **Usuarios:** Supervisao (Joao Paulo Valenca)
- **Finalidade:** Ferramenta de acompanhamento principal de supervisores (apresentada por Ana)
- **Limitacoes Reportadas:**
  - Unilateral (somente leitura), sem interacao
- **Status:** Em uso

### Sites dos Condados (Property Appraiser, portais de permit)
- **Categoria:** Portais Governamentais
- **Usuarios:** Scheduling (consulta de informacoes de lotes), Inspecao (Dandara -- agendamento de inspecoes), Permits (acompanhamento de revisoes)
- **Finalidade:** Dados de lote, agendamento de inspecoes, acompanhamento de permits
- **Limitacoes Reportadas:**
  - Cada condado tem site diferente com regras proprias (Marion, Citrus, Charlotte)
  - Sem integracao possivel
  - Resultados nem sempre precisos (Citrus via Slack)
- **Status:** Em uso -- sem alternativa

### iPad Notes / Post-its / Caderno Fisico
- **Categoria:** Anotacoes Manuais
- **Usuarios:** Klauser Silva (deposito -- registro de recebimento no iPad Notes), Thercyo (caderno fisico), Giovana (quadro/papel), Scheduling (post-its)
- **Finalidade:** Registro rapido de informacoes no campo, pedidos avulsos
- **Limitacoes Reportadas:**
  - Nao integrado com nenhum sistema
  - Controles improvisados e pessoais
  - Dependem de iniciativa individual
- **Status:** Em uso -- sem alternativa formal

### Software Lakeshore (Ruby on Rails)
- **Categoria:** Software Proprio de Gestao de Construcao
- **Usuarios:** Em fase de validacao com todos os departamentos (+65 horas de entrevistas)
- **Finalidade:** Substituir BuilderTrend, Zorro, Excel, ClickUp e integrar todos os processos em um unico sistema
- **Limitacoes Reportadas:**
  - Em desenvolvimento (meta: junho 2026)
  - Bug de interface (menu sumindo ao clicar)
  - Limite de upload de 20MB insuficiente (precisa 100MB)
  - Falta modo offline/mobile
  - Falta integracao com QuickBooks
- **Status:** Em desenvolvimento

## Matriz Ferramenta x Departamento

| Ferramenta | Orcamento | Compras | Financeiro | Scheduling | Supervisao | Inspecao | Warranty | Projetos | Permits | Client Relations | Utilities | Core Craft | Deposito | Land | RH |
|------------|-----------|---------|------------|------------|------------|---------|----------|----------|---------|-----------------|-----------|------------|----------|------|-----|
| BuilderTrend | X | X | X | X | X | X | X | X | X | X | X | X | X | X | - |
| QuickBooks | - | - | X | - | - | - | - | - | - | - | - | - | - | - | - |
| Zorro | - | X | - | - | - | - | - | - | - | - | - | X | X | - | - |
| Excel/Sheets | X | X | X | X | X | X | X | X | X | X | X | X | X | - | X |
| ClickUp | X | - | - | - | - | - | - | X | - | - | X | - | - | X | - |
| Slack | - | - | X | X | - | X | X | - | - | X | X | X | - | - | X |
| WhatsApp | X | X | - | X | - | - | X | - | - | X | - | X | X | X | - |
| E-mail | X | X | X | - | - | X | X | X | X | - | X | - | - | - | - |
| Google Drive | X | - | - | - | - | - | - | X | - | - | - | - | - | - | - |
| BlueBeam | - | - | - | - | - | - | - | X | - | - | - | - | - | - | - |
| AutoCAD | - | - | - | - | - | - | - | X | - | - | - | - | - | - | - |
| SketchUp | - | - | - | - | - | - | - | X | - | - | - | - | - | - | - |
| HubSpot | - | - | - | - | - | - | - | - | - | X | - | - | - | - | - |
| Brokermint | - | - | X | - | - | - | - | - | - | - | - | - | - | - | - |
| ChatGPT | X | - | - | - | - | - | - | X | - | - | - | - | - | - | - |
| Power BI | - | - | - | X | X | - | - | - | - | - | - | - | - | - | - |
| Sites Condados | - | - | - | X | - | X | - | - | X | - | X | - | - | - | - |
| Globin | X | - | - | - | - | - | - | X | - | - | - | - | - | - | - |

## Gaps de Automacao

Processos atualmente manuais onde falta ferramenta adequada:

| Departamento | Processo Manual | Impacto | Ferramenta Ideal |
|--------------|-----------------|---------|------------------|
| Financeiro | Inclusao de classe no QuickBooks (86 bills = 2h/dia) | Alto -- horas perdidas diariamente | Integracao automatica software-QuickBooks |
| Compras | Distribuicao contabil manual entre casas (Zorro nao integra) | Alto -- 12+ planilhas abertas | Sistema unificado de compras com rateio automatico |
| Scheduling | Preenchimento 3x da mesma informacao (daily log + schedule + PO) | Alto -- todos os schedulers reclamam | Sistema que propaga informacao automaticamente |
| Orcamento | Atualizacao manual de 3.500 itens entre modelos similares | Alto -- dias de trabalho manual | Template com duplicacao automatica de valores |
| Takeoff | Compilacao manual do BlueBeam para lista no Word | Medio -- retrabalho em cada projeto | Integracao BlueBeam via API ou takeoff no software |
| Inspecao | Verificacao manual de remocao de holds (sem notificacao) | Alto -- risco de casas paradas sem necessidade | Notificacao automatica quando hold removido |
| Warranty | Sem software dedicado (3 daily logs por reparo) | Alto -- prejuizos nao rastreados ($14k em caso extremo) | Modulo de warranty com portal do cliente |
| Permits | Gestao de modifications/extensions completamente manual | Alto -- risco de permit expirar sem aviso | Tracking automatico de validade e renovacao |
| Client Relations | Portal do cliente desatualizado (schedule, budget) | Alto -- gera reclamacoes e desconfianca | Atualizacao em tempo real do portal |
| Utilities | Triplo registro (planilha + daily logs + campos BT) | Medio -- retrabalho diario | Registro unico com propagacao |
| RH | Calculo manual de PTOs, cargas, expiracoes | Baixo -- processo demorado mas de baixo volume | Automatizacao de calculos e saldos |
| Deposito | "Peregrinacao" entre Zorro, BT, planilhas, Notes, WhatsApp | Alto -- perda de tempo e erros | Sistema unico de gestao de deposito |
| Supervisao | Ferramentas somente leitura (sem anotacoes interativas) | Medio -- supervisores criam workarounds | Visualizacao interativa com anotacoes |
| Core Craft | Valores de servicos indefinidos no momento da execucao | Medio -- equipe executa sem saber custos | Tabela de precos integrada ao agendamento |
| Orcamento | Follow-up manual de cotacoes com fornecedores por e-mail | Medio -- cotacoes perdidas em e-mails individuais | E-mail automatizado com tracking de respostas |
| Financeiro | Bills artificiais para fechamento de casas sem invoice real | Medio -- risco de valores incorretos | Estimativa automatica baseada em historico |

## Notas

### Ferramentas em transicao
- **BuilderTrend -> Software proprio Lakeshore (Ruby on Rails)**: Substituicao completa planejada. Software em desenvolvimento com meta para junho 2026. Ja validado com multiplos departamentos (+65 horas de entrevistas).
- **Zorro -> Software proprio**: Gestao de estoque sera absorvida pelo novo sistema.
- **Excel/Google Sheets -> Software proprio**: Objetivo explicito de Bernardo e a eliminacao de planilhas.
- **ClickUp -> Software proprio**: Tracking de tarefas sera integrado.

### Integracao entre ferramentas (ou falta dela)
- **BuilderTrend <-> QuickBooks**: Integracao incompleta. Data de vencimento nao serve como criterio. Processo manual de sincronizacao.
- **Zorro <-> BuilderTrend**: Zero integracao. Informacoes duplicadas manualmente entre os dois sistemas.
- **Zorro <-> Planilhas**: Zero integracao. Klauser registra no iPad Notes e copia para planilhas.
- **BlueBeam <-> Planilhas**: Funcao paga de link com planilhas nunca foi utilizada. Compilacao manual no Word.
- **Slack <-> BuilderTrend**: Bots de notificacao parcialmente configurados, mas inconsistentes.
- **Google Drive <-> Qualquer sistema**: Sem integracao. Upload manual de arquivos.

### Problema critico: Hardware
- CPUs da Lakeshore nao rodam adequadamente: AutoCAD, SketchUp, Enscape, BlueBeam
- Candida e Gabriela usam computadores pessoais para trabalhar
- Internet ruim no campo impede uso efetivo de Slack e BuilderTrend

---

### Infraestrutura de TI (Fonte: Drive QPS)

#### AWS (Amazon Web Services)
- **Categoria:** Plataforma de Nuvem
- **Servicos em uso:**
  - **Lambda:** Execucao de codigo serverless (sem servidor dedicado), escala automaticamente por demanda
  - **EventBridge:** Roteamento de eventos entre servicos, usado para arquiteturas orientadas a eventos e agendamentos (substitui cron jobs)
  - **Step Functions / State Machine:** Orquestracao de workflows com multiplos servicos AWS em sequencia com condicoes e transicoes
  - **Lightsail:** Servidores virtuais simplificados, usado para hospedar apps leves como Slack bots com Flask
  - **EC2 Windows:** Servidor virtual Windows na nuvem, usado para hospedar o Power BI Gateway
- **Acesso:** Solicitar a Diego Araujo ou Alexandre Lira -- cadastro via e-mail corporativo com MFA obrigatorio
- **Link:** AWS Console (https://aws.amazon.com/console/)
- **Autenticacao:** Multi-Factor Authentication (MFA) obrigatorio; chave .pem para acesso a instancias EC2
- **Status:** Em uso pela equipe de TI

#### Power BI Premium
- **Categoria:** Business Intelligence / Dashboards
- **Modelo:** Conta unica centralizada (Premium) -- todos os dashboards sob uma unica conta corporativa
- **Acesso:** Credenciais no board do Canva no canal Slack "#qps-tqm-private"
- **Link:** Power BI Portal (https://app.powerbi.com/)
- **Gateway:** Hospedado em instancia EC2 Windows ("power-bi-gateway") para conexao com fontes de dados locais
- **Usuarios:** Diego Araujo, Rost, Joao Paulo Valenca, equipe de Analytics
- **Status:** Em uso -- sera complementado por dashboards integrados no software proprio

#### PostgreSQL (Banco de Dados)
- **Categoria:** Banco de Dados Relacional
- **Acesso:**
  - Credenciais em arquivo .docx na pasta "IT Lakeshore" da conta support@lakeshoredevelopmentfl.com
  - Credenciais tambem disponiveis no board do Canva no canal "#qps-tqm-private"
  - Solicitar criacao de role de desenvolvedor a Diego Araujo ou Alexandre Lira
  - Alternativa: usar usuario admin para criar usuario proprio
- **Status:** Em uso -- banco principal do software Lakeshore (Ruby on Rails)

#### GitHub
- **Categoria:** Repositorio de Codigo / Controle de Versao
- **Acesso:** Usar e-mail support (support@lakeshoredevelopmentfl.com) para convidar e-mail corporativo ao repositorio
- **Status:** Em uso -- repositorio do software proprio Lakeshore

#### EC2 Windows (Power BI Gateway)
- **Categoria:** Servidor Virtual na Nuvem
- **Instancia:** "power-bi-gateway"
- **Acesso:**
  - Conexao via opcao "RDP Client" no console AWS
  - Arquivo de chave necessario: "connect-ec2-gateway.pem" (disponivel na pasta "IT Lakeshore" da conta support)
  - Usar o arquivo .pem para recuperar a senha da instancia e completar a conexao
- **Finalidade:** Hospedar Power BI Gateway para atualizacao em tempo real dos dashboards com fontes de dados internas
- **Status:** Em uso

#### Requisitos Minimos de Hardware (TI)
- **Processador:** Intel i5 (ou equivalente) rodando a 3 GHz
- **Memoria RAM:** 12 GB minimo
- **Armazenamento:** SSD (obrigatorio)
- **Justificativa:** Certas aplicacoes Power BI exigem RAM significativa -- especificacoes acima sao o minimo recomendado
- **Observacao:** CPUs atuais da Lakeshore nao atendem adequadamente para AutoCAD, SketchUp, Enscape e BlueBeam -- funcionarios usam computadores pessoais como alternativa

---

## Navegacao

- [Indice Geral](INDICE.md)
- [Organograma](01_ORGANOGRAMA.md)
- [Glossario de Termos](03_GLOSSARIO.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- [Catalogo de Dores](07_CATALOGO_DORES.md)
- [Fluxo Spec Home](05_FLUXO_SPEC_HOME.md)
- [Fluxo Custom Home](06_FLUXO_CUSTOM_HOME.md)
