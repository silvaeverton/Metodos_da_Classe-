# Métodos da Classe `Math`

### A classe Math em Java oferece muitos métodos úteis para realizar operações matemáticas. Aqui está uma lista de alguns dos métodos mais comuns, com uma breve explicação e um exemplo simples para cada um:


***1.*** `Math.abs()`

**Descrição:** Retorna o valor absoluto de um número.

```java

int valor = -10;
int absoluto = Math.abs(valor); // absoluto será 10
```
***2.*** `Math.max()`

**Descrição:** Retorna o maior de dois valores.

```java

int a = 5;
int b = 10;
int maior = Math.max(a, b); // maior será 10
```

***3.*** `Math.min()`

**Descrição:** Retorna o menor de dois valores.

```java

int a = 5;
int b = 10;
int menor = Math.min(a, b); // menor será 5
```
***4.*** `Math.pow()`

**Descrição:** Retorna o valor de um número elevado à potência de outro número.

```java

double base = 2;
double expoente = 3;
double resultado = Math.pow(base, expoente); // resultado será 8.0
```

***5.*** `Math.sqrt()`
**Descrição:** Retorna a raiz quadrada de um número.

```java

double numero = 16;
double raiz = Math.sqrt(numero); // raiz será 4.0
```
***6.*** `Math.random()`
**Descrição:** Retorna um valor aleatório entre 0.0 (inclusive) e 1.0 (exclusivo).

```java

double aleatorio = Math.random(); // aleatorio será um valor entre 0.0 e 1.0
```
***7.*** `Math.round()`

**Descrição:** Arredonda um número para o inteiro mais próximo.

```java

double numero = 5.7;
long arredondado = Math.round(numero); // arredondado será 6
```
***8.*** `Math.ceil()`

**Descrição:** Arredonda um número para cima, para o inteiro mais próximo.

```java

double numero = 5.3;
double arredondadoParaCima = Math.ceil(numero); // arredondadoParaCima será 6.0
```

***9.*** `Math.floor()`

**Descrição:** Arredonda um número para baixo, para o inteiro mais próximo.

```java

double numero = 5.7;
double arredondadoParaBaixo = Math.floor(numero); // arredondadoParaBaixo será 5.0
```
***10.*** `Math.log()`

**Descrição:** Retorna o logaritmo natural (base e) de um número.

```java

double numero = 10;
double logaritmo = Math.log(numero); // logaritmo será aproximadamente 2.302585
```
