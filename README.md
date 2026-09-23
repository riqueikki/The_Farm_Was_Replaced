# 🌾 The Farmer Was Replaced — Guia de Programação

Documentação educacional e coleção de exemplos desenvolvidos durante minha jornada com o jogo **The Farmer Was Replaced**.

O objetivo deste projeto é utilizar o jogo como uma ferramenta prática para aprender e ensinar conceitos básicos de **lógica de programação e Python**, utilizando o drone como elemento central das atividades.

> **Aprender programação fazendo.**

---

## 🎮 Sobre o jogo

**The Farmer Was Replaced** é um jogo de automação no qual o jogador programa um drone para cuidar de uma fazenda.

Em vez de controlar o personagem manualmente, criamos instruções para que o drone:

* 🌱 plante;
* 🌾 colha;
* 🚜 prepare o solo;
* 🧭 se movimente;
* 👀 obtenha informações do ambiente;
* 🔄 repita tarefas;
* 📦 utilize variáveis;
* 🧠 tome decisões com condições;
* ⚙️ utilize funções;
* 📋 trabalhe com listas.

O jogo utiliza uma linguagem inspirada em Python, permitindo trabalhar conceitos de programação de forma visual e prática.

---

## 🎯 Objetivo desta documentação

Esta documentação foi criada para organizar os códigos desenvolvidos durante minha progressão no jogo e, ao mesmo tempo, transformar essa experiência em um material de apoio para estudantes.

A proposta é apresentar os conceitos de programação **passo a passo**, começando por comandos simples e avançando gradualmente para programas mais completos.

O foco é compreender:

```text
Comando
   ↓
Repetição
   ↓
Condição
   ↓
Movimentação
   ↓
Plantio
   ↓
Sentidos
   ↓
Variáveis
   ↓
Funções
   ↓
Listas
   ↓
Automação
```

---

## 🧑‍🏫 Público-alvo

Este material pode ser utilizado como apoio introdutório para estudantes interessados em:

* lógica de programação;
* pensamento computacional;
* programação básica;
* automação;
* Python;
* desenvolvimento de algoritmos.

Os exemplos também podem ser adaptados para atividades com estudantes do **Ensino Fundamental**, especialmente a partir dos anos iniciais, utilizando uma linguagem mais simples e atividades práticas.

---

# 📚 Conteúdos

## 01 — Loops

Primeiro aprendemos a fazer o drone repetir uma tarefa.

### `while True`

O `while True` cria um ciclo contínuo:

```python
while True:
    harvest()
```

O drone continuará executando o comando enquanto o programa estiver funcionando.

📖 [Aprender sobre while](01-loop/while_true.md)

---

# 02 — Colheita

Depois aprendemos a verificar se existe alguma planta pronta antes de colher.

### `can_harvest()`

```python
if can_harvest():
    harvest()
```

O `can_harvest()` verifica se a planta está pronta para ser colhida.

### `harvest()`

O `harvest()` realiza a colheita.

📖 [Can Harvest e Harvest](01-loop/comandoharvest.md)

---

# 03 — Movimentação

Depois ensinamos o drone a se movimentar pela fazenda.

```python
move(North)
move(East)
move(South)
move(West)
```

Esses comandos permitem criar caminhos e percorrer diferentes áreas da fazenda.

📖 [Move](03-movimentacao/move.md)

📖 [Direções](03-movimentacao/directions.md)

---

# 04 — Plantio

Depois do movimento e da colheita, podemos ensinar o drone a plantar.

Exemplo:

```python
plant(Entities.Bush)
```

Também podemos trabalhar com diferentes entidades, como:

```python
Entities.Bush
Entities.Carrot
Entities.Grass
```

⚠️ **Observação:** Grass cresce naturalmente em `Grassland`. Portanto, `Entities.Grass` não deve ser tratado da mesma maneira que Bush e Carrot usando `plant()`.

📖 [Plant](04-plantio/plant.md)

📖 [Bush](04-plantio/bush.md)

📖 [Carrot](04-plantio/carrot.md)

📖 [Grass](04-plantio/grass.md)

---

# 05 — Sentidos

Os sentidos permitem que o drone obtenha informações sobre o ambiente.

Por exemplo:

```python
get_pos_x()
```

informa a posição X.

```python
get_pos_y()
```

informa a posição Y.

Também podemos verificar o tipo de terreno:

```python
get_ground_type()
```

Essas informações permitem que o programa tome decisões.

📖 [get_pos_x()](05-sentidos/get_pos_x.md)

📖 [get_pos_y()](05-sentidos/get_pos_y.md)

📖 [get_ground_type()](05-sentidos/get_ground_type.md)

📖 [get_entity_type()](05-sentidos/get_entity_type.md)

---

# 06 — Condições e Operadores

Agora podemos fazer o drone **tomar decisões**.

Exemplo:

```python
if get_pos_x() == 2:
    move(East)
```

O programa verifica uma condição antes de executar o comando.

Também aprendemos operadores como:

```text
==    igual
!=    diferente
>     maior
<     menor
>=    maior ou igual
<=    menor ou igual
```

📖 [if](06-condicoes/if.md)

📖 [else](06-condicoes/else.md)

📖 [Operadores](06-condicoes/operadores.md)

---

# 07 — Variáveis

Uma variável permite guardar uma informação.

Por exemplo:

```python
planta = Entities.Carrot
```

Depois podemos utilizar essa informação:

```python
plant(planta)
```

Isso permite reutilizar o mesmo código com diferentes valores.

📖 [Variáveis](07-variaveis/variaveis.md)

---

# 08 — Funções

Funções são blocos de código utilizados para realizar tarefas.

No jogo encontramos funções prontas, como:

```python
harvest()
plant()
move()
can_harvest()
```

Também podemos aprender a criar nossas próprias funções utilizando `def`.

📖 [Funções](08-funcoes/funcoes.md)

---

# 09 — Listas

Uma lista permite guardar várias informações juntas.

Exemplo:

```python
plantas = [
    Entities.Bush,
    Entities.Carrot
]
```

Podemos então trabalhar com vários valores utilizando uma única estrutura.

📖 [Listas](09-listas/listas.md)

---

# 10 — Expansão da Fazenda

À medida que a fazenda cresce, nossos programas também precisam evoluir.

### Fazenda 3×3

```text
3 colunas × 3 linhas
= 9 espaços
```

### Fazenda 4×4

```text
4 colunas × 4 linhas
= 16 espaços
```

### Fazenda 5×5

```text
5 colunas × 5 linhas
= 25 espaços
```

O objetivo é substituir códigos repetitivos por soluções mais inteligentes e reutilizáveis.

📖 [Fazenda 4×4](10-expansao/fazenda_4x4.md)

📖 [Fazenda 5×5](10-expansao/fazenda_5x5.md)

---

# 🧪 Exemplos

Os exemplos práticos ficam na pasta `exemplos/`.

```text
exemplos/
├── bush_3x3.py
├── bush_grass_carrot_4x4.py
└── bush_grass_carrot_5x5.py
```

A ideia é que cada arquivo represente uma etapa da aprendizagem.

---

# 🧠 Conceitos trabalhados

| Conceito    | O que aprendemos               |
| ----------- | ------------------------------ |
| `while`     | Repetição contínua             |
| `for`       | Repetição controlada           |
| `if`        | Tomada de decisão              |
| `else`      | Alternativa                    |
| `==`        | Comparação                     |
| Variáveis   | Armazenamento de informações   |
| Funções     | Organização de tarefas         |
| Listas      | Organização de vários valores  |
| Sentidos    | Obtenção de informações        |
| Coordenadas | Localização do drone           |
| Automação   | Execução automática de tarefas |

---

# 🌱 Projeto educacional

Este projeto também pode ser utilizado para trabalhar **Pensamento Computacional**, especialmente:

* decomposição de problemas;
* reconhecimento de padrões;
* criação de algoritmos;
* abstração;
* automação;
* resolução de problemas.

A fazenda funciona como um ambiente de experimentação: o estudante escreve o código, executa, observa o resultado e modifica o programa quando algo não funciona.

---

# 📺 Conteúdo em vídeo

Este projeto acompanha uma série de conteúdos produzidos para o canal **Professor Henrique Brandão**, utilizando *The Farmer Was Replaced* como recurso para apresentar programação de maneira prática.

Os vídeos demonstram a construção dos códigos e a evolução da fazenda passo a passo.

---

## 📌 Observação

Este repositório possui finalidade **educacional**.

Os códigos são desenvolvidos para estudar programação e automação dentro do ambiente do jogo.

Para informações completas e atualizadas sobre as funções e mecânicas do jogo, consulte também a documentação da comunidade do *The Farmer Was Replaced*.

---

## 👨‍🏫 Autor

**Professor Henrique Brandão**

Projeto voltado para:

**Educação • Tecnologia Educacional • Pensamento Computacional • Programação • Gamificação**

---

> 🌾 **Plante código. Colha conhecimento.**
