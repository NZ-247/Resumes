
O modelo OSI (Open Systems Interconnection) é uma estrutura de referência em camadas que padroniza as funções de um sistema de comunicação em sete níveis. Cada camada fornece serviços à camada imediatamente superior e utiliza os serviços da camada abaixo. A seguir, veremos um resumo de cada camada até a de transporte.

---

### 🧱 Camada 1 – Física (Physical Layer)

- Responsável por transmitir bits crus (0s e 1s) através do meio físico (cabos, ondas de rádio, etc).
- Define características elétricas, ópticas e mecânicas dos dispositivos.
- **Exemplos de tecnologias**: Ethernet (físico), cabos UTP, fibra óptica, sinal Wi-Fi.

---

### 🔗 Camada 2 – Enlace de Dados (Data Link Layer)

- Função principal: transformar um meio físico propenso a erros em um canal confiável.
- Organiza os bits em **quadros (frames)** e realiza a comunicação entre dispositivos diretamente conectados.
- É dividida em duas subcamadas:
  - **MAC (Media Access Control)**: Gerencia o acesso ao meio físico, utiliza **endereços MAC** para identificação exclusiva de dispositivos.
  - **LLC (Logical Link Control)**: Controla os protocolos de enlace e possibilita o uso de múltiplos protocolos de camada superior.
- **Responsabilidades principais**:
  - Controle de acesso ao meio (ex: CSMA/CD na Ethernet)
  - Detecção e correção de erros
  - Controle de fluxo
- **Protocolos e tecnologias associadas**:
  - **Ethernet** (IEEE 802.3)
  - **Wi-Fi** (IEEE 802.11)
  - **PPP**, **HDLC**, entre outros

---

### 🌐 Camada 3 – Rede (Network Layer)

- Responsável por entregar pacotes de um host de origem para um host de destino através de múltiplas redes.
- Lida com o **endereçamento lógico** (ex: endereços IP).
- Define o roteamento, fragmentação de pacotes e controle de congestionamento.
- **Protocolos e tecnologias associadas**:
  - **IP (IPv4 / IPv6)**: Protocolo de endereçamento e roteamento de pacotes.
  - **ICMP**: Diagnóstico e mensagens de erro (ex: ping).
  - **Roteadores** atuam nesta camada.

---

### 🚚 Camada 4 – Transporte (Transport Layer)

- Garante a entrega completa e confiável de dados entre os sistemas finais.
- Divide dados das aplicações em segmentos, entrega e reordena os dados no destino.
- Pode prover:
  - Conexão orientada (com controle de erro e fluxo) → **TCP**
  - Serviço sem conexão, mais rápido e com menos sobrecarga → **UDP**

---

### 📦 TCP – Transmission Control Protocol (Protocolo de Controle de Transmissão)

- **Protocolo da camada de transporte orientado à conexão.**
- Utiliza um **handshake de três vias (three-way handshake)** para estabelecer a conexão:
  - **SYN → SYN-ACK → ACK**
- Responsável por:
  - Fragmentar e numerar dados (segmentos)
  - Garantir a **entrega ordenada** e **sem erros**
  - **Controlar o fluxo** e **retransmitir pacotes perdidos**
- **Processo básico**:
  1. A aplicação (ex: HTTP) solicita envio de dados.
  2. TCP divide em segmentos e entrega ao IP.
  3. IP roteia os pacotes.
  4. No destino, TCP reordena os pacotes e entrega à aplicação.
- **Bandeiras TCP (Flags)**:
  - **SYN**: Início de conexão
  - **ACK**: Confirmação
  - **RST**: Reset da conexão
  - **FIN**: Fim da conexão
  - **PSH**: Entrega imediata
  - **URG**: Dados urgentes

---

### 📊 Exemplo de Funcionamento do TCP

> Ao carregar uma página web, o navegador usa HTTP (camada de aplicação), que solicita ao TCP (camada de transporte) que envie dados. O TCP cria segmentos numerados, envia via IP e, no destino, todos os segmentos são reagrupados e enviados à aplicação.

