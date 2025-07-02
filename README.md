![1](https://github.com/user-attachments/assets/e871f92f-750f-4c67-a67f-f7a7fd400629)

![2](https://github.com/user-attachments/assets/50252ccc-a0c5-4de2-8585-deb60630dddc)  ![3](https://github.com/user-attachments/assets/268493a9-4193-48ae-a45f-2d9b93c70266)
![4](https://github.com/user-attachments/assets/52bf96ae-4846-4978-aa6f-85237ff5d36b)







## 🧠 Introdução

### Por que aprender Estrutura de Dados?

Se você quer aprender a programar de verdade, precisa ir além de "fazer funcionar". Precisa entender *como* o seu programa funciona por dentro. Estruturas de dados são o coração disso. Elas definem como as informações são armazenadas, acessadas e manipuladas.

Imagine que você vai mudar de casa. Não basta jogar tudo no caminhão de qualquer jeito. É preciso organizar: roupas em malas, pratos em caixas acolchoadas, documentos em pastas. Em programação é igual. Estruturas de dados te ajudam a organizar a bagunça e tornar tudo mais rápido, eficiente e limpo.

Ao dominar estruturas de dados, você vai:

* Resolver problemas com mais elegância
* Escrever código mais rápido e eficiente
* Entender melhor os algoritmos
* Estar preparado para entrevistas de emprego em tecnologia

### Como usar este eBook

Este eBook foi criado com um objetivo: **te ensinar estrutura de dados de forma simples, direta e sem enrolação**.

Formato:

* Capítulos curtos e objetivos
* Linguagem informal e com analogias do cotidiano
* Exemplos práticos e comentados
* Desafios simples para exercitar

Siga a ordem dos capítulos, reflita sobre os exemplos, e tente imaginar situações do seu dia a dia onde aquilo faria sentido. A cada tópico, pense: *"Onde eu já vi isso acontecer na vida real?"*

Vamos nessa?

---

## 🧩 Parte 1 — Fundamentos Essenciais

### O que são Estruturas de Dados, afinal?

Estruturas de dados são formas de **organizar, armazenar e acessar informações** de maneira eficiente dentro de um programa.

Na prática, é como organizar a vida:

* Uma **playlist** é uma lista de músicas (Array)
* Sua **lista de tarefas** tem ordem de prioridade (Fila ou Pilha)
* Um **armário** tem compartimentos para cada tipo de objeto (Hash Table)

Ou seja, cada tipo de estrutura tem um formato diferente que serve para resolver um tipo de problema.

### Pensando como um programador

Um programador pensa em **como representar um problema com estruturas e lógica**. Antes de codar, ele imagina:

* Que tipo de dado vou usar?
* Com que frequência vou acessar ou modificar esse dado?
* Preciso de ordem? Rápida busca? Evitar repetidos?

Por exemplo: para armazenar os nomes dos clientes em uma loja virtual, você pode usar uma lista. Mas se quiser buscar rapidamente um cliente pelo e-mail, talvez um dicionário seja melhor.

### Memória e performance: como o computador pensa

Seu computador é rápido, mas **não é mágico**. Cada vez que você acessa, busca ou muda um dado, ele faz operações na memória. Algumas estruturas facilitam isso, outras dificultam.

Pense assim: você vai viajar. Pode colocar tudo em uma mala desorganizada (lento pra encontrar) ou em várias necessaires separadas (rápido e organizado). A segunda opção é melhor. É isso que uma boa estrutura de dados faz.

A escolha da estrutura **afeta diretamente o desempenho do seu programa**.

---

## 📦 Parte 2 — Estruturas Lineares no Dia a Dia

### Arrays e Listas: o armário de sapatos da programação

Arrays são como armários com divisórias fixas. Cada item tem um lugar específico, e você acessa pelo número da porta (o índice).

Exemplo: `array[0]` é o primeiro item, `array[1]` o segundo e assim por diante. Rápido para acessar, mas difícil de crescer ou encolher.

Listas (ou listas dinâmicas) são mais flexíveis — como uma sapateira extensível. Você pode adicionar ou remover sapatos facilmente, mas leva mais tempo para encontrar um específico.

**Use Arrays quando:**

* Você sabe exatamente quantos elementos terá.
* Precisa de acesso rápido por índice.

**Use Listas quando:**

* A quantidade de elementos muda bastante.
* Vai adicionar/remover itens com frequência.

---

### Pilhas (Stacks): pratos empilhados em um restaurante

Imagine uma pilha de pratos limpos. Você sempre coloca o novo prato em cima (push) e pega o último colocado (pop). Isso é o conceito de **LIFO (Last In, First Out)**.

Usamos pilhas para:

* Desfazer ações (Ctrl+Z)
* Controlar chamadas de funções
* Voltar páginas no navegador

**Funções principais:**

* `push(item)`: adiciona um item ao topo
* `pop()`: remove o item do topo
* `peek()`: olha o topo sem remover

---

### Filas (Queues): a fila do banco, sem jeitinho brasileiro

A fila é justa: quem chega primeiro, sai primeiro. Isso é **FIFO (First In, First Out)**.

Você adiciona no fim da fila (`enqueue`) e remove do início (`dequeue`).

Usamos filas para:

* Processar tarefas em ordem
* Atender requisições em sistemas
* Controlar impressão de documentos

**Funções principais:**

* `enqueue(item)`: adiciona no fim da fila
* `dequeue()`: remove o primeiro
* `peek()`: olha o primeiro sem remover

---

### Listas Ligadas: vagões de trem conectados

Diferente dos arrays, onde tudo está lado a lado na memória, nas **listas ligadas** cada elemento aponta para o próximo.

Imagine uma sequência de vagões onde cada um tem um acoplamento pro próximo.

**Vantagens:**

* Cresce facilmente
* Remoção e inserção mais eficientes em posições intermediárias

**Desvantagens:**

* Mais difícil de percorrer rapidamente
* Gasta mais memória (por causa dos ponteiros)

**Tipos:**

* Lista simplesmente ligada
* Lista duplamente ligada
* Lista circular

---

## 🧭 Parte 3 — Organizando e Localizando com Inteligência

### Dicionários e Hash Tables: o mapa de contatos do seu celular

Imagine procurar um contato no celular: você digita o nome e já encontra o número. Isso é uma operação com **chave-valor** — e é exatamente como funcionam os dicionários.

Em programação, dicionários (ou mapas/hash tables) armazenam dados usando uma **chave única** para acessar rapidamente um valor associado.

Exemplo:

```python
dicionario = {"lucas": "9999-1234", "ana": "9888-0000"}
print(dicionario["ana"])  # saída: 9888-0000
```

**Vantagens:**

* Busca muito rápida
* Ideal para consultas por identificadores únicos

**Desvantagens:**

* Consome mais memória
* Não tem ordem garantida (em alguns casos)

---

### Conjuntos (Sets): o que você já tem na coleção

Sets são como coleções que **não aceitam itens duplicados**. Imagine colecionar figurinhas e garantir que nenhuma repetida vá para o álbum.

Muito usado quando precisamos:

* Remover duplicatas
* Fazer operações de comparação entre grupos (união, interseção, diferença)

Exemplo:

```python
conjunto = {"banana", "maçã", "banana"}
print(conjunto)  # saída: {"banana", "maçã"}
```

---

## 🌳 Parte 4 — Estruturas Não Lineares

### Árvores (Trees): sua árvore genealógica ou decisões do dia a dia

Árvores são estruturas em formato hierárquico. Pense em uma árvore genealógica ou em um menu de decisões.

Cada **nó** pode ter vários **filhos**, mas apenas **um pai** (exceto a raiz).

Usos comuns:

* Representar hierarquias (como categorias em sites)
* Árvores de decisão (ex: jogos)
* Estruturas de busca (como a Binary Search Tree — BST)

---

### Grafos (Graphs): como o Google Maps conecta os caminhos

Grafos são conjuntos de **nós** (ou vértices) conectados por **arestas**. Eles representam relacionamentos complexos, como:

* Mapa de ruas
* Redes sociais
* Ligações entre aeroportos

Existem grafos direcionados (com sentido) e não direcionados (conexões livres). E ainda, podem ser ponderados (com custo) ou não.

---

## 🎮 Parte 5 — Aplicações Práticas e Próximos Passos

### Qual estrutura usar?

| Situação                          | Estrutura recomendada |
| --------------------------------- | --------------------- |
| Lista de tarefas                  | Lista, Pilha ou Fila  |
| Agenda de contatos                | Dicionário            |
| Controle de histórico (navegador) | Pilha                 |
| Fila de impressão                 | Fila                  |
| Sistema de categorias             | Árvore                |
| Rotas de mapa                     | Grafo                 |

---

### Mini projetos para treinar o que aprendeu

* **Simulador de fila de supermercado** (com `Queue`)
* **Agenda de contatos com busca por nome** (com `Dict`)
* **Navegador com botão “desfazer/refazer”** (com `Stack`)
* **Organizador de tarefas com prioridades** (com árvore ou heap)

---

### Erros comuns que iniciantes cometem com estruturas de dados

* Escolher a estrutura errada para o problema
* Tentar reinventar estruturas já prontas
* Usar listas para tudo (mesmo quando ineficiente)
* Não considerar a performance

---

### Próximos passos: como continuar evoluindo

* Estude algoritmos clássicos
* Participe de desafios de programação (Ex: HackerRank, LeetCode)
* Leia códigos open source
* Pratique resolvendo problemas reais

---

## Exemplos Praticos - Codigo Python

---

## 🧩 Parte 1 — Fundamentos Essenciais

### O que são Estruturas de Dados, afinal?

Estruturas de dados são formas de **organizar, armazenar e acessar informações** de maneira eficiente dentro de um programa.

Na prática, é como organizar a vida:

* Uma **playlist** é uma lista de músicas (Array)
* Sua **lista de tarefas** tem ordem de prioridade (Fila ou Pilha)
* Um **armário** tem compartimentos para cada tipo de objeto (Hash Table)

Ou seja, cada tipo de estrutura tem um formato diferente que serve para resolver um tipo de problema.

---

## 📦 Parte 2 — Estruturas Lineares no Dia a Dia

### Arrays e Listas

```python
# Exemplo de Array (lista em Python)
nomes = ["Ana", "Bruno", "Carlos"]
print(nomes[0])  # Ana
nomes.append("Daniel")
print(nomes)
```

### Pilhas (Stacks)

```python
# Exemplo de Pilha usando lista
pilha = []
pilha.append("prato1")
pilha.append("prato2")
pilha.append("prato3")
print(pilha.pop())  # prato3
print(pilha)        # ['prato1', 'prato2']
```

### Filas (Queues)

```python
# Exemplo de Fila com deque
from collections import deque
fila = deque()
fila.append("cliente1")
fila.append("cliente2")
print(fila.popleft())  # cliente1
print(fila)            # deque(['cliente2'])
```

### Listas Ligadas

```python
# Exemplo básico de Lista Ligada
class No:
    def __init__(self, dado):
        self.dado = dado
        self.proximo = None

no1 = No("A")
no2 = No("B")
no3 = No("C")
no1.proximo = no2
no2.proximo = no3

# Percorrer lista
atual = no1
while atual:
    print(atual.dado)
    atual = atual.proximo
```

---

## 🧭 Parte 3 — Organizando e Localizando com Inteligência

### Dicionários (Hash Tables)

```python
# Exemplo de Dicionário
contatos = {"Lucas": "9999-1234", "Ana": "9888-0000"}
print(contatos["Ana"])
contatos["João"] = "9777-3333"
print(contatos)
```

### Conjuntos (Sets)

```python
# Exemplo de Set
frutas = {"maçã", "banana", "maçã"}
print(frutas)  # {'maçã', 'banana'}
frutas.add("laranja")
print(frutas)
```

---

## 🌳 Parte 4 — Estruturas Não Lineares

### Árvores (árvore binária simples)

```python
class No:
    def __init__(self, valor):
        self.valor = valor
        self.esq = None
        self.dir = None

raiz = No(10)
raiz.esq = No(5)
raiz.dir = No(15)

# Percurso em ordem
def em_ordem(no):
    if no:
        em_ordem(no.esq)
        print(no.valor)
        em_ordem(no.dir)

em_ordem(raiz)
```

### Grafos (representação com dicionário)

```python
# Grafo simples não direcionado
grafo = {
    "A": ["B", "C"],
    "B": ["A", "D"],
    "C": ["A", "D"],
    "D": ["B", "C"]
}

# Percorrer vizinhos de A
print("Vizinhos de A:", grafo["A"])
```

---

## 🎮 Parte 5 — Aplicações Práticas e Mini Projetos

```python
# Simulador de fila de supermercado
from collections import deque
fila = deque()
fila.append("Cliente 1")
fila.append("Cliente 2")
print("Atendendo:", fila.popleft())

# Agenda com busca
agenda = {"Lucas": "1111-2222", "Maria": "3333-4444"}
nome = "Maria"
if nome in agenda:
    print("Número:", agenda[nome])

# Navegador com botão de desfazer
historico = []
historico.append("Página 1")
historico.append("Página 2")
print("Desfazer:", historico.pop())

# Organizador de tarefas com árvore (representação simples)
tarefas = {
    "Trabalho": ["Relatório", "Apresentação"],
    "Casa": ["Lavar roupa", "Limpar"]
}
print("Tarefas do Trabalho:", tarefas["Trabalho"])
```
---

Obrigado por ler! 🚀

**Autor: Lucas Lima**
