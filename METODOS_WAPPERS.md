# Métodos Comuns das Classes Wrapper 

## Funcionalidades dos Metodos. 


***1.*** `valueOf()`

- **Descrição:** Converte um valor primitivo em um objeto da classe Wrapper correspondente.
- **Exemplo:** `Integer aObj = Integer.valueOf(5);`


```java
public class Main {
    public static void main(String[] args) {
        Integer intObj = Integer.valueOf(10);
        Double doubleObj = Double.valueOf(10.5);
        Boolean boolObj = Boolean.valueOf(true);

        System.out.println("Integer object: " + intObj);
        System.out.println("Double object: " + doubleObj);
        System.out.println("Boolean object: " + boolObj);
    }
}
```
***2.*** `xxxValue()`

- **Descrição:** Converte um objeto da classe Wrapper de volta para o tipo primitivo correspondente. Substitua xxx pelo tipo primitivo desejado (por exemplo, intValue(), doubleValue()).

**Exemplo:**  `int a = aObj.intValue();`

```java
public class Main {
    public static void main(String[] args) {
        Integer intObj = Integer.valueOf(10);
        int intValue = intObj.intValue();

        Double doubleObj = Double.valueOf(10.5);
        double doubleValue = doubleObj.doubleValue();

        System.out.println("int value: " + intValue);
        System.out.println("double value: " + doubleValue);
    }
}

```
***3.*** `parseXxx()`

**Descrição:** Converte uma string em um valor primitivo. Substitua Xxx pelo tipo primitivo desejado (por exemplo, parseInt(), parseDouble()).

**Exemplo:** `int a = Integer.parseInt("123");`
```java

public class Main {
    public static void main(String[] args) {
        int intValue = Integer.parseInt("123");
        double doubleValue = Double.parseDouble("123.45");

        System.out.println("Parsed int: " + intValue);
        System.out.println("Parsed double: " + doubleValue);
    }
}
```
***4.*** `toString()`

**Descrição:** Converte um valor primitivo ou um objeto da classe Wrapper em uma string.

**Exemplo:** `String s = Integer.toString(123);`

```java
public class Main {
    public static void main(String[] args) {
        Integer intObj = Integer.valueOf(123);
        String intStr = intObj.toString();

        Double doubleObj = Double.valueOf(123.45);
        String doubleStr = doubleObj.toString();

        System.out.println("String representation of Integer: " + intStr);
        System.out.println("String representation of Double: " + doubleStr);
    }
}
```
***5.***`toString()`

**Descrição:** Converte um valor primitivo ou um objeto da classe Wrapper em uma string.

**Exemplo:** ` String s = Integer.toString(123);`

```java 
public class Main {
    public static void main(String[] args) {
        Integer intObj1 = Integer.valueOf(10);
        Integer intObj2 = Integer.valueOf(20);

        int comparison = intObj1.compareTo(intObj2);

        System.out.println("Comparison result: " + comparison); // Output: -1 (because 10 < 20)
    }
}
```
***6.*** `equals()`

**Descrição:** Verifica se dois objetos da classe Wrapper são iguais.

**Exemplo:** `boolean isEqual = aObj.equals(anotherObj);`

```java
public class Main {
    public static void main(String[] args) {
        Integer intObj1 = Integer.valueOf(10);
        Integer intObj2 = Integer.valueOf(10);

        boolean isEqual = intObj1.equals(intObj2);

        System.out.println("Are the objects equal? " + isEqual); // Output: true
    }
}
```
***7.*** `hashCode()`

**Descrição:** Retorna o código hash do objeto.

**Exemplo:** `int hash = aObj.hashCode();`

```java 
public class Main {
    public static void main(String[] args) {
        Integer intObj = Integer.valueOf(10);
        int hashCode = intObj.hashCode();

        System.out.println("Hash code: " + hashCode);
    }
}
```
***8.*** `isNaN() (apenas para Float e Double)`

**Descrição:** Verifica se o valor é “Not-a-Number” (NaN).

**Exemplo:** `boolean isNaN = Double.isNaN(0.0 / 0.0);`

```java
public class Main {
    public static void main(String[] args) {
        Double nanValue = Double.valueOf(0.0 / 0.0);
        boolean isNaN = nanValue.isNaN();

        System.out.println("Is NaN? " + isNaN); // Output: true
    }
}
```

