<h1 align="center">Willian Sandi</h1>
<h3 align="center">Entrepreneur & Software Developer — construo soluções automatizadas que colocam tecnologia para trabalhar.</h3>

<p align="center">
  Empreendedor e dono de negócio que resolve problemas reais escrevendo código: automação de processos, integração de sistemas e produtos de software de ponta a ponta — do backend à experiência do usuário.
</p>

###

<div align="center">
  <img src="https://github-stats-extended.vercel.app/api/top-langs?username=williansandi&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=6&theme=dracula&hide_border=false" height="150" alt="languages graph"/>
</div>

###

<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="30" alt="python logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" height="30" alt="typescript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="30" alt="javascript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" height="30" alt="react logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flutter/flutter-original.svg" height="30" alt="flutter logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/dart/dart-original.svg" height="30" alt="dart logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/fastapi/fastapi-original.svg" height="30" alt="fastapi logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/firebase/firebase-plain.svg" height="30" alt="firebase logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" height="30" alt="postgresql logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/sqlite/sqlite-original.svg" height="30" alt="sqlite logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" height="30" alt="docker logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" height="30" alt="git logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" height="30" alt="csharp logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" height="30" alt="vscode logo"  />
</div>

###

## 🚀 Portfólio de Projetos

> A maior parte dos meus projetos roda em repositórios **privados**, pois são produtos e ferramentas de uso próprio ou comercial. Aqui apresento a **arquitetura, o stack e a engenharia** por trás de cada um — sem entrar em estratégia de negócio, nicho ou dados sensíveis — para mostrar como penso e construo software na prática.

**Panorama:**

| Projeto | Domínio | Stack principal | Status |
|---|---|---|---|
| Expert Advisor MT5 | Automação | MQL5 | 🟢 Produção |
| Conector MT4 ↔ Serviço externo | Automação / Integração | Python · ZeroMQ · Flask | 🟢 Produção |
| App Mobile de Consumo | Mobile | Flutter · Dart · Firebase | 🔵 Próximo do MVP |
| Bot Conversacional (Telegram) | IA / Conversacional | Python · LLM API · SQLite | 🟡 Pré-lançamento |
| Assistente Pessoal Autônomo | IA / Agentes | Python · FastAPI · React | 🔵 Em desenvolvimento |
| Otimizador de Estratégias | Dados / ML | Python · XGBoost · Optuna | ⏸️ Pausado |
| App de Gestão de Carteira | Mobile / Fintech | React Native · Expo · TS | ⚪ Especificado |
| Laboratório de Execução | Pesquisa | Python · MT5 API | 🔬 Ativo |
| Engenharia Reversa | Pesquisa / Segurança | Ghidra · Análise de binários | 🔬 Ativo |

<br>

---

## 🟢 Em Produção

### 🤖 Expert Advisor — MetaTrader 5
![Status](https://img.shields.io/badge/status-em%20produção-brightgreen)
![MQL5](https://img.shields.io/badge/MQL5-1a1a2e)
![VPS](https://img.shields.io/badge/deploy-VPS%2024%2F7-informational)

Expert Advisor desenvolvido em **MQL5**, operando de forma autônoma e ininterrupta em VPS. O foco do projeto é a engenharia de automação em si — **não a estratégia empregada**:

- Módulo próprio de **gerenciamento de risco** com limites parametrizáveis por sessão;
- **Filtros de entrada configuráveis** e desacoplados da lógica de execução;
- **Máquina de estados persistente**, que sobrevive a reinício do terminal sem perder contexto operacional;
- **Logging estruturado** de cada evento, para auditoria posterior;
- Rotinas de **auto-proteção** contra queda de conexão e eventos atípicos;
- **Licenciamento offline** por instância, com validação local.

Versionamento disciplinado: cada release passa por auditoria de código linha a linha e validação em ambiente isolado antes de ir a produção. Versões anteriores ficam arquivadas e rastreáveis.

<br>

### ⚙️ Conector MT4 ↔ Serviço Externo
![Status](https://img.shields.io/badge/status-em%20produção-brightgreen)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![ZeroMQ](https://img.shields.io/badge/ZeroMQ-message%20queue-white)
![Flask](https://img.shields.io/badge/Flask-web%20panel-000000?logo=flask&logoColor=white)

Sistema de automação em **Python** que integra o MetaTrader 4 a um serviço de execução externo através de uma arquitetura de **microsserviços orientada a eventos** (ZeroMQ pub/sub). Eventos são capturados, normalizados e passam por um pipeline de validação antes da execução.

- **Supervisor com autorrecuperação (watchdog)** — detecta serviços que caíram e os reinicia sozinho;
- **Painel web de controle** (Flask) para configuração e monitoramento em tempo real;
- **Notificações automáticas** via Telegram (resumos periódicos e alertas críticos);
- **Suíte de testes unitários** cobrindo os módulos críticos do pipeline;
- Tratamento explícito de **codificação de arquivos e logs legados** (UTF-16 / CP1252), armadilha clássica de integração com plataformas Windows antigas;
- Arquitetura desenhada para rodar de forma **resiliente e desatendida** em VPS.

<br>

---

## 🔵 Próximo do MVP

### 📱 App Mobile de Consumo
![Status](https://img.shields.io/badge/status-próximo%20do%20MVP-blue)
![Flutter](https://img.shields.io/badge/Flutter-02569B?logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?logo=dart&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black)

Aplicativo mobile multiplataforma em **Flutter/Dart**, base de código única para iOS e Android, com backend serverless em **Firebase**. Projeto mais maduro do portfólio, com boa parte do fluxo de usuário e da camada de segurança já fechados.

**Engenharia:**
- **Design system próprio** (tokens de cor e tipografia centralizados), com rollout controlado tela a tela;
- **OCR on-device** com pipeline de normalização e conferência obrigatória pelo usuário — automação nunca preenche dado sem validação humana;
- **Busca geoespacial** por raio usando indexação **GeoHash**, com paginação obrigatória em toda consulta (controle de custo é requisito de arquitetura, não detalhe);
- **Cloud Functions** para toda lógica sensível — regras de negócio críticas são *server-authoritative*, nunca calculadas no cliente;
- **App Check** com Play Integrity em modo *enforcing*, e regras de segurança versionadas junto do código;
- Camada de **cache local** para uso com conectividade instável e sincronização assíncrona;
- **Pipeline de dados** separado em Python (coleta, ETL e carga), com execução em modo `--dry-run` obrigatória antes de qualquer operação em massa.

<br>

---

## 🟡 Pré-lançamento

### 💬 Bot Conversacional com IA — Telegram
![Status](https://img.shields.io/badge/status-pré--lançamento-yellow)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![LLM](https://img.shields.io/badge/LLM-API%20integration-412991)
![Telegram](https://img.shields.io/badge/Telegram-Bot%20API-26A5E4?logo=telegram&logoColor=white)

Bot conversacional em **Python**, integrado a um LLM via API e operando sobre a Telegram Bot API. O foco técnico é a **inteligência da conversa**, não o assunto tratado:

- **Memória em múltiplas camadas** (curto, médio e longo prazo), mantendo coerência e continuidade em conversas longas;
- **Motor de decisão contextual**, que escolhe a próxima ação com base em histórico e estado atual da interação;
- **Máquina de estados de engajamento**, com lógica de reengajamento proativo baseada em regras e agendamento (APScheduler);
- **Camada de acesso a dados centralizada** (padrão DAO) — nenhum módulo abre conexão com o banco por conta própria;
- **Integração de pagamento e entrega digital automatizada**, com múltiplos provedores atrás de uma interface única;
- **Validação de contratos de dados** com Pydantic em toda fronteira externa;
- **Ferramenta própria de auditoria de documentação**, que compara a data de cada `.md` com a dos módulos que ele referencia e sinaliza documentação obsoleta antes que ela engane alguém.

<br>

---

## 🔵 Em Desenvolvimento

### 🧠 Assistente Pessoal Autônomo
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-blue)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)

Assistente pessoal autônomo com interface de texto e voz. Backend em **Python 3.12 / FastAPI** com comunicação por **WebSocket**, frontend em **React + Vite + TypeScript**, persistência em SQLite.

- **Orquestração multi-provedor de LLM** com cadeia de *failover* automático — se um provedor cai, o próximo assume sem intervenção;
- **Pipeline de voz local**: transcrição com Whisper e síntese com Piper, sem dependência de serviço externo;
- **Camada de segurança autônoma** — validação de origem, varredura de conteúdo, execução em sandbox e quarentena;
- **Capacidade de auto-desenvolvimento**: lê, edita, testa e aplica mudanças no próprio código, com backup e reinício controlado;
- Canal de notificação assíncrono para eventos relevantes.

<br>

---

## ⏸️ Pausado

### 📊 Otimizador Autônomo de Estratégias
![Status](https://img.shields.io/badge/status-pausado-lightgrey)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-ML-EC4E20)
![Optuna](https://img.shields.io/badge/Optuna-hyperparameter%20tuning-2E6DB4)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)

Plataforma de **otimização e validação automatizada** de estratégias, construída como sistema completo — não como script:

- **Orquestrador central** coordenando ciclos de teste, avaliação e ajuste;
- **Otimização de hiperparâmetros com Optuna** e modelagem com **XGBoost** sobre pandas/numpy;
- **API em FastAPI** + **dashboard** para acompanhamento em tempo real;
- **Camada de memória** que acumula resultados entre execuções, para não repetir experimento já feito;
- **Adaptador desacoplado** da plataforma de mercado, isolando a integração do núcleo de otimização;
- Empacotamento em **Docker**, suíte de testes com pytest e lint com ruff.

Pausado por priorização — o código e o ambiente permanecem versionados e reutilizáveis.

<br>

---

## ⚪ Especificado — não iniciado

### 💼 App de Gestão de Carteira
![Status](https://img.shields.io/badge/status-especificado-lightgrey)
![React Native](https://img.shields.io/badge/React%20Native-61DAFB?logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo-000020?logo=expo&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)

Projeto **integralmente especificado antes da primeira linha de código** — 7 documentos cobrindo modelo de dados, motor de cálculo, telas, roadmap por fases com critérios de aceite, e análise de exposição regulatória.

Decisões de arquitetura já fechadas:
- **Motor de cálculo isolado da UI**, em TypeScript puro — roda em Node, com suíte de testes própria. Nenhuma tela calcula valor;
- **Aritmética inteira em centavos** — nunca ponto flutuante em armazenamento, arredondamento só na exibição;
- **Eventos imutáveis** — nada é editado ou deletado; correção acontece por estorno, preservando trilha de auditoria;
- **Separação estrita de camadas de visibilidade** por perfil de usuário;
- Fuso horário fixo em toda operação temporal, nunca o relógio do dispositivo;
- **12 casos de teste definidos como gate** da primeira fase — o motor não é declarado pronto sem eles verdes.

Escrever a especificação antes de codar é deliberado: é a parte do sistema sem conserto barato depois.

<br>

---

## 🔬 Pesquisa e Estudo Contínuo

### 🧪 Laboratório de Execução Automatizada
![Status](https://img.shields.io/badge/status-ativo-success)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)

Ambiente isolado, em conta de demonstração, para desenvolver e validar automações de execução em condições reais de mercado — sem risco financeiro. Serve como campo de prova para ideias que só depois migram para os projetos de produção.

### 🔍 Engenharia Reversa e Análise de Binários
![Status](https://img.shields.io/badge/status-ativo-success)
![Ghidra](https://img.shields.io/badge/Ghidra-NSA-red)

Estudo prático de engenharia reversa com **Ghidra**, operado em **modo headless e scriptado** para análise reproduzível. Metodologia central: **análise diferencial controlada** — compilar variações mínimas de um mesmo fonte e comparar os binários byte a byte para mapear empiricamente a estrutura de formatos fechados.

Escopo restrito a binários próprios, com acesso legítimo. **Finalidade educacional e defensiva.**

<br>

---

## 🛠️ Engenharia & Metodologia

O que se repete em todos os projetos, independente da linguagem:

**Arquitetura**
`Separação de camadas` · `Microsserviços orientados a eventos` · `Padrão DAO / repositório` · `Máquinas de estado` · `Adaptadores para isolar dependência externa` · `Lógica sensível server-authoritative` · `Serverless (Cloud Functions)`

**Qualidade e operação**
`Testes unitários e de integração` · `Critérios de aceite antes do código` · `Validação em pequena escala antes de qualquer operação em massa` · `Watchdog e autorrecuperação` · `Logging estruturado` · `Deploy desatendido em VPS` · `Versionamento semântico com auditoria por release`

**Segurança**
`Credenciais fora do código e do versionamento` · `Validação e sanitização em toda fronteira externa` · `Attestation de app (Play Integrity)` · `Regras de acesso versionadas junto do código` · `Sandbox e quarentena para execução não confiável`

**Dados e IA**
`Integração com LLM multi-provedor com failover` · `Memória persistente em camadas` · `Otimização de hiperparâmetros` · `OCR on-device` · `Indexação geoespacial` · `ETL e pipelines de coleta`

**Processo**
Documentação viva versionada junto do código, decisões de arquitetura registradas com o **porquê** (não só o quê), e engenharia de contexto para agentes de IA — mantendo memória estruturada e auditável entre sessões de trabalho, de forma que a informação certa esteja disponível no momento certo em vez de ser reconstruída toda vez.

<br>

---

<p align="center">
  <i>Projetos privados são apresentados aqui em nível de arquitetura e stack técnico, sem exposição de estratégia, nicho ou dados de negócio.</i>
</p>
