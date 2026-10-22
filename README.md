# JAVA-PRACTICE-CODES

1.Arithmetic Operators

import java.util.Scanner;

public class MyClass {
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        System.out.println(a + b);
        System.out.println(a - b);
        System.out.println(a * b);
        System.out.println(a / b);
        System.out.println(a % b);

        sc.close();
    }
}

2. Unary aur Assignment Operators

public class MyClass {
    public static void main(String args[]) {
        int a = 5;
        int b = 10;

        a++;
        b--;
        a += 3;
        b *= 2;

        System.out.println(a);
        System.out.println(b);
    }
}

3. Odd/Even without % operator

import java.util.Scanner;

public class MyClass {
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();

        if ((a & 1) == 0) {
            System.out.println("Even");
        } else {
            System.out.println("Odd");
        }

        sc.close();
    }
}   

4. Greatest of Three Numbers

import java.util.Scanner;

public class MyClass {
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();
        int c = sc.nextInt();

        if (a >= b && a >= c) {
            System.out.println(a);
        } else if (b >= a && b >= c) {
            System.out.println(b);
        } else {
            System.out.println(c);
        }

        sc.close();
    }
}

5. Even Numbers from 1 to N

import java.util.Scanner;

public class MyClass {
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();

        for (int i = 1; i <= n; i++) {
            if (i % 2 == 0) {
                System.out.print(i + " ");
            }
        }

        sc.close();
    }
}

6. Count Digits of a Number

import java.util.Scanner;

public class MyClass {
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int count = 0;

        while (n > 0) {
            count++;
            n = n / 10;
        }

        System.out.println(count);
        sc.close();
    }
}

7. Sum of Inputs Until User Enters 0

import java.util.Scanner;

public class MyClass {
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);

        int n;
        int sum = 0;

        do {
            n = sc.nextInt();
            sum += n;
        } while (n != 0);

        System.out.println(sum);
        sc.close();
    }
}
