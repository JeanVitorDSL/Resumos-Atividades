
---

Microprocessadores são componentes digitais capazes de executar diversas funções e têm diferentes quantidades de pinos para conectá-los a outros componentes tão necessários quanto eles: memórias, sensores, atuadores, entre outros. Um microcontrolador, por sua vez, possui um microprocessador acoplado, bem como alguns desses dispositivos complementares integrados a ele. É um meio de reduzir a complexidade de desenvolvimento, mesmo que com isso a capacidade de processamento não seja tão elevada. Esses dispositivos foram utilizados em um primeiro momento em indústrias para automação de processos, mas à medida que o custo e o tamanho foram sendo reduzidos, enquanto a capacidade de processamento foi ampliada, diversas aplicações surgiram. Hoje grande parte dos dispositivos eletrônicos tem algum tipo de processador embutido.

Nesta Unidade de Aprendizagem, você verá com maiores detalhes de que forma esses dois dispositivos são programados e como o desenvolvimento tecnológico e as necessidades fizeram com que eles chegassem até as pessoas. Também perceberá que a quantidade de modelos existentes é enorme. E como forma de facilitar a comercialização e permitir que os programadores selecionem adequadamente um modelo que atenda as suas necessidades, esses dispositivos costumam ser divididos em famílias, algumas delas de grande relevância para a história dos processadores. Por fim, você conhecerá como e em que tipo de equipamentos os microprocessadores e os microcontroladores costumam ser utilizados.

Bons estudos.

#### Ao final desta Unidade de Aprendizagem, você deve apresentar os seguintes aprendizados:

- Caracterizar microcontroladores e microprocessadores.
- Identificar famílias de microcontroladores.
- Analisar aplicações de microcontroladores

---

# Microprocessadores e Microcontroladores — Resumo

## 1. Microprocessador

Um **microprocessador** é um circuito integrado que contém **apenas a CPU**.

Para funcionar, ele precisa de componentes externos.

### Componentes externos necessários

- memória RAM
    
- memória de armazenamento
    
- controladores de entrada e saída
    
- chipset
    

### Aplicações

- computadores pessoais
    
- servidores
    
- notebooks
    

### Características

- **alto poder de processamento**
    
- maior flexibilidade
    
- depende de vários componentes externos
    

---

# Microcontrolador

Um **microcontrolador** é um circuito integrado que reúne **vários componentes dentro do mesmo chip**.

### Componentes integrados

- CPU
    
- memória RAM
    
- memória Flash
    
- portas de entrada e saída (I/O)
    
- temporizadores
    
- periféricos
    

### Características

- pode funcionar **quase sozinho**
    
- **baixo consumo de energia**
    
- menor custo
    
- ideal para **sistemas embarcados**
    

### Exemplos

- Arduino (ATmega)
    
- PIC
    
- STM32
    

---

# Diferença entre Microprocessador e Microcontrolador

|Característica|Microprocessador|Microcontrolador|
|---|---|---|
|Componentes integrados|apenas CPU|CPU + memória + periféricos|
|Uso|computadores|sistemas embarcados|
|Consumo de energia|maior|menor|
|Necessidade de hardware externo|alta|baixa|

---

# Eletrônica Digital

A **eletrônica digital** trabalha com sinais discretos representados por:

- **0**
    
- **1**
    

Esses valores representam **estados lógicos**.

---

# Principais vantagens da eletrônica digital

### Reprogramação

Um mesmo dispositivo pode executar **diferentes funções apenas alterando o software**.

Isso permitiu o surgimento de:

- microcontroladores
    
- computadores
    
- dispositivos inteligentes
    

---

### Outras vantagens

- maior confiabilidade
    
- facilidade de processamento de dados
    
- integração com sistemas computacionais
    
- automação de processos
    

---

# Programação de Microcontroladores

Para programar um microcontrolador é necessário:

1️⃣ escrever o código  
2️⃣ compilar o código  
3️⃣ gravar o programa no microcontrolador

---

## Compilação

A **compilação** é o processo de traduzir o código de uma linguagem de alto nível para uma linguagem que a máquina compreenda.

Exemplo:

C / Assembly → Código de máquina (binário)

---

# Tipos de Erros em Programação

## Erro de Sintaxe

Ocorre quando:

- comandos estão escritos incorretamente
    
- compilador não reconhece a instrução
    

Esse erro **é detectado na compilação**.

---

## Erro Lógico

Ocorre quando:

- o programa executa
    
- mas o resultado é **incorreto**
    

Exemplo:

- acessar **endereços de memória errados**
    
- operações matemáticas erradas
    

Esse erro **não é detectado pelo compilador**.

---

# Instruções de Processador

Cada processador possui seu próprio **conjunto de instruções (Instruction Set)**.

Essas instruções são representadas por **mnemônicos**.

Exemplo:

|Mnemônico|Função|
|---|---|
|MOV|mover dados|
|ADD|somar|
|SUB|subtrair|
|LOAD|carregar valor|
|STORE|armazenar valor|

---

# Registrador Acumulador

O **acumulador (ACC)** é um registrador usado para **realizar operações aritméticas e lógicas**.

Ele armazena **resultados temporários** das operações.

---

## Exemplo

Memória:

M1 = 5  
M2 = 8

Operação:

LOAD M1  
SUB M2

Resultado:

ACC = 5 - 8  
ACC = -3

---

# Troca de Valores na Memória

Para trocar valores entre dois endereços de memória é necessário usar uma **posição temporária**.

### Exemplo

MOV 3,1  
MOV 1,2  
MOV 2,3

Resultado:

- endereço 1 recebe valor do endereço 2
    
- endereço 2 recebe valor do endereço 1
    

---

# Conceitos Importantes para Prova

### Microcontrolador

- possui **CPU + memória + periféricos no mesmo chip**
    

### Microprocessador

- possui **apenas CPU**
    

### Compilação

- tradução de código para linguagem de máquina
    

### Tipos de erro

- sintaxe
    
- lógico
    

### Acumulador

- registrador que armazena resultados temporários
    

### Instruções

- representadas por **mnemônicos**
    

---

# O que mais costuma cair em prova

Estude principalmente:

1️⃣ diferença **microprocessador vs microcontrolador**  
2️⃣ vantagens da **eletrônica digital**  
3️⃣ **processo de compilação**  
4️⃣ **erros de sintaxe vs erros lógicos**  
5️⃣ **função do acumulador**  
6️⃣ **instruções básicas (MOV, ADD, SUB)**

---

