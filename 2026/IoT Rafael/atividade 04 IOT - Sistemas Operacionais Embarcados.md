
---

A utilização de sistemas embarcados vem crescendo exponencialmente: muitos utilizam esse tipo de tecnologia e não têm noção da sua existência. Essa popularização está diretamente ligada à melhora da usabilidade, ao barateamento de componentes e à facilidade da construção de protótipos. Contudo, é necessário ter um controle maior sobre o _hardware_ utilizado, para garantir que determinados requisitos sejam cumpridos. Imagine, por exemplo, a complexidade de desenvolver um código que, além de realizar as funções básicas do dispositivo, implemente politicas de segurança, gestão de energia e controle de acesso. Para isso, há _softwares_ que gerenciam todo o sistema e dão possibilidade de implementar funções que, até então, não eram possíveis, chamados _sistemas operacionais_.

Nesta Unidade de Aprendizagem, você conhecerá o que são os sistemas operacionais para sistemas embarcados e como é o ambiente que eles executam. Por fim, entenderá também as diferentes formas de organizar os componentes internos do sistema operacional.

Bons estudos.

#### Ao final desta Unidade de Aprendizagem, você deve apresentar os seguintes aprendizados:

- Definir a aplicação dos sistemas operacionais embarcados.
- Relacionar os ambientes de uso dos sistemas operacionais embarcados.
- Descrever as arquiteturas dos sistemas operacionais embarcados.]

---
# Sistemas Operacionais Embarcados — Resumo

## 1. O que é um Sistema Operacional Embarcado

Um **Sistema Operacional Embarcado (Embedded OS)** é um sistema operacional projetado para **dispositivos específicos**, normalmente integrados diretamente ao hardware.

### Características

- Integrado ao **hardware do dispositivo**
    
- **Otimizado** para poucos recursos
    
- Usado em **sistemas dedicados**
    
- Pode receber **atualizações e subsistemas** pelos desenvolvedores
    

### Exemplos de uso

- IoT
    
- Automóveis
    
- Equipamentos industriais
    
- Roteadores
    
- Smart TVs
    

---

# Arquitetura de Sistemas Operacionais

A arquitetura define **como os componentes do sistema operacional se organizam e se comunicam**.

## 1. Sistema Monolítico

Todo o sistema roda dentro do **kernel**.

### Vantagens

- **Alto desempenho**
    
- Comunicação rápida entre componentes
    

### Desvantagens

- Baixa segurança
    
- Falha em um módulo pode afetar todo o sistema
    

Exemplo:  
Linux tradicional

---

## 2. Sistema em Camadas

O sistema operacional é dividido em **camadas hierárquicas**.

### Características

- Cada camada usa serviços da camada inferior
    
- Melhor organização
    

### Desvantagem

- **Menor desempenho** por causa das várias chamadas entre camadas
    

---

## 3. Microkernel

O **núcleo do sistema é mínimo**.

Ele gerencia apenas:

- comunicação entre processos
    
- gerenciamento básico de memória
    
- escalonamento
    

Outros serviços ficam **fora do kernel**.

### Vantagens

- maior segurança
    
- maior modularidade
    
- maior estabilidade
    

---

# Tipos de Sistemas Operacionais Embarcados
]
Existem dois principais:

## 1. GPOS (General Purpose Operating System)

Sistema operacional de **uso geral**.

### Exemplos

- Linux
    
- Windows
    
- Android
    

### Características

- Não garante **tempo de resposta determinístico**
    
- Usado em sistemas menos críticos
    

---

## 2. RTOS (Real Time Operating System)

Sistema operacional de **tempo real**.

### Características

- garante execução dentro de um **tempo limite**
    
- usado em **sistemas críticos**
    

### Exemplos de aplicação

- controle industrial
    
- sistemas automotivos
    
- equipamentos médicos
    
- robótica
    

### Conceito importante

**Deadline**

Tempo máximo que uma tarefa pode levar para ser executada.

---

# Estrutura de Privilégios do Sistema Operacional

Os sistemas operacionais são divididos em áreas de acesso.

## 1. User Space

Área onde os **programas do usuário são executados**.

### Características

- menor privilégio
    
- não acessa diretamente hardware
    
- não pode modificar o kernel
    

---

## 2. Kernel Space

Área onde roda o **núcleo do sistema operacional**.

### Características

- acesso total ao sistema
    
- controla hardware
    
- gerencia memória e processos
    

---

# Drivers

Drivers são **softwares que permitem ao sistema operacional comunicar-se com hardware específico**.

### Exemplos

- driver de impressora
    
- driver de placa de vídeo
    
- driver de rede
    

Eles funcionam como **ponte entre o hardware e o sistema operacional**.

---

# Conceitos Importantes para Prova

### Sistema Operacional Embarcado

- otimizado
    
- adaptado ao hardware
    
- atende requisitos da aplicação
    

### Arquiteturas

- monolítico
    
- camadas
    
- microkernel
    

### Tipos de SO

- **GPOS**
    
- **RTOS**
    

### Estrutura

- user space
    
- kernel space
    
- drivers
    

---

# O que mais costuma cair em prova

Estude principalmente:

1. Diferença entre **RTOS e GPOS**
    
2. Diferença entre **User Space e Kernel Space**
    
3. Arquiteturas de SO
    
4. Função dos **drivers**
    
5. Características de **sistemas embarcados**
    

---
