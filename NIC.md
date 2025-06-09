# Placa de Interface de Rede (NIC) — Resumo para CompTIA A+

## 📌 Função Básica

A NIC (Network Interface Card) permite que computadores e servidores se conectem a redes, funcionando como interface entre o dispositivo e a rede.

### Atua nas seguintes camadas:

- **Camada física** → transmissão de sinais
- **Camada de rede (TCP/IP)** → entrega de pacotes de dados

---

## 📌 Componentes Principais de uma NIC

- **Controlador:** mini CPU que processa os dados de rede.
- **Boot ROM:** permite inicialização pela rede (*boot remoto*), útil em estações sem disco.
- **Porta de conexão:** conecta fisicamente a rede:
    - RJ45 (par trançado)
    - BNC (coaxial fino)
    - AUI (coaxial grosso)
    - Porta óptica (fibra óptica)
- **Interface de barramento:** conecta NIC ao computador/servidor:
    - PCIe
    - PCI
    - USB
- **LEDs indicadores:** mostram o status da conexão e transmissão.
- **Suporte físico:** fixação em slot de expansão:
    - Altura total (12 cm)
    - Baixo perfil (8 cm)

---

## 📌 Tipos de NIC

### Por meio de conexão

- **NIC com fio:** utiliza cabos Ethernet ou fibra óptica.
- **NIC sem fio:** utiliza antena e rádio (Wi-Fi).

### Por tipo de barramento (interface com o computador)

| Tipo | Observações |
|------|-------------|
| ISA  | Obsoleto, 9 Mbps |
| PCI  | Até 266 MBps |
| PCI-X | Até 1064 MBps |
| PCIe | Atual, diversas versões e velocidades |
| USB  | Versátil, para NICs externas |

### Por tipo de porta de conexão

| Porta | Cabo Utilizado |
|-------|----------------|
| RJ45  | Par trançado (Cat 5, Cat 6) |
| AUI   | Coaxial grosso |
| BNC   | Coaxial fino |
| Óptica| Fibra óptica |

---

## 📌 Velocidades de Transmissão Comuns

| Velocidade         | Aplicação Típica |
|--------------------|------------------|
| 10 Mbps            | Muito básico, obsoleto |
| 100 Mbps           | Pequenas redes domésticas e escritórios |
| 1 Gbps (1000 Mbps) | Rede Gigabit — padrão moderno |
| 10 Gbps            | Empresas e data centers |
| 25 Gbps ou mais    | Data centers, alta performance |

---

## 📌 Diferenças entre NIC de PC e NIC de Servidor

| NIC de PC                                | NIC de Servidor |
|------------------------------------------|-----------------|
| Geralmente integrada na placa-mãe        | Alta velocidade (10G, 25G, 40G, 100G) |
| Velocidades padrão (100 Mbps - 1 Gbps)   | Otimizada para virtualização e alto desempenho |
| Usa mais recursos da CPU                 | Possui controlador dedicado para aliviar a CPU |

---

## 📌 Resumo Final

- A NIC é um componente essencial para a conectividade em rede.
- Existem tipos e velocidades de NIC adequadas para diferentes cenários: doméstico, profissional e data center.
- A maioria dos PCs modernos possui NIC integrada.
- Servidores utilizam NICs especializadas para atender demandas de alta performance.

---

# ✅ Dicas para Documentar no Kaggle e GitHub

- **Estrutura com Títulos (`#`, `##`, `###`)** para facilitar navegação por TOC (Table of Contents).
- **Tabelas**: tornam a informação mais legível.
- **Emojis (opcional)**: ajudam a destacar seções importantes.
- **Separadores (`---`)**: melhoram a separação visual entre blocos de conteúdo.
- No **GitHub**, usar como `README.md` principal ou em subpastas específicas de estudos para o CompTIA A+.
- No **Kaggle**, criar um **Notebook** com células de código + Markdown, mantendo o conteúdo sempre em Markdown para referência rápida durante os estudos.

---

