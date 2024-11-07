#  Métodos da Classe String

 ## Principais métodos utilizados em Java com Exemplos Práticos

***1.*** `charAt()`

Retorna o caractere em uma posição específica.

```java

public class Main {
    public static void main(String[] args) {
        String str = "Hello";
        char ch = str.charAt(1); // 'e'
        System.out.println("Character at index 1: " + ch);
    }
}
```

***2.*** `length()`

Retorna o comprimento da string.

```java

public class Main {
    public static void main(String[] args) {
        String str = "Hello";
        int length = str.length();
        System.out.println("Length of the string: " + length);
    }
}

```


***3.***  `substring()`

Retorna uma substring da string original.

```java

public class Main {
    public static void main(String[] args) {
        String str = "Hello, World!";
        String substr = str.substring(7, 12); // "World"
        System.out.println("Substring: " + substr);
    }
}
```
***4.*** `toLowerCase() e toUpperCase()`

Converte a string para letras minúsculas ou maiúsculas.

```java

public class Main {
    public static void main(String[] args) {
        String str = "Hello, World!";
        String lower = str.toLowerCase();
        String upper = str.toUpperCase();
        System.out.println("Lowercase: " + lower);
        System.out.println("Uppercase: " + upper);
    }
}
```

***5.*** `trim()`

Remove espaços em branco no início e no final da string.

```java

public class Main {
    public static void main(String[] args) {
        String str = "   Hello, World!   ";
        String trimmed = str.trim();
        System.out.println("Trimmed string: '" + trimmed + "'");
    }
}
```

***6.*** `equals() e equalsIgnoreCase()`

Compara duas strings para verificar se são iguais, considerando ou ignorando diferenças de maiúsculas e minúsculas.

```java

public class Main {
    public static void main(String[] args) {
        String str1 = "Hello";
        String str2 = "hello";
        boolean isEqual = str1.equals(str2); // false
        boolean isEqualIgnoreCase = str1.equalsIgnoreCase(str2); // true
        System.out.println("Equals: " + isEqual);
        System.out.println("Equals ignoring case: " + isEqualIgnoreCase);
    }
}
```

***7.*** `replace()`

Substitui todas as ocorrências de um caractere ou sequência de caracteres por outra.

```java

public class Main {
    public static void main(String[] args) {
        String str = "Hello, World!";
        String replaced = str.replace("World", "Java");
        System.out.println("Replaced string: " + replaced);
    }
}

```

***8.*** `split()`

Divide a string em um array de substrings com base em um delimitador.

```java

public class Main {
    public static void main(String[] args) {
        String str = "apple,banana,cherry";
        String[] fruits = str.split(",");
        for (String fruit : fruits) {
            System.out.println(fruit);
        }
    }
}
``` 

***9.*** `indexOf()`

Retorna o índice da primeira ocorrência de um caractere ou sequência de caracteres.

```java

public class Main {
    public static void main(String[] args) {
        String str = "Hello, World!";
        int index = str.indexOf("World");
        System.out.println("Index of 'World': " + index);
    }
}
```

***10.*** `contains()`

Verifica se a string contém uma sequência específica de caracteres.

```java

public class Main {
    public static void main(String[] args) {
        String str = "Hello, World!";
        boolean contains = str.contains("World");
        System.out.println("Contains 'World': " + contains);
    }
}
```
