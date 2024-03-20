## Задание 2 Java (11)

1. Написать программу, которая принимает на вход два целых числа (a и b) и совершает с ними следующие действия:
сравнивает эти два числа и возвращает результат сравнения путем вывода в консоль одного из вариантов: "a > b", "a < b" или "a = b";
совершает с этими числами операции сложения, вычитания, деления и умножения и результат выводит в консоль.

```

import java.util.Scanner;

public class main {
    public static void Main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Ввод двух целых чисел
        System.out.print("Введите первое целое число (a): ");
        int a = scanner.nextInt();

        System.out.print("Введите второе целое число (b): ");
        int b = scanner.nextInt();

        // Сравнение чисел и вывод результата
        if (a > b) {
            System.out.println("a > b");
        } else if (a < b) {
            System.out.println("a < b");
        } else {
            System.out.println("a = b");
        }

        // Операции со значениями a и b и вывод результатов
        System.out.println("a + b = " + (a + b));
        System.out.println("a - b = " + (a - b));
        
        // Проверка деления на 0
        if(b != 0){
            System.out.println("a / b = " + ((double)a / b)); // Чтобы получить вещественный результат
        } else {
            System.out.println("Невозможно выполнить деление на 0.");
        }
        
        System.out.println("a * b = " + (a * b));

        scanner.close();
    }
}

```
2. Написать программу, которая принимает на вход две строки (a и b) и сравнивает их. В результате сравнения в консоль должно быть выведено одно из сообщений: "Строки неидентичны" или "Строки идентичны"

```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Ввод двух строк
        System.out.print("Введите первую строку (a): ");
        String a = scanner.nextLine();

        System.out.print("Введите вторую строку (b): ");
        String b = scanner.nextLine();

        // Сравнение строк и вывод результата
        if (a.equals(b)) {
            System.out.println("Строки идентичны");
        } else {
            System.out.println("Строки неидентичны");
        }

        scanner.close();
    }
}
```

3. Задан массив целых чисел: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]. Необходимо написать программу, которая выведет в консоль все чётные числа.

```
public class Main {
    public static void main(String[] args) {
        // Заданный массив целых чисел
        int[] numbers = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

        // Вывод четных чисел
        System.out.println("Четные числа в массиве:");
        for (int number : numbers) {
            if (number % 2 == 0) {
                System.out.print(number + " ");
            }
        }
    }
}
```
