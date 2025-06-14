# 🔐 Segurança - Tipos de Criptografia (CompTIA A+)

Documentação otimizada para estudo da certificação **CompTIA A+**, abordando os tipos de criptografia e sua aplicação nos três estados dos dados: **em movimento**, **em uso** e **em repouso**.

---

## 📌 Conceito de Criptografia

A **criptografia** é o processo de **codificação de dados** de forma que apenas partes autorizadas possam acessá-los, garantindo a **confidencialidade** das informações.

---

## 🔄 Tipos de Criptografia

### 🔒 Criptografia Simétrica

- Mesma chave para **criptografar** e **descriptografar**.
- **Rápida**, ideal para grandes volumes de dados.
- **Algoritmos comuns**:
  - `DES (Data Encryption Standard)`
  - `3DES (Triple DES)`
  - `AES (Advanced Encryption Standard)` → padrão da indústria, com chaves recomendadas de **128 bits ou mais**.

### 🔑 Criptografia Assimétrica

- Usa duas chaves distintas:
  - **Pública** (para criptografar)
  - **Privada** (para descriptografar)
- **Mais lenta**, mas ideal para:
  - **Troca de chaves seguras**
  - **Assinaturas digitais**
- **Algoritmos comuns**:
  - `RSA (Rivest–Shamir–Adleman)`
  - `ECC (Elliptic Curve Cryptography)`

---

## 💽 Estados dos Dados e Criptografia

Os dados podem existir em **três estados** distintos. Todos devem ser protegidos adequadamente com criptografia.

---

### 🚚 Dados em Movimento (Data in Transit)

#### ➤ Definição:
Dados transferidos entre sistemas, redes ou dispositivos (e-mails, uploads, mensagens).

#### ➤ Tecnologias de Proteção:
- `TLS (Transport Layer Security)` → substitui SSL.
- `HTTPS` (HTTP sobre TLS)
- VPNs, túneis seguros

#### ➤ Processo:
1. Sessão segura iniciada com **criptografia assimétrica**.
2. Transmissão contínua com **criptografia simétrica**.

#### ➤ Ameaças:
- Espionagem de tráfego (`eavesdropping`)
- Sniffing de pacotes não criptografados

---

### 🖥️ Dados em Uso (Data in Use)

#### ➤ Definição:
Dados que estão sendo **acessados ou processados ativamente** (ex: RAM, arquivos abertos).

#### ➤ Proteções:
- **Autenticação forte**:
  - `MFA (Autenticação Multifator)`
  - `SSO (Single Sign-On)`
- **Controle de acesso baseado em função** (RBAC)
- **Virtualização Criptografada Segura (SEV)**:
  - Usa `AES-128`
  - Ex: processadores `AMD EPYC`, `Intel SGX`

#### ➤ Ameaças:
- Ataques de autenticação (phishing, brute-force)
- `Cold Boot Attacks`: extração de dados da RAM após desligamento

---

### 💾 Dados em Repouso (Data at Rest)

#### ➤ Definição:
Dados armazenados e não utilizados ativamente (ex: bancos de dados, HDs, SSDs, unidades USB, buckets em nuvem).

#### ➤ Técnicas de Criptografia:
- **Criptografia de disco completo (FDE)**
- **Criptografia de arquivos ou sistemas de arquivos**
- **Criptografia de banco de dados**
- **Criptografia de ativos em nuvem**

#### ➤ Boas Práticas:
- Usar algoritmos padrão como `AES`
- Chaves fortes, rotacionadas periodicamente
- **Gerenciamento seguro das chaves criptográficas**:
  - `HSMs (Hardware Security Modules)`
  - `Cloud KMS`:
    - `Azure Key Vault`
    - `AWS KMS`
    - `Google Cloud KMS`

#### ➤ Ameaças:
- **Exfiltração de dados**
- Acesso físico não autorizado
- Força bruta contra chaves criptográficas

---

## 🔑 Gerenciamento de Chaves Criptográficas

- **Não armazenar chaves junto aos dados**
- Usar **dispositivos dedicados** (`HSMs`)
- Adotar **serviços confiáveis em nuvem**:
  - `Azure Key Vault`
  - `AWS KMS`
  - `GCP KMS`

---

## ✅ Resumo Rápido

| Estado dos Dados | Proteções Comuns                      | Principais Ameaças                     |
|------------------|----------------------------------------|----------------------------------------|
| **Em Movimento** | TLS, HTTPS, VPN                        | Espionagem de tráfego, sniffing        |
| **Em Uso**       | SEV, MFA, SSO, RBAC                    | Cold boot, ataques de autenticação     |
| **Em Repouso**   | AES, FDE, KMS, HSM                     | Exfiltração, acesso físico não autorizado |

---

> **Importante:** a criptografia **não substitui** autenticação, controle de acesso ou políticas de segurança física, mas sim complementa essas práticas.

