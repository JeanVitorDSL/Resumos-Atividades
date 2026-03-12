
---
Conhecer o desenvolvimento de sistemas embarcados dá suporte ao estudante, não apenas para ser programador desses MCUs (Microcontroller Unit - Unidades de Microcontroladores), mas também para entender de forma sistêmica o processo mecânico que envolve as ligações entre _hardware_ e _software_. Há poucos anos, apenas linguagens de baixo nível possibilitavam a programação de MCU. Hoje, as aplicações de sistemas embarcados com microcomputadores podem ser desenvolvidas em liguagens mais modernas e amigáveis, inclusive com o uso de ambiente próprio.

Nesta Unidade de Aprendizagem, você irá aprender sobre as possibilidades de aplicações de sistemas embarcados que utilizam microcontroladores e verá como programá-los por meio de linguagens de alto nível, além das ligações por sensores analógicos digitais e atuadores.

Bons estudos.

#### Ao final desta Unidade de Aprendizagem, você deve apresentar os seguintes aprendizados:

- Explicar o uso da linguagem de programação de microcontroladores de alto nível.
- Demonstrar o funcionamento de sensores analógicos digitais em microcontroladores.
- Reconhecer os tipos de atuadores em sistemas embarcados com microcontroladores.
---

	

---
# Linguagem C e Programação em Microcontroladores — Resumo

## 1. Linguagens de Programação

As linguagens de programação podem ser classificadas pelo **nível de abstração**.

### Linguagens de Alto Nível

São linguagens **mais próximas da linguagem humana** e mais fáceis de utilizar.

#### Características

- sintaxe mais simples
    
- maior produtividade
    
- código mais fácil de entender
    
- **reduz tempo de desenvolvimento**
    
- reduz **custo de desenvolvimento**
    

#### Exemplos

- C
    
- C++
    
- Python
    
- Java
    

Essas linguagens precisam ser **compiladas ou interpretadas** para que o processador possa executá-las.

---

# Linguagem C em Sistemas Embarcados

A **linguagem C** é uma das mais utilizadas em:

- microcontroladores
    
- sistemas embarcados
    
- firmware
    
- dispositivos IoT
    

### Vantagens

- código eficiente
    
- controle de hardware
    
- portabilidade entre plataformas
    
- boa performance
    

---

# Estrutura de Programas em Arduino

Na programação de **Arduino**, baseada em **C/C++**, existem duas funções principais.

## Função `setup()`

Executada **uma única vez** quando o sistema inicia.

### Função

- inicializar hardware
    
- configurar pinos
    
- iniciar comunicação
    

Exemplo:

void setup() {  
  pinMode(13, OUTPUT);  
}

---

## Função `loop()`

Executa **continuamente enquanto o sistema estiver ligado**.

### Características

- execução infinita
    
- repete até o sistema ser desligado ou reiniciado
    

Exemplo:

void loop() {  
  digitalWrite(13, HIGH);  
  delay(1000);  
}

---

# Variáveis

Variáveis armazenam **valores utilizados no programa**.

Exemplo:

int a = 4;  
int b = 2;

Elas podem ser declaradas:

- fora das funções (globais)
    
- dentro das funções (locais)
    

---

# Estruturas Condicionais em C

As estruturas condicionais permitem **tomar decisões no programa**.

### Estrutura `if`

Exemplo:

if (a > 5) {  
   // executa ação  
}

---

## Operadores de comparação

|Operador|Significado|
|---|---|
|`==`|igual|
|`<`|menor|
|`>`|maior|
|`<=`|menor ou igual|
|`>=`|maior ou igual|
|`!=`|diferente|

⚠ **Erro comum**

if (a = 5)

Aqui ocorre **atribuição**, não comparação.

O correto seria:

if (a == 5)

---

# Execução de Código no Loop

No Arduino, o `loop()` executa continuamente.

Exemplo de lógica:

a = a + b;  
b = b + 1;

Se:

a = 4  
b = 2

Valores gerados:

|Iteração|a|b|
|---|---|---|
|1|6|3|
|2|9|4|
|3|13|5|
|4|18|6|

Valores exibidos:

6, 9, 13, 18

---

# Arduino e Módulos

Em sistemas embarcados com Arduino, vários componentes trabalham juntos.

### Elementos principais

1️⃣ **Microcontrolador**

Responsável por executar o programa.

Exemplo:

- ATmega328
    

---

2️⃣ **Módulos de interface**

Permitem comunicação com o mundo externo.

Exemplos:

- sensores
    
- displays LCD
    
- motores
    
- módulos WiFi
    
- relés
    

---

3️⃣ **Código-fonte**

Programa escrito pelo desenvolvedor que controla o funcionamento do sistema.

---

# IDE (Ambiente de Desenvolvimento)

A **IDE** é o software utilizado para:

- escrever código
    
- compilar
    
- enviar o programa ao microcontrolador
    

Exemplo:

- **Arduino IDE**
    

⚠ A IDE **não faz parte do sistema embarcado**, apenas do desenvolvimento.

---

# Conceitos Importantes para Prova

### Linguagens de alto nível

- facilitam programação
    
- reduzem tempo e custo
    

### Arduino

- usa **linguagem C/C++**
    

### Funções principais

- `setup()` → inicialização
    
- `loop()` → repetição contínua
    

### Estruturas condicionais

- `if`
    
- operadores de comparação
    

### Sistema embarcado com Arduino

- microcontrolador
    
- módulos de interface
    
- código-fonte
    

---

# O que mais costuma cair em prova

Estude principalmente:

1️⃣ função **setup()**  
2️⃣ função **loop()**  
3️⃣ erro **= vs ==** em condições  
4️⃣ execução passo a passo de código  
5️⃣ papel do **microcontrolador**  
6️⃣ relação **Arduino + módulos + código**

---