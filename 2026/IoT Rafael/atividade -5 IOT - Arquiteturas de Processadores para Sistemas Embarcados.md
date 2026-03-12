
---

As arquiteturas criadas ao longo dos anos passaram, para dar suporte aos recursos computacionais de processamento de instruções, por uma constante evolução, acompanhada pelas principais tendências do mercado.

Com o surgimento de novos dispositivos e diferentes formas de comunicação, as arquiteturas tiveram que ser adaptadas para conseguir suprir os requisitos de aplicações em diversas áreas industriais, principalmente os relacionados aos dispositivos de IoT em sistemas embarcados com limitações de recursos e inseridos em ambientes de atividades críticas.

Nesta Unidade de Aprendizagem, você aprenderá a diferenciar as arquiteturas RISC e CISC, a avaliar as tecnologias ARM em arquiteturas de processadores para sistemas embarcados e a definir os diversos tipos de estruturas que compõem a família de processadores ARM. 

Bons estudos.

#### Ao final desta Unidade de Aprendizagem, você deve apresentar os seguintes aprendizados:

- Definir a família de processadores ARM.
- Classificar a arquitetura RISC.
- Avaliar o uso massivo da tecnologia ARM em sistemas embarcados.

---

# Arquitetura ARM e Dispositivos Embarcados — Resumo

## 1. Arquitetura ARM

A **ARM (Advanced RISC Machine)** é uma arquitetura de processadores baseada no modelo **RISC**, muito utilizada em:

- sistemas embarcados
    
- smartphones
    
- tablets
    
- dispositivos IoT
    
- Raspberry Pi
    

### Características

- **baixo consumo de energia**
    
- **alto desempenho por watt**
    
- arquitetura **RISC**
    
- muito usada em **dispositivos móveis**
    

---

# RISC vs CISC

## RISC (Reduced Instruction Set Computer)

Características:

- instruções **simples**
    
- execução rápida
    
- uso intenso de **registradores**
    
- arquitetura **load/store**
    

Exemplos:

- ARM
    
- RISC-V
    

---

## CISC (Complex Instruction Set Computer)

Características:

- instruções **complexas**
    
- maior variedade de modos de endereçamento
    
- acesso direto à **memória**
    

Exemplos:

- Intel
    
- AMD (x86)
    

---

# Evolução da Arquitetura ARM

A arquitetura ARM evoluiu para melhorar:

- desempenho
    
- eficiência energética
    
- suporte a novas tecnologias
    

### Principais versões

|Arquitetura|Características|
|---|---|
|ARMv6|usada em dispositivos antigos|
|ARMv7|maior desempenho e novos recursos|
|ARMv8|suporte a **32 bits e 64 bits**|

---

# Modos da ARMv8

A arquitetura **ARMv8** possui dois modos de execução:

### AArch32

- executa **instruções de 32 bits**
    
- compatibilidade com arquiteturas anteriores
    

### AArch64

- executa **instruções de 64 bits**
    
- maior capacidade de processamento
    
- mais registradores
    

---

# Linhas de Processadores ARM

A arquitetura ARM possui três linhas principais.

## Linha A (Cortex-A)

Voltada para **alto desempenho**.

Usada em:

- smartphones
    
- tablets
    
- Raspberry Pi
    
- sistemas operacionais completos
    

Características:

- suporte a Linux e Android
    
- alto poder de processamento
    

---

## Linha R (Cortex-R)

Voltada para **sistemas de tempo real**.

Usada em:

- automóveis
    
- controle industrial
    
- sistemas críticos
    

Características:

- memória **determinística**
    
- alta confiabilidade
    
- baixa latência
    

---

## Linha M (Cortex-M)

Voltada para **microcontroladores**.

Usada em:

- IoT
    
- sensores
    
- dispositivos embarcados simples
    

Exemplos:

- Cortex-M23
    
- Cortex-M33
    

Características:

- baixo consumo de energia
    
- baixo custo
    
- processamento eficiente
    

---

# Raspberry Pi e Arquitetura ARM

Os dispositivos **Raspberry Pi** utilizam processadores baseados em ARM.

### Evolução

|Modelo|Arquitetura|
|---|---|
|Raspberry Pi 1|ARMv6|
|Raspberry Pi 2|ARMv7|
|Raspberry Pi 3+|ARMv8|

A evolução trouxe:

- maior desempenho
    
- suporte a mais sistemas operacionais
    
- melhor capacidade de processamento
    

---

# Extensões da Arquitetura ARM

Para melhorar o desempenho, a ARM criou diversas extensões.

## TrustZone

Tecnologia de **segurança**.

Divide o sistema em:

- ambiente **seguro**
    
- ambiente **não seguro**
    

---

## NEON / Advanced SIMD

Tecnologia para **processamento vetorial**.

Usada em:

- multimídia
    
- processamento de imagem
    
- cálculos paralelos
    

---

## Virtualization

Permite executar **máquinas virtuais** em sistemas ARM.

Muito usado em:

- servidores ARM
    
- cloud computing
    

---

## Cryptographic Extension

Acelera operações de **criptografia** no hardware.

Usada em:

- segurança
    
- comunicação segura
    
- proteção de dados
    

---

# ARM e Inteligência Artificial

A ARM vem desenvolvendo tecnologias para suportar **algoritmos de IA**.

## Projeto Trillium

Projeto criado para melhorar:

- **machine learning**
    
- **redes neurais**
    
- **processamento de visão computacional**
    

Inclui:

- **NPU (Neural Processing Unit)**
    
- aceleração de algoritmos de IA
    
- maior eficiência energética
    

---

# Conceitos Importantes para Prova

### Arquitetura ARM

- baseada em **RISC**
    
- usada em **sistemas embarcados**
    

### ARMv8

- suporta **32 bits e 64 bits**
    

### Linhas ARM

- **Cortex-A → alto desempenho**
    
- **Cortex-R → tempo real**
    
- **Cortex-M → microcontroladores**
    

### Extensões

- TrustZone
    
- NEON
    
- Virtualization
    
- Cryptographic
    

### IA na ARM

- **Projeto Trillium**
    

---

# O que mais costuma cair em prova

Estude principalmente:

1. Diferença **RISC vs CISC**
    
2. Linhas **Cortex A / R / M**
    
3. Evolução **ARMv6 → ARMv7 → ARMv8**
    
4. Modos **AArch32 e AArch64**
    
5. Tecnologias **TrustZone e NEON**
    
6. **Projeto Trillium (IA)**

---

