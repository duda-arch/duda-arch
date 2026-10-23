### ⚡ Sobre mim

Sou desenvolvedor full-stack com um pé no hardware. Crio automações de IoT para **telemetria e controle remoto**: leitura e parametrização de medidores de energia, monitoramento de sensores e acionamento de equipamentos, via LoRaWAN, MQTT e portas seriais. E construo todo o sistema em volta delas: firmware, coleta, API, banco de dados, painel web e deploy. Gosto de pegar um processo manual e transformar num sistema que roda sozinho, se monitora e avisa quando algo dá errado.

#### 🔌 IoT, telemetria e automação
- **Medidores de energia**: leitura e parametrização remota, via LoRaWAN, MQTT ou diretamente pelas portas seriais
- **Sensores e monitoramento**: temperatura, umidade, sondas de nível e sondas de qualidade do ar
- **Controle e acionamento**: sensores de abertura e fechamento de portas e acionamento remoto de relés
- **Protocolos de medição**: ABNT NBR 14522 para comunicação óptica com multimedidores de energia e Modbus
- **Meios físicos**: RS485, RS232, porta e cabo óptico, UART/TTL, entre outros
- **LoRaWAN de ponta a ponta**: do firmware do dispositivo (OTAA/ABP) à infraestrutura, com broker MQTT, Network Server no ChirpStack e integração com a aplicação
- **Placas próprias com ESP32**: desenvolvimento de placas para integrar aos meus projetos, com Ethernet, modem celular 3G/4G (chip SIM) e NB-IoT
- **Firmware para ESP32-S3** em C/C++ com FreeRTOS: Ethernet W5500, Wi-Fi, display OLED e portal de configuração web embarcado
- Ferramentas de leitura e parametrização de equipamentos legados, em Python, empacotadas como executáveis para Windows e Linux

#### 🔧 Equipamentos com que já trabalhei

| Fabricante | Modelos |
|---|---|
| Schneider Electric | PM210 · PM510 · PM750 · PM5300 · iEM3150 / iEM3250 |
| Kron | Mult-K Plus · Mult-K 120 · Konect Plus RW · CCK7550S · iKron-03 |
| IMS | PowerNET T500 · PowerNET T500-G4 · Smart Trans |
| Landis+Gyr | E34A |
| Carlo Gavazzi | EM330 |
| Pextron | PCPT4 |
| Dragino | WSS-03 (CO2, PM2.5 e PM10) |
| Vini | Vini Modbus |

#### 🤖 Automação de processos e web scraping
- **Automação de tarefas manuais em sites**: transformo funções repetitivas que pessoas fazem em sistemas web (acessar portais, preencher formulários, baixar documentos, conferir e lançar dados) em robôs que rodam sozinhos
- **Dois caminhos, conforme o caso**: automação do navegador com Puppeteer ou engenharia reversa da API do site, chamando diretamente as requisições que a página faz, o que deixa o robô mais rápido e estável
- **Passo por bloqueios de automação**: captchas, detecção de bots e outros sistemas anti-automação
- **Toolkit próprio de engenharia reversa**: grava o tráfego HTTP e WebSocket de um site, mapeia as rotas e replica fluxos completos encadeando tokens
- **Robôs em produção**: pool de navegadores, fila persistida e retomada automática de tarefas
- Parsers de PDF que transformam faturas em dados para o ERP, validados por testes de regressão em mais de 3.700 documentos reais
- Integração com ERP pelo webservice e, onde não existe API, pela automação da própria tela

#### 🏗️ Back-end e operação
- APIs e painéis em Node.js (Express, Socket.io) e Python (Flask), com PostgreSQL e migrações
- Segurança desde o início: login com Google, permissões por usuário, CSRF, validação com Zod, cofre de segredos com AES-256-GCM e trilha de auditoria
- Servidores Linux com nginx, systemd, PM2, backups, health checks e alertas automáticos por WhatsApp

---

### 🛠️ Tecnologias

**Linguagens**

[![Linguagens](https://skillicons.dev/icons?i=py,js,java,c,cpp,bash,powershell&theme=dark)](https://skillicons.dev)

**Back-end e Web**

[![Web](https://skillicons.dev/icons?i=nodejs,express,html,css,bootstrap,postgres,firebase&theme=dark)](https://skillicons.dev)

**Hardware, Infra e Ferramentas**

[![Infra](https://skillicons.dev/icons?i=raspberrypi,arduino,linux,azure,terraform,git,github&theme=dark)](https://skillicons.dev)

![Puppeteer](https://img.shields.io/badge/Puppeteer-40B5A4?style=for-the-badge&logo=puppeteer&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=for-the-badge&logo=socketdotio&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white)
![LoRaWAN](https://img.shields.io/badge/LoRaWAN-1F6FEB?style=for-the-badge&logo=semtech&logoColor=white)
![ChirpStack](https://img.shields.io/badge/ChirpStack-0B4F8A?style=for-the-badge&logo=lora&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white)
![Modbus](https://img.shields.io/badge/Modbus-4A4A4A?style=for-the-badge&logoColor=white)
![RS485](https://img.shields.io/badge/RS485_%7C_RS232-2E7D32?style=for-the-badge&logoColor=white)
![ABNT 14522](https://img.shields.io/badge/ABNT_NBR_14522-009739?style=for-the-badge&logoColor=white)
![WhatsApp](https://img.shields.io/badge/WhatsApp_API-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)
![Capacitor](https://img.shields.io/badge/Capacitor-119EFF?style=for-the-badge&logo=capacitor&logoColor=white)

---

### 🚀 Vitrine de projetos

> A maior parte dos meus projetos é privada, mas aqui está um resumo do que já construí.

| | Projeto | O que faz | Stack |
|:-:|---|---|---|
| 🧾 | **Gestão automática de faturas** | Robôs que entram nos portais das operadoras, baixam as faturas, leem os PDFs e organizam tudo num painel web com fila de tarefas, gráficos e login com Google | Node.js · Express · Puppeteer · PostgreSQL · Socket.io · Chart.js |
| ⚡ | **Telemetria de energia** | Leitura e parametrização remota de medidores de energia via RS485 e sonda óptica, com gateways Raspberry Pi em campo, API de gestão e painel para acompanhar os equipamentos | Python · Raspberry Pi · RS485 · MQTT · Node.js |
| 📡 | **Firmware ESP32 + LoRa** | Firmware para ESP32-S3 com comunicação LoRa para coleta de dados em locais sem internet | C · C++ · PlatformIO |
| 🔌 | **Controle remoto de USB serial** | Serviço que libera ou bloqueia o adaptador serial de uma Raspberry Pi a partir de uma API, com modo à prova de falhas quando fica sem internet | Python · systemd · Node.js |
| 💬 | **Bots de WhatsApp** | Envio de mensagens e atendimento automático, tanto pelo WhatsApp Web quanto pela API oficial da Meta | Node.js · whatsapp-web.js · Python · Meta Cloud API |
| 📱 | **App mobile Android e iOS** | App nativo com notificações push (equipamento offline, faturas vencendo, pagamento confirmado) e build automatizado na nuvem | Capacitor · Firebase · Codemagic |
| ☁️ | **[Infra como código na Azure](https://github.com/duda-arch/terraform_azure)** | Provisionamento de infraestrutura na Azure com Terraform | Terraform · Azure |

---
