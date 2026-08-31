# BASIC

## conditional | *if, if...else, if...else if...else*

<img width="300" height="840" alt="image" src="https://github.com/user-attachments/assets/5d38e486-3764-4dd9-b1b7-78a7acde039a" />
<img width="300" height="840" alt="image" src="https://github.com/user-attachments/assets/8393cf8f-7dcf-4621-9697-196ebe2f5505" />
<img width="300" height="840" alt="image" src="https://github.com/user-attachments/assets/e49898ba-1ce6-42c6-9bf0-62595c5ae3fe" />

## User input | In / Scanner 

### Scanner
# Java Input

## 1. Scanner

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String str = sc.next();      // reads a single token (stops at whitespace)
        String line = sc.nextLine(); // reads a whole line (stops at newline)
        int num = sc.nextInt();      // reads an integer

        sc.close();                  // closes the scanner
    }
}
```

> **Note:** `next()` and `nextInt()` leave the newline character in the buffer.
> Calling `nextLine()` right after them returns an empty string.
> Use an extra `sc.nextLine()` to consume the leftover newline.

> **Note:** `sc.close()` also closes `System.in`.
> Once closed, no further console input is possible in that program.

## 2. System.in (raw byte input)

> **`throws Exception` is required because `read()` declares a checked `IOException`.**
> `IOException` : Input Output Exception
> `throws IOException`은 컴파일만 통과시킬 뿐, 실제로 예외가 발생하면 프로그램은 종료된다.

```java
public class Main {
    public static void main(String[] args) throws Exception {
        int input = System.in.read();  // reads one byte, returns 0–255 (-1 at EOF)
        System.out.println(input);        // 65
        System.out.println((char) input); // A
    }
}
```
> Korean (and other multi-byte characters) will not throw an exception —
> they silently produce garbled output.
`System.in.read()` returns an `int`, not a character.
Cast to `char` to display the actual letter.

`throws Exception` is required because `read()` declares a checked `IOException`.


## Comparison

| | Scanner | System.in.read() |
|---|---|---|
| Unit | token / line | 1 byte |
| Returns | String, int, ... | int (byte value) |
| Exception handling | not required | required |
| Korean text | OK | breaks (UTF-8 is multi-byte) |
| Use case | general | learning / low-level |

## 3. In class input

```java

```
