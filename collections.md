# Collections

As Collections em Java são estruturas que permitem armazenar, organizar e manipular dados de forma eficiente. Aqui está uma lista detalhada dos principais tipos de collections e seus métodos mais importantes, com exemplos de utilização:

## **1.** List 

Uma List é uma coleção ordenada que permite elementos duplicados.

*  *ArrayList*
    * Métodos principais: `add()`, `get()`, `remove()`, `size()`
    * Exemplo:
 ```java

List<String> arrayList = new ArrayList<>();
    arrayList.add("Elemento 1");
    arrayList.add("Elemento 2");
    System.out.println(arrayList.get(0)); // Saída: Elemento 1

```
* *LinkedList* 

    * Métodos principais: `add()`, `get()`, `remove()`, `size()`,  `addFirst()`, `addLast()`

    * Exemplo:
```java

LinkedList<String> linkedList = new LinkedList<>();
    linkedList.add("Elemento 1");
    linkedList.addFirst("Elemento 0");
    System.out.println(linkedList.get(0)); // Saída: Elemento 0
```
## **2.** Set
 Um Set é uma coleção que não permite elementos duplicados.

* *HashSet*

    * Métodos principais: `add()`, `remove()`, `contains()`, `size()`
    * Exemplo:

```java
Set<String> hashSet = new HashSet<>();
    hashSet.add("Elemento 1");
    hashSet.add("Elemento 2");
    System.out.println(hashSet.contains("Elemento 1")); // Saída: true
```

* *TreeSet*

    * Métodos principais: `add()`, `remove()`,` contains()`,` size()`, `first()`, `last()`
    * Exemplo:

```java
TreeSet<String> treeSet = new TreeSet<>();
    treeSet.add("Elemento 1");
    treeSet.add("Elemento 2");
    System.out.println(treeSet.first()); // Saída: Elemento 1
```

# **3.** Queue

Uma Queue é uma coleção usada para armazenar elementos antes de processá-los.

* *PriorityQueue*

    * Métodos principais: `add()`, `poll()`, `peek()`, `size()`
    * Exemplo:

```java

Queue<String> priorityQueue = new PriorityQueue<>();
    priorityQueue.add("Elemento 1");
    priorityQueue.add("Elemento 2");
    System.out.println(priorityQueue.poll()); // Saída: Elemento 1
```
## **4.** Map
Um Map é uma coleção que mapeia chaves para valores.

* *HashMap*

    * Métodos principais: `put()`, `get()`, `remove()`, `containsKey()`, `size()`
    * Exemplo:

```java
Map<String, String> hashMap = new HashMap<>();
    hashMap.put("chave1", "valor1");
    hashMap.put("chave2", "valor2");
    System.out.println(hashMap.get("chave1")); // Saída: valor1

```
* *TreeMap*

    * Métodos principais: `put()`, `get()`, `remove()`, `containsKey()`, `size()`,` firstKey()`, `lastKey()`
    * Exemplo:

```java

TreeMap<String, String> treeMap = new TreeMap<>();
    treeMap.put("chave1", "valor1");
    treeMap.put("chave2", "valor2");
    System.out.println(treeMap.firstKey()); // Saída: chave1
```
# Observação

 A escolha entre usar uma estrutura de dados baseada em árvore (Tree) ou hash (Hash), ou entre listas ligadas (Linked) e arrays (Array), depende do caso de uso específico e das características de desempenho que você precisa. Aqui estão algumas diretrizes para ajudar na decisão:

 ## Tree vs. Hash
**Tree (TreeSet, TreeMap)**
* Quando usar:

    * Ordenação: Quando você precisa que os elementos estejam      sempre ordenados.
    * Navegação: Quando você precisa navegar pelos elementos em uma ordem específica (por exemplo, encontrar o menor ou maior elemento).
    * Intervalos: Quando você precisa realizar operações de intervalo, como encontrar todos os elementos entre dois valores.
* Exemplo:

```java

TreeSet<Integer> treeSet = new TreeSet<>();
    treeSet.add(10);
    treeSet.add(5);
    treeSet.add(20);
    System.out.println(treeSet.first()); // Saída: 5
```
**Hash (HashSet, HashMap)**
* Quando usar:

    * Desempenho: Quando a velocidade de acesso e inserção é crucial. As operações de busca, inserção e remoção são geralmente O(1).
    * Unicidade: Quando você precisa garantir que não haja elementos duplicados (HashSet) ou chaves duplicadas (HashMap).
* Exemplo:

```java

HashSet<String> hashSet = new HashSet<>();
    hashSet.add("Elemento 1");
    hashSet.add("Elemento 2");
    System.out.println(hashSet.contains("Elemento 1")); // Saída: true
```

## Linked vs. Array
**Array (ArrayList)**
* Quando usar:

    * Acesso rápido: Quando você precisa de acesso rápido e aleatório aos elementos. O tempo de acesso é O(1).
    * Tamanho fixo: Quando o tamanho da coleção é conhecido e não muda frequentemente.
* Exemplo:

```java
ArrayList<String> arrayList = new ArrayList<>();
    arrayList.add("Elemento 1");
    arrayList.add("Elemento 2");
    System.out.println(arrayList.get(0)); // Saída: Elemento 1
```

**Linked (LinkedList)**
* Quando usar:

    * Inserções/remoções frequentes: Quando você precisa inserir ou remover elementos frequentemente, especialmente no início ou no meio da lista. O tempo de inserção/remoção é O(1) para essas operações.
    * Tamanho variável: Quando o tamanho da coleção muda frequentemente.

* Exemplo:
```java
LinkedList<String> linkedList = new LinkedList<>();
    linkedList.add("Elemento 1");
    linkedList.addFirst("Elemento 0");
    System.out.println(linkedList.get(0)); // Saída: Elemento 0
```
