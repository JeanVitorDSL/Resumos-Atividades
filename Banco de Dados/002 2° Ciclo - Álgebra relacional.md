
---

Claro, aqui está o mesmo resumo de estudo, formatado como um texto contínuo, sem marcações Markdown.

Resumo de Estudo: Álgebra Relacional e SQL

1. O que é Álgebra Relacional?
    

A Álgebra Relacional é uma linguagem de consulta procedural e formal para o modelo de banco de dados relacional.

Ela é formal porque possui uma base matemática sólida, vinda da teoria dos conjuntos. É procedural porque você especifica quais operadores usar e em qual sequência para obter o resultado desejado. Em outras palavras, você descreve o "como fazer" passo a passo.

Ela serve como o fundamento teórico sobre o qual linguagens de consulta mais amigáveis, como o SQL, foram construídas. Entender Álgebra Relacional é entender como o banco de dados "pensa" ao executar uma consulta.

A diferença crucial é: Álgebra Relacional (Procedural): "Vá até a tabela Alunos, filtre pelas linhas onde Cidade = 'Varginha' e depois me mostre apenas as colunas Nome e Idade." SQL (Declarativa): "Eu quero o Nome e a Idade dos alunos que moram em 'Varginha'." (Você declara o que quer, não como obter).

2. Conceitos Fundamentais
    

Relação: O termo formal para uma tabela. Tupla: O termo formal para uma linha ou registro. Atributo: O termo formal para uma coluna. Semântica de Conjunto: Relações na álgebra relacional são conjuntos de tuplas. Isso implica duas regras importantes: primeiro, não há tuplas duplicadas; segundo, a ordem das tuplas não importa.

3. Operadores Fundamentais
    

Aqui detalhamos os operadores e adicionamos outros essenciais.

3.1. Operadores Unários (Operam em uma única relação)

a) Seleção (Selection) - σ Propósito: Filtrar tuplas (linhas) com base em uma condição (predicado). É o "filtro horizontal". Sintaxe Álgebra: σ_{predicado}(Relação) Análogo SQL: WHERE Exemplo: Selecionar todos os alunos com mais de 20 anos da tabela ALUNOS. Álgebra: σ_{Idade > 20}(ALUNOS) SQL: SELECT * FROM ALUNOS WHERE Idade > 20;

b) Projeção (Projection) - π Propósito: Selecionar atributos (colunas) específicos de uma relação. É o "filtro vertical". Sintaxe Álgebra: π_{lista_de_atributos}(Relação) Análogo SQL: SELECT [DISTINCT] Observação Crucial: Como a álgebra relacional trabalha com conjuntos, a projeção elimina automaticamente as tuplas duplicadas que possam surgir. Por isso, a tradução mais fiel para SQL usa DISTINCT. Exemplo: Listar apenas o nome e a cidade de todos os alunos. Álgebra: π_{Nome, Cidade}(ALUNOS) SQL: SELECT DISTINCT Nome, Cidade FROM ALUNOS;

c) Renomeação (Rename) - ρ Propósito: Mudar o nome de uma relação ou de seus atributos. Útil para evitar ambiguidades, especialmente em junções. Sintaxe Álgebra: ρ_{NovoNome}(Relação) ou ρ_{NovoNome(Atrib1, Atrib2, ...)}(Relação) Análogo SQL: AS Exemplo: Criar uma cópia da relação ALUNOS com o nome ESTUDANTES. Álgebra: ρ_{ESTUDANTES}(ALUNOS) SQL (em uma cláusula FROM): SELECT * FROM ALUNOS AS ESTUDANTES;

3.2. Operadores Binários (Operam em duas relações)

Estes operadores, em sua maioria, exigem que as relações sejam compatíveis em união, ou seja, devem ter o mesmo número de atributos e os domínios (tipos de dados) correspondentes devem ser compatíveis.

a) União (Union) - ∪ Propósito: Combina todas as tuplas de duas relações, eliminando as duplicadas. Sintaxe Álgebra: Relação1 ∪ Relação2 Análogo SQL: UNION Exemplo: Unir uma tabela de ALUNOS_2024 com ALUNOS_2025. Álgebra: ALUNOS_2024 ∪ ALUNOS_2025 SQL: SELECT * FROM ALUNOS_2024 UNION SELECT * FROM ALUNOS_2025;

b) Interseção (Intersection) - ∩ Propósito: Retorna apenas as tuplas que existem em ambas as relações. Sintaxe Álgebra: Relação1 ∩ Relação2 Análogo SQL: INTERSECT Exemplo: Encontrar alunos que estão matriculados tanto no curso de 'Inglês' quanto no de 'Espanhol'. Álgebra: π_{ID_Aluno}(σ_{Curso='Inglês'}(MATRICULAS)) ∩ π_{ID_Aluno}(σ_{Curso='Espanhol'}(MATRICULAS)) SQL: SELECT ID_Aluno FROM MATRICULAS WHERE Curso = 'Inglês' INTERSECT SELECT ID_Aluno FROM MATRICULAS WHERE Curso = 'Espanhol';

c) Diferença (Set Difference) - − Propósito: Retorna as tuplas que estão na primeira relação, mas não estão na segunda. Sintaxe Álgebra: Relação1 - Relação2 Análogo SQL: EXCEPT (padrão SQL) ou MINUS (Oracle). Exemplo: Encontrar alunos que cursaram 'Inglês', mas não cursaram 'Espanhol'. Álgebra: π_{ID_Aluno}(σ_{Curso='Inglês'}(MATRICULAS)) - π_{ID_Aluno}(σ_{Curso='Espanhol'}(MATRICULAS)) SQL: SELECT ID_Aluno FROM MATRICULAS WHERE Curso = 'Inglês' EXCEPT SELECT ID_Aluno FROM MATRICULAS WHERE Curso = 'Espanhol';

d) Produto Cartesiano (Cartesian Product) - × Propósito: Combina cada tupla da primeira relação com cada tupla da segunda. O resultado é uma nova relação com todos os atributos de ambas. Cuidado: Se a Relação A tem n tuplas e a Relação B tem m tuplas, o resultado terá n * m tuplas. Isso pode gerar tabelas gigantescas e raramente é usado de forma isolada. É a base para a operação de Junção. Sintaxe Álgebra: Relação1 × Relação2 Análogo SQL: CROSS JOIN ou a sintaxe legada FROM Tabela1, Tabela2 Exemplo: Combinar cada aluno com cada curso existente. Álgebra: ALUNOS × CURSOS SQL: SELECT * FROM ALUNOS CROSS JOIN CURSOS;

4. Operador Derivado Essencial: A Junção (Join) - ⋈
    

A Junção é a operação mais importante para consultar bancos de dados relacionais. Ela combina o Produto Cartesiano com uma Seleção para criar relacionamentos significativos entre tabelas.

Propósito: Combinar tuplas de diferentes relações com base em uma condição de junção. Sintaxe Álgebra (Theta Join): Relação1 ⋈_{condição} Relação2. Isso é um atalho para: σ_{condição}(Relação1 × Relação2) Análogo SQL: JOIN ... ON Exemplo: Listar o nome de cada aluno e o nome do curso em que ele está matriculado, usando as tabelas ALUNOS(ID, Nome) e MATRICULAS(ID_Aluno, Nome_Curso). Álgebra: ALUNOS ⋈_{ALUNOS.ID = MATRICULAS.ID_Aluno} MATRICULAS SQL: SELECT ALUNOS.Nome, MATRICULAS.Nome_Curso FROM ALUNOS JOIN MATRICULAS ON ALUNOS.ID = MATRICULAS.ID_Aluno;

5. Resumo dos Operadores
    

Operador: Seleção. Símbolo: σ. Propósito: Filtra linhas (horizontal). Equivalente SQL: WHERE. Operador: Projeção. Símbolo: π. Propósito: Seleciona colunas (vertical). Equivalente SQL: SELECT DISTINCT. Operador: União. Símbolo: ∪. Propósito: Une duas tabelas (sem duplicatas). Equivalente SQL: UNION. Operador: Interseção. Símbolo: ∩. Propósito: Encontra linhas em comum. Equivalente SQL: INTERSECT. Operador: Diferença. Símbolo: −. Propósito: Encontra linhas exclusivas da 1ª tabela. Equivalente SQL: EXCEPT / MINUS. Operador: Produto Cartesiano. Símbolo: ×. Propósito: Combina tudo com tudo. Equivalente SQL: CROSS JOIN. Operador: Renomeação. Símbolo: ρ. Propósito: Altera nomes de tabelas/colunas. Equivalente SQL: AS. Operador: Junção. Símbolo: ⋈. Propósito: Combina tabelas por uma condição. Equivalente SQL: JOIN ... ON.