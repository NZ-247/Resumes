# Fundamentos CompTIA A+ – Cabos de Fibra Óptica

## Estrutura de um Cabo de Fibra Óptica

- Núcleo feito de **vidro** (ou plástico), onde o **sinal de luz** é transmitido.
- **Revestimento acrílico** sobre o núcleo, com codificação por cores.
- Envolto em **tubos soltos ou apertados**, reforçados com **fibra de vidro** e **Kevlar**.
- Uma **bainha externa protetora** completa o cabo.

> Os cabos de fibra óptica transmitem **luz**, e não sinais elétricos.

---

## Aplicações dos Cabos de Fibra Óptica

Utilizados em:

- Sistemas de **CFTV (TV de circuito fechado)**
- **Transmissão de dados**
- **LAN/WAN e multimídia**
- Conexões entre **quadros de distribuição**
- **Redes de alta velocidade**
- Ambientes com **interferência eletromagnética** (ex: usinas nucleares)
- **Conexões de longa distância**
- Ambientes que exigem **segurança ponto a ponto**

---

## Construção de um Cabo Óptico

1. **Núcleo e revestimento**: para reflexão interna total.
2. **Camada acrílica**: proteção e codificação.
3. Fibras colocadas em **tubos apertados ou soltos**.
4. Tubos agrupados em formato **multi-tubo** com torção S/Z.
5. Reforço com **Kevlar** ou fibra de vidro.
6. Camadas adicionais: **blindagem metálica** ou **não metálica**.
7. **Conectores ópticos** especiais para terminação.

---

## Tipos de Fibra Óptica

### 1. Multimodo (MMF)

- Diâmetro do núcleo: **50 µm** ou **62,5 µm**
- Diâmetro do revestimento: **125 µm**
- Luz infravermelha com comprimento de onda entre **850 e 1300 nm**
- Transmissão por **vários modos** (caminhos de luz)
- Mais **barata**, mas com **maior atenuação**
- Ideal para: **LANs, distâncias curtas**

#### Subtipos por estrutura de índice:

- **Índice Degrau (Step-Index)**: núcleo com índice de refração constante.
- **Índice Gradual (Graded-Index)**: núcleo com variação gradual de índice.

#### Tipos Padronizados:

| Tipo | Cor         | Núcleo (µm) | Largura de Banda | Distância | Aplicações                         |
|------|-------------|-------------|------------------|-----------|------------------------------------|
| OM1  | Laranja     | 62,5        | 1 Gb @ 850nm     | até 300m  | Redes locais de curto alcance      |
| OM2  | Laranja     | 50          | 1 Gb @ 850nm     | até 600m  | LAN, redes de médio alcance        |
| OM3  | Turquesa    | 50          | 10 Gb @ 850nm    | até 300m  | 10/40/100 GbE com conectores MPO   |
| OM4  | Violeta     | 50          | 10 Gb @ 850nm    | até 550m  | Data centers, campus corporativos |
| OM5  | Verde-limão | 50          | 40-100 Gb/s      | >= 550m   | DWDM, alta largura de banda        |

---

### 2. Monomodo (SMF)

- Núcleo de **~9 µm**
- Transmite luz laser com **comprimento de onda entre 1310 e 1550 nm**
- **Apenas um modo de propagação**
- Alta **velocidade**, **baixa atenuação**
- Ideal para **longas distâncias** (até 100 km)

---

## Comparativo: Multimodo vs. Monomodo

| Característica               | Multimodo                       | Monomodo                          |
|-----------------------------|----------------------------------|-----------------------------------|
| Diâmetro do núcleo          | 50 ou 62,5 µm                    | ~9 µm                             |
| Caminho de luz              | Vários modos                     | Um único modo                     |
| Distância                   | Curta (até 600m)                 | Longa (até 100 km)                |
| Custo do cabo               | Mais caro                        | Mais barato                       |
| Custo de componentes        | Mais barato                      | Mais caro                         |
| Fontes de luz               | LEDs                             | Diodos laser                      |
| Facilidade de terminação    | Mais fácil                       | Mais difícil                      |
| Aplicações                  | LANs, campus                     | WANs, operadoras, backbones       |

---

## Materiais do Revestimento

- Devem ser **resistentes à radiação UV**, **óleo** e **químicos**.
- Influenciam a **resistência mecânica**.
- **PVC** está sendo substituído por materiais **livres de halogênio** (LSZH) por questões ambientais e normativas.

---

## Conclusão

A fibra óptica é fundamental para:

- **Altas velocidades**
- **Baixa latência**
- **Longas distâncias**
- **Ambientes críticos**

A escolha entre **multimodo** e **monomodo** depende da aplicação, distância e orçamento.

> Em redes modernas, a fibra óptica é uma das principais soluções para backbone e comunicação de alta performance.
