# Introdução a Classes, Métodos, Objetos e Construtores em Java

## Classes

Uma classe em Java é como um molde ou um plano que define a estrutura e o comportamento de objetos. Pense em uma classe como a planta de uma casa. Ela descreve como a casa será construída, mas não é a casa em si.

 **`Exemplo de uma classe: `**
```java

public class Pessoa {
    // Atributos (ou variáveis de instância)
    String nome;
    int idade;

    // Métodos (ou funções)
    void falar() {
        System.out.println("Olá, meu nome é " + nome);
    }

    void aniversario() {
        idade++;
    }
}
```
## Objetos
Um objeto é uma instância de uma classe. Usando a analogia da casa, se a classe é a planta, o objeto é a casa construída a partir dessa planta. Cada objeto tem suas próprias características (atributos) e pode realizar ações (métodos).

**` Criando um objeto:  `**
```java

public class Main {
    public static void main(String[] args) {
        // Criando um objeto da classe Pessoa
        Pessoa pessoa1 = new Pessoa();
        pessoa1.nome = "João";
        pessoa1.idade = 25;

        // Usando os métodos do objeto
        pessoa1.falar(); // Saída: Olá, meu nome é João
        pessoa1.aniversario();
        System.out.println(pessoa1.idade); // Saída: 26
    }
}
```
## Métodos
Os métodos são as ações que um objeto pode realizar. Eles são definidos dentro de uma classe e podem manipular os atributos da classe ou realizar outras operações.

**Exemplo de métodos:**
No exemplo da classe Pessoa, temos dois métodos:

    falar(): Imprime uma mensagem com o nome da pessoa.

    falar(): Imprime uma mensagem com o nome da pessoa.

### Construtores
Os construtores são métodos especiais usados para inicializar objetos. Eles são chamados automaticamente quando um objeto é criado e têm o mesmo nome da classe. Construtores não têm tipo de retorno, nem mesmo void.

#### Tipos de Construtores:
***1.Construtor Padrão:*** Não recebe parâmetros e é fornecido automaticamente pelo Java se nenhum outro construtor for definido.

```java
public class Carro {
    String modelo;
    int ano;

    // Construtor padrão
    public Carro() {
        modelo = "Desconhecido";
        ano = 2020;
    }
}
```
***2.Construtor Parametrizado:*** Recebe parâmetros que permitem inicializar os atributos da classe com valores específicos.
```java 
public class Carro {
    String modelo;
    int ano;

    // Construtor parametrizado
    public Carro(String modelo, int ano) {
        this.modelo = modelo;
        this.ano = ano;
    }
}
```
***Sobrecarga de Construtores:*** Você pode ter múltiplos construtores em uma classe, desde que eles tenham assinaturas diferentes (diferentes tipos ou quantidades de parâmetros).
```java
public class Carro {
    String modelo;
    int ano;

    // Construtor padrão
    public Carro() {
        modelo = "Desconhecido";
        ano = 2020;
    }

    // Construtor parametrizado
    public Carro(String modelo, int ano) {
        this.modelo = modelo;
        this.ano = ano;
    }
}
```
### Membros da Classe

Os **membros da classe** incluem atributos (variáveis) e métodos (funções) que pertencem à classe.

**`1.Atributos: `** São variáveis que armazenam o estado de um objeto.

```java
public class Pessoa {
    String nome; // Atributo de instância
    int idade;   // Atributo de instância
}
```
**`2.Métodos:`** São funções que definem o comportamento dos objetos.

```java
public class Pessoa {
    String nome;
    int idade;

    // Método para falar
    void falar() {
        System.out.println("Olá, meu nome é " + nome);
    }

    // Método para incrementar a idade
    void aniversario() {
        idade++;
    }
}
```
#### Resumo

* **Classe:**  Define a estrutura e o comportamento dos objetos.
* **Objeto:** Uma instância de uma classe, com seus próprios atributos e métodos.
* **Métodos:** Ações que os objetos podem realizar.
* **Construtores:** Inicializam objetos e podem ser padrão ou parametrizados.
* **Atributos:** Variáveis que representam o estado de um objeto.
