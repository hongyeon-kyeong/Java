1. String → char

    (1) 단일일 경우

    ```java
    String str = "c";
    char ch = str.charAt(0);
    ```

    (2) 문자 여러개일 경우

    ```java
    String str = "java";
    char[] arrayChar = str.toCharArray();
    // ["j","a","v","a"]
    ```

2. char → String

    (1) Character 클래스 toString() 메소드 (내부적으로 String 클래스의 valueOf() 메소드 호출)

    ```java
    char ch =  "A";
    String str = Character.toString(ch);
    String str2 = new Character(ch).toString();
    ```

    (2) String 클래스의 valueOf() 메소드

    ```java
    char ch = "A";
    char[] arrChar = new char[] {'a','b','c'};

    String str = String.valueOf(ch);
    String str2 = String.valueOf(arrChar);
    ```

    (3) String 클래스 생성자

    ```java
    char[] arrChar = new char[] {'a','b','c'};
    String str = new String(arrChar);
    ```

    (4) + 연산자

    ```java
    char ch = "A";
    String str = ch + "";
    ```
