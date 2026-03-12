---

---

---

Desenvolver um sistema ou um aplicativo para equipamentos de propósito geral é sempre um desafio, pois há de se contemplar todos os requisitos e transformá-los em código.

Ao se tratar de sistemas embarcados, esta realidade é ainda mais complexa, pois, além dos requisitos do programa, é necessário reunir toda engenharia de _hardware_para atender as necessidades do cliente ou do negócio.

Nesta Unidade de Aprendizagem, por meio da introdução aos sistemas embarcados, você aprenderá mais sobre as aplicações, os requisitos e os diferentes tipos e elementos que envolvem o planejamento de novos sistemas.

Bons estudos.

#### Ao final desta Unidade de Aprendizagem, você deve apresentar os seguintes aprendizados:

- Identificar as propriedades dos sistemas embarcados.
- Classificar os tipos de processos executados em sistemas embarcados.
- Descrever a fase de planejamento dos sistemas embarcados.

----
# 📘 Resumo de Estudo — Sistemas Embarcados e Microcontroladores

## 1️⃣ Sistemas Embarcados

Um **sistema embarcado** é um sistema computacional dedicado que executa **uma função específica dentro de um equipamento maior**.

### Características principais

- Função **específica**
    
- Normalmente usa **microcontroladores**
    
- **Baixo consumo de energia**
    
- Integrado ao hardware do equipamento
    
- Muitas vezes possui **restrições de tempo real**
    

### Exemplos

- Micro-ondas
    
- Máquina de lavar
    
- Sistemas automotivos (ABS, airbag)
    
- Equipamentos industriais
    
- IoT
    

---

# 2️⃣ Microcontroladores em Sistemas Embarcados

Um **microcontrolador** é um chip que contém:

- **CPU**
    
- **Memória**
    
- **Periféricos de entrada e saída**
    

Tudo **no mesmo circuito integrado**.

Isso permite:

✔ menor custo  
✔ menor consumo de energia  
✔ maior eficiência para tarefas específicas

---

# 3️⃣ Análise dos Modelos de Microcontroladores (Exemplo da tabela)

|Modelo|Clock|Barramento|Compatibilidade|
|---|---|---|---|
|PIC10|5 MHz|12|Atual|
|PIC12|5 MHz|14|98%|
|PIC12F|8 MHz|14|95%|
|PIC18|16 MHz|16|40%|

### Conceitos importantes

#### Clock

Define a **velocidade de execução do processador**.

✔ Quanto **maior o clock**, mais rápido o sistema.

Exemplo:

PIC10 → 5 MHz  
PIC12F → 8 MHz

➡ aumento de **60% de velocidade**

---

#### Barramento

É o **caminho por onde os dados trafegam dentro do sistema**.

✔ Quanto **maior o barramento**, mais dados podem ser transferidos ao mesmo tempo.

Exemplo:

12 bits → 14 bits  
➡ aumento de **16% de capacidade**

---

### Melhor escolha no estudo

O **PIC12F** foi considerado o melhor porque:

✔ 60% mais rápido  
✔ barramento maior  
✔ compatibilidade de 95%

Ou seja:

✔ melhora desempenho  
✔ pouca necessidade de reescrever código

---

# 4️⃣ Compatibilidade e Reescrita de Código

Quando troca o microcontrolador:

Pode acontecer:

- comandos diferentes
    
- registradores diferentes
    
- arquitetura diferente
    

Isso exige:

⚠ **reescrita de partes do software**

Por isso **compatibilidade é importante**.

---

# 5️⃣ PLC como Sistema Embarcado

PLC significa:

**Programmable Logic Controller**

ou

**Controlador Lógico Programável**

É muito usado na **automação industrial**.

---

## Estrutura básica de um PLC

Todo PLC possui:

1️⃣ **Fonte de alimentação**  
2️⃣ **CPU programável**  
3️⃣ **Entradas e saídas (I/O)**

---

# 6️⃣ Funcionamento do PLC

### Fluxo básico

1️⃣ **Sensor envia sinal (entrada)**  
2️⃣ PLC **processa a informação**  
3️⃣ PLC envia comando para **atuadores**

Exemplo da imagem:

Sensor → PLC → Bomba → Válvula → Controle de nível do tanque

---

# 7️⃣ Exemplos de aplicações com PLC

- Controle de **nível de tanque**
    
- Controle de **temperatura**
    
- Controle de **pressão**
    
- Controle de **bombas**
    
- Dosagem de materiais
    

Muito usado em:

🏭 indústria  
⚙️ automação  
🚰 controle de processos

---

# 8️⃣ Controle PID (importante para prova)

Na imagem aparece **controle PID do nível do tanque**.

PID significa:

- **P** → Proporcional
    
- **I** → Integral
    
- **D** → Derivativo
    

É um **algoritmo usado para controle automático**.

Exemplo:

Manter o nível da água constante no tanque.

---

# 📚 O QUE VOCÊ DEVE PESQUISAR MAIS (para prova)

Se você estudar esses tópicos abaixo, você domina a matéria.

---

## 1️⃣ Sistemas Embarcados

Pesquise:

- definição
    
- características
    
- exemplos
    
- diferença entre:
    
    - **microprocessador**
        
    - **microcontrolador**
        

---

## 2️⃣ Arquitetura de Microcontroladores

Estude:

- clock
    
- barramento
    
- memória
    
- registradores
    
- periféricos
    

---

## 3️⃣ Microcontroladores PIC

Pesquise:

- arquitetura PIC
    
- famílias PIC10, PIC12, PIC16, PIC18
    
- aplicações
    

---

## 4️⃣ Compatibilidade de Hardware

Entenda:

- portabilidade de código
    
- reescrita de firmware
    
- compatibilidade entre microcontroladores
    

---

## 5️⃣ PLC

Pesquise:

- o que é PLC
    
- estrutura
    
- entradas e saídas
    
- aplicações industriais
    
- linguagens de programação de PLC
    

---

## 6️⃣ Controle PID

Muito comum cair em prova.

Estude:

- conceito de controle PID
    
- para que serve
    
- aplicações
    

---

# 🎯 Dica de Professor (o que MAIS cai em prova)

Normalmente cobram:

✔ definição de **sistema embarcado**  
✔ diferença **microprocessador vs microcontrolador**  
✔ função do **clock**  
✔ função do **barramento**  
✔ estrutura do **PLC**  
✔ conceito de **controle PID**