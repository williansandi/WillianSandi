<h1 align="center">Willian Sandi</h1>
<h3 align="center">Entrepreneur & Software Developer — construo soluções automatizadas que colocam tecnologia para trabalhar.</h3>

<p align="center">
  Empreendedor e dono de negócio que resolve problemas reais escrevendo código: automação de processos, integração de sistemas e produtos de software de ponta a ponta — do backend à experiência do usuário.
</p>

###

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=williansandi&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=6&theme=dracula&hide_border=false" height="150" alt="languages graph"  />
</div>

###

<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="30" alt="python logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" height="30" alt="typescript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" height="30" alt="react logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flutter/flutter-original.svg" height="30" alt="flutter logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/dart/dart-original.svg" height="30" alt="dart logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" height="30" alt="html5 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="30" alt="css3 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" height="30" alt="csharp logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="30" alt="javascript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" height="30" alt="docker logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/visualstudio/visualstudio-plain.svg" height="30" alt="visualstudio logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" height="30" alt="vscode logo"  />
</div>

###

## 🚀 Portfólio de Projetos

> A maior parte dos meus projetos roda em repositórios **privados**, pois são produtos e ferramentas de uso próprio ou comercial. Aqui apresento a **arquitetura, o stack e a engenharia** por trás de cada um — sem entrar em estratégia de negócio, nicho ou dados sensíveis — para mostrar como penso e construo software na prática.

<br>

### 📱 App Mobile — Bora Poupar
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-blue)
![Flutter](https://img.shields.io/badge/Flutter-02569B?logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?logo=dart&logoColor=white)

Aplicativo mobile multiplataforma construído em **Flutter/Dart**, com uma única base de código para iOS e Android. A engenharia é focada em experiência nativa e responsividade: gerenciamento de estado reativo, camada de cache local para uso com conectividade instável e sincronização assíncrona com backend em nuvem, priorizando telas fluidas mesmo sob carga de dados.

<br>

### 🤖 Robô de Automação — Canal Ref (MetaTrader 5)
![Status](https://img.shields.io/badge/status-em%20produção-brightgreen)
![MQL5](https://img.shields.io/badge/MQL5-1a1a2e)

Expert Advisor desenvolvido em **MQL5**, operando de forma autônoma e ininterrupta dentro do MetaTrader 5. O projeto tem como foco a engenharia de automação em si: módulo próprio de gerenciamento de risco, filtros de entrada parametrizáveis, logging detalhado de cada operação e rotinas de auto-proteção contra falhas de conexão e eventos atípicos de mercado — sem entrar em detalhes da estratégia utilizada.

<br>

### ⚙️ Automação de Trading — Conector MT4
![Status](https://img.shields.io/badge/status-em%20produção-brightgreen)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![ZeroMQ](https://img.shields.io/badge/ZeroMQ-message%20queue-white)
![Flask](https://img.shields.io/badge/Flask-web%20panel-000000?logo=flask&logoColor=white)

Sistema de automação em **Python** que integra o MetaTrader 4 a um serviço de execução externo através de uma arquitetura de **microsserviços orientada a eventos** (ZeroMQ pub/sub). Sinais são capturados, normalizados e passam por um pipeline de validação antes de chegar à execução. Destaques de engenharia:
- **Supervisor com autorrecuperação (watchdog)** — detecta serviços que caíram e os reinicia sozinho;
- **Painel web de controle** (Flask) para configuração e monitoramento em tempo real;
- **Notificações automáticas** via Telegram (resumos e alertas críticos);
- **Suíte de testes unitários** cobrindo os módulos críticos do pipeline;
- Arquitetura pensada para rodar de forma resiliente e desatendida em VPS.

<br>

### 💬 Assistente Conversacional com IA — Chatbot da Gabi
![Status](https://img.shields.io/badge/status-em%20produção-brightgreen)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![LLM](https://img.shields.io/badge/LLM-API%20integration-412991)
![Telegram](https://img.shields.io/badge/Telegram-Bot%20API-26A5E4?logo=telegram&logoColor=white)

Assistente conversacional em **Python**, integrado a um LLM via API e operando como bot no Telegram. O foco técnico do projeto é a inteligência por trás da conversa, não o assunto tratado:
- **Memória em múltiplas camadas** (curto, médio e longo prazo), mantendo coerência e continuidade em conversas longas;
- **Motor de raciocínio contextual**, que ajusta respostas com base no histórico e no estado atual da interação;
- **Máquina de estados para engajamento**, com lógica automatizada de reengajamento proativo baseada em regras;
- Arquitetura pensada para personalidade consistente e resposta em tempo real.

<br>

---

<p align="center">
  <i>Projetos privados são apresentados aqui em nível de arquitetura e stack técnico, com autorização e sem exposição de dados de negócio.</i>
</p>
