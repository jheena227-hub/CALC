[program-1 WAP for addition sub mul div using object and classes](#code1)
[program-2 WAP for addition of two distance where each distance is given in m,cm,mm](#code2)
[program-3 WAP for similarly,test the result by creation of object in main class where each distance is given in m,cm](#code3)
[program-4 WAP for similarly for time given in hours,min and seconds](#code4)
[program-5 WAP for time given in hours and miniutes](#code5)
[program-6 WAP for collect the code from internet for any five programs of c language (fact,armstrong,palindrome,fibonacci,pattern)](#code6)
[program-7 WAP for class that is having four method for 1-dimensionalarray](#code7)
[program-8 WAP for class with multiple methods to perform matrix operations (transpose,addition,sum of rows,sum of columns,sum of diagonal](#code8)
[program-9 WAP for program using three classes to print 1-100,1-100,1-100 with and without thread and analyse the output and repeat the same program using runnable interface](#code9)
[program-10 WAP for Using the concept of multithreading the output of all three threads must be synchronised (use join method).   ](#code10)
[program-11 WAP for Addition of 2 numbers using swing. ](#code11)
[program-12 WAP for Make a registration form with 10 elements and send the data into database (use jdbc connectivity)](#code12)
[program-13 WAP for Make one calculator in swing. ](#code13)
[program-14 WAP for Matrix Addition using swing class.](#code14)
[program-15 WAP for Create one jframe apply 10 buttons on that after clicking on each button a new structure is created. (Circle, oval rectangle, etc ](#code15)
[program-16 WAP for Just using mouse Event create a frame like paint brush with selection of colour and width ](#code16)
[program-17 WAP for Create one package and sub package import and test it.](#code17)
[program-18 WAP for  Create one small array of size 5 apply array out of bounds exception using try catch give a proper message in catch and demonstrate the exception exactly in the same fashion demonstrate arithmetic exception ](#code18)
[program-19 WAP for To test the range of age of one student.write a program using user defined exception.](#code19)
[program-20 WAP for File Handling Programs](#code20)
[program-21 WAP for Inheritance Programs, using interface and abstract classes.](#code21)
[program-22 WAP for Java program to create a file using FileWriter, write data into it, and then read the same file using FileReader and display its content using character stream. ](#code22)
[program-23 WAP for Java program to copy content from one file to another using byte stream (FileInputStream and FileOutputStream). ](#code23)
[program-24 WAP for Java program to copy content from one file to another using character stream (FileReader and FileWriter).](#code24)
[program-25 WAP for a Java program to perform file copying using byte stream without using character stream.](#code25)
[program-26 WAP for a Java Swing application for a Registration Form including various GUI components like JTextField, JPasswordField, JRadioButton, JCheckBox, JComboBox, and JButton. Display a success message on form submission.](#code26)
[program-27 WAP for a Java program to write data into a file using FileOutputStream and then read and display the same data using FileInputStream (Byte Stream File Handling).](#code27)
## Assi-1
```
class Arithmetic {
    int a = 10, b = 5;

    void add() { System.out.println("Add: " + (a + b)); }
    void sub() { System.out.println("Sub: " + (a - b)); }
    void mul() { System.out.println("Mul: " + (a * b)); }
    void div() { System.out.println("Div: " + (a / b)); }

    public static void main(String[] args) {
        Arithmetic obj = new Arithmetic();
        obj.add(); obj.sub(); obj.mul(); obj.div();
    }
}
```

<img width="594" height="185" alt="image" src="https://github.com/user-attachments/assets/681015d1-13aa-4480-b07a-222354312a75" />

## Assi-2
```
class Distance {
    int m, cm, mm;

    Distance(int m, int cm, int mm) {
        this.m = m;
        this.cm = cm;
        this.mm = mm;
    }

    void add(Distance d) {
        int total = (m*1000 + cm*10 + mm) + (d.m*1000 + d.cm*10 + d.mm);

        int m1 = total / 1000;
        int r = total % 1000;
        int cm1 = r / 10;
        int mm1 = r % 10;

        System.out.println(m1 + "m " + cm1 + "cm " + mm1 + "mm");
    }

    public static void main(String[] args) {
        Distance d1 = new Distance(2,50,5);
        Distance d2 = new Distance(1,30,7);
        d1.add(d2);
    }
}
```

<img width="630" height="120" alt="image" src="https://github.com/user-attachments/assets/eee6122d-4d6a-436b-ac78-4b2406f22b61" />

## Assi-3
```
class DistanceTest {
    int m, cm;

    DistanceTest(int m, int cm) {
        this.m = m;
        this.cm = cm;
    }

    void display() {
        System.out.println("Distance: " + m + "m " + cm + "cm");
    }

    public static void main(String[] args) {
        DistanceTest d = new DistanceTest(5, 75);
        d.display();
    }
}
```

<img width="627" height="116" alt="image" src="https://github.com/user-attachments/assets/6a71736e-79ce-4d04-b03e-8ed43be66f2c" />

## Assi-4
```
class TimeFull {
    int h, m, s;

    TimeFull(int h, int m, int s) {
        this.h = h;
        this.m = m;
        this.s = s;
    }

    void display() {
        System.out.println("Time: " + h + "h " + m + "m " + s + "s");
    }

    public static void main(String[] args) {
        TimeFull t = new TimeFull(2, 45, 30);
        t.display();
    }
}
```

<img width="595" height="123" alt="image" src="https://github.com/user-attachments/assets/5fadfad1-a9c5-4c53-afb2-61823f8df17c" />

## ASSI-5
```
class TimeHM {
    int h, m;

    TimeHM(int h, int m) {
        this.h = h;
        this.m = m;
    }

    void display() {
        System.out.println("Time: " + h + " hours " + m + " minutes");
    }

    public static void main(String[] args) {
        TimeHM t = new TimeHM(3, 40);
        t.display();
    }
}
```

<img width="589" height="118" alt="image" src="https://github.com/user-attachments/assets/aaaa9f35-4e45-44b4-8aa2-af296db913e2" />

## Assi-6(a)
```
#include <stdio.h>

int main() {
    int n = 5, fact = 1;
    for(int i = 1; i <= n; i++)
        fact *= i;

    printf("Factorial = %d", fact);
    return 0;
}
```

<img width="677" height="121" alt="image" src="https://github.com/user-attachments/assets/c5d0eae3-0f91-4e60-bd70-cc1cc7a6e5b5" />

6(b)
```
#include <stdio.h>

int main() {
    int n = 153, temp, r, sum = 0;
    temp = n;

    while(n > 0) {
        r = n % 10;
        sum += r*r*r;
        n /= 10;
    }

    if(temp == sum)
        printf("Armstrong Number");
    else
        printf("Not Armstrong");

    return 0;
}
```

<img width="661" height="126" alt="image" src="https://github.com/user-attachments/assets/f6901ef1-a149-4344-be1f-40834166b6be" />

6(c)
```
#include <stdio.h>

int main() {
    int n = 121, rev = 0, temp = n;

    while(n > 0) {
        rev = rev * 10 + n % 10;
        n /= 10;
    }

    if(temp == rev)
        printf("Palindrome");
    else
        printf("Not Palindrome");

    return 0;
}
```

<img width="695" height="119" alt="image" src="https://github.com/user-attachments/assets/470678a8-58c0-472b-a78f-780814619eee" />

6(d)
```
#include <stdio.h>

int main() {
    int n = 10, a = 0, b = 1, c;

    printf("%d %d ", a, b);

    for(int i = 2; i < n; i++) {
        c = a + b;
        printf("%d ", c);
        a = b;
        b = c;
    }

    return 0;
}
```

<img width="657" height="114" alt="image" src="https://github.com/user-attachments/assets/315f7133-45a6-4214-bf3a-28a8b2f2bc31" />

6(e)
```
#include <stdio.h>

int main() {
    for(int i = 1; i <= 5; i++) {
        for(int j = 1; j <= i; j++) {
            printf("* ");
        }
        printf("\n");
    }
    return 0;
}
```

<img width="661" height="216" alt="image" src="https://github.com/user-attachments/assets/66319966-16e2-47c9-96a1-8d56ebc0ab2b" />

## Assi-7
```
class Array1D {
    int arr[] = {10, 20, 30, 40, 50};

    void display() {
        System.out.print("Array: ");
        for(int i : arr)
            System.out.print(i + " ");
        System.out.println();
    }

    void reverse() {
        System.out.print("Reverse: ");
        for(int i = arr.length - 1; i >= 0; i--)
            System.out.print(arr[i] + " ");
    }

    public static void main(String[] args) {
        Array1D obj = new Array1D();
        obj.display();
        obj.reverse();
    }
}
```

<img width="615" height="142" alt="image" src="https://github.com/user-attachments/assets/8ee4b3e7-12c4-43c1-be66-9e09f3bff8dd" />

## Assi-8
```
class MatrixOps {
    int[][] a = {{1,2,3},{4,5,6},{7,8,9}};

    void display() {
        System.out.println("Matrix:");
        for(int i=0;i<3;i++){
            for(int j=0;j<3;j++){
                System.out.print(a[i][j]+" ");
            }
            System.out.println();
        }
    }

    void transpose() {
        System.out.println("Transpose:");
        for(int i=0;i<3;i++){
            for(int j=0;j<3;j++){
                System.out.print(a[j][i]+" ");
            }
            System.out.println();
        }
    }

    void rowSum() {
        for(int i=0;i<3;i++){
            int sum=0;
            for(int j=0;j<3;j++){
                sum += a[i][j];
            }
            System.out.println("Row "+i+" sum: "+sum);
        }
    }

    void colSum() {
        for(int j=0;j<3;j++){
            int sum=0;
            for(int i=0;i<3;i++){
                sum += a[i][j];
            }
            System.out.println("Col "+j+" sum: "+sum);
        }
    }

    public static void main(String[] args) {
        MatrixOps m = new MatrixOps();
        m.display();
        m.transpose();
        m.rowSum();
        m.colSum();
    }
}

```

<img width="589" height="401" alt="image" src="https://github.com/user-attachments/assets/7031e402-890d-4775-90b1-00d0f94d9d1f" />

## Assi-9
```
class A extends Thread {
    public void run() {
        for(int i=1;i<=100;i++)
            System.out.println("A: " + i);
    }
}

class B extends Thread {
    public void run() {
        for(int i=1;i<=100;i++)
            System.out.println("B: " + i);
    }
}

class C extends Thread {
    public void run() {
        for(int i=1;i<=100;i++)
            System.out.println("C: " + i);
    }
}

class ThreadDemo {
    public static void main(String[] args) {
        A t1 = new A();
        B t2 = new B();
        C t3 = new C();

        t1.start();
        t2.start();
        t3.start();
    }
}
```

<img width="599" height="807" alt="image" src="https://github.com/user-attachments/assets/5a7b2328-2289-4d8e-9a84-4297a6fae7de" />

## Assi-10
```
class A extends Thread {
    public void run() {
        for(int i=1;i<=10;i++)
            System.out.println("A: " + i);
    }
}

class B extends Thread {
    public void run() {
        for(int i=1;i<=10;i++)
            System.out.println("B: " + i);
    }
}

class C extends Thread {
    public void run() {
        for(int i=1;i<=10;i++)
            System.out.println("C: " + i);
    }
}

class ThreadJoin {
    public static void main(String[] args) throws Exception {
        A t1 = new A();
        B t2 = new B();
        C t3 = new C();

        t1.start();
        t1.join();

        t2.start();
        t2.join();

        t3.start();
        t3.join();
    }
}
```

<img width="644" height="756" alt="image" src="https://github.com/user-attachments/assets/d950fb82-2792-4936-bb81-60ece7c55e20" />

## Assi-11
```
import javax.swing.*;
import java.awt.event.*;

class AddSwing {
    public static void main(String[] args) {
        JFrame f = new JFrame("Addition");

        JTextField t1 = new JTextField();
        JTextField t2 = new JTextField();
        JTextField t3 = new JTextField();
        JButton b = new JButton("Add");

        t1.setBounds(50,50,100,30);
        t2.setBounds(50,100,100,30);
        b.setBounds(50,150,100,30);
        t3.setBounds(50,200,100,30);

        f.add(t1); f.add(t2); f.add(b); f.add(t3);

        b.addActionListener(e -> {
            int a = Integer.parseInt(t1.getText());
            int b1 = Integer.parseInt(t2.getText());
            t3.setText(String.valueOf(a + b1));
        });

        f.setSize(300,300);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```

<img width="350" height="358" alt="image" src="https://github.com/user-attachments/assets/306cca18-35f4-4f9d-b7b8-e2c3599cc24b" />

## Assi-12
```
import javax.swing.*;
import java.awt.event.*;

public class RegisterForm {
    public static void main(String[] args) {

        JFrame f = new JFrame("Registration Form");

        // Labels
        JLabel l1 = new JLabel("Name:");
        JLabel l2 = new JLabel("Email:");
        JLabel l3 = new JLabel("Password:");
        JLabel l4 = new JLabel("Gender:");
        JLabel l5 = new JLabel("DOB:");
        JLabel l6 = new JLabel("Phone:");
        JLabel l7 = new JLabel("Address:");
        JLabel l8 = new JLabel("Course:");
        JLabel l9 = new JLabel("Hobbies:");
        JLabel l10 = new JLabel("Country:");

        // TextFields
        JTextField t1 = new JTextField();
        JTextField t2 = new JTextField();
        JPasswordField t3 = new JPasswordField();
        JTextField t5 = new JTextField();
        JTextField t6 = new JTextField();
        JTextField t7 = new JTextField();

        // Radio Buttons (Gender)
        JRadioButton r1 = new JRadioButton("Male");
        JRadioButton r2 = new JRadioButton("Female");
        ButtonGroup bg = new ButtonGroup();
        bg.add(r1); bg.add(r2);

        // ComboBox (Course)
        String courses[] = {"B.Tech","BCA","MCA","MBA"};
        JComboBox c1 = new JComboBox(courses);

        // CheckBoxes (Hobbies)
        JCheckBox h1 = new JCheckBox("Reading");
        JCheckBox h2 = new JCheckBox("Music");
        JCheckBox h3 = new JCheckBox("Sports");

        // Country ComboBox
        String country[] = {"India","USA","UK","Canada"};
        JComboBox c2 = new JComboBox(country);

        // Button
        JButton b = new JButton("Submit");

        // Set Bounds
        l1.setBounds(50,30,100,30);   t1.setBounds(150,30,150,30);
        l2.setBounds(50,70,100,30);   t2.setBounds(150,70,150,30);
        l3.setBounds(50,110,100,30);  t3.setBounds(150,110,150,30);
        l4.setBounds(50,150,100,30);  r1.setBounds(150,150,70,30); r2.setBounds(220,150,80,30);
        l5.setBounds(50,190,100,30);  t5.setBounds(150,190,150,30);
        l6.setBounds(50,230,100,30);  t6.setBounds(150,230,150,30);
        l7.setBounds(50,270,100,30);  t7.setBounds(150,270,150,30);
        l8.setBounds(50,310,100,30);  c1.setBounds(150,310,150,30);
        l9.setBounds(50,350,100,30);  h1.setBounds(150,350,80,30); h2.setBounds(230,350,80,30); h3.setBounds(310,350,80,30);
        l10.setBounds(50,390,100,30); c2.setBounds(150,390,150,30);

        b.setBounds(150,440,100,30);

        // Add components
        f.add(l1); f.add(t1);
        f.add(l2); f.add(t2);
        f.add(l3); f.add(t3);
        f.add(l4); f.add(r1); f.add(r2);
        f.add(l5); f.add(t5);
        f.add(l6); f.add(t6);
        f.add(l7); f.add(t7);
        f.add(l8); f.add(c1);
        f.add(l9); f.add(h1); f.add(h2); f.add(h3);
        f.add(l10); f.add(c2);
        f.add(b);

        // Button Action
        b.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {
                JOptionPane.showMessageDialog(f, "Registration Successful");
            }
        });

        f.setSize(450,550);
        f.setLayout(null);
        f.setVisible(true);
    }
}
```

<img width="523" height="657" alt="image" src="https://github.com/user-attachments/assets/bb839c2c-9771-47bd-88de-7227b5472fba" />

## Assi-13
```
import javax.swing.*;
import java.awt.event.*;

public class Calculator {
    public static void main(String[] args) {

        JFrame f = new JFrame("Calculator");

        JTextField t = new JTextField();
        t.setBounds(30,30,240,30);

        // Buttons
        JButton b1 = new JButton("1");
        JButton b2 = new JButton("2");
        JButton b3 = new JButton("3");
        JButton b4 = new JButton("+");

        JButton b5 = new JButton("4");
        JButton b6 = new JButton("5");
        JButton b7 = new JButton("6");
        JButton b8 = new JButton("-");

        JButton b9 = new JButton("7");
        JButton b10 = new JButton("8");
        JButton b11 = new JButton("9");
        JButton b12 = new JButton("*");

        JButton b13 = new JButton("0");
        JButton b14 = new JButton("C");
        JButton b15 = new JButton("=");
        JButton b16 = new JButton("/");

        // Set positions
        b1.setBounds(30,80,50,40);
        b2.setBounds(90,80,50,40);
        b3.setBounds(150,80,50,40);
        b4.setBounds(210,80,50,40);

        b5.setBounds(30,130,50,40);
        b6.setBounds(90,130,50,40);
        b7.setBounds(150,130,50,40);
        b8.setBounds(210,130,50,40);

        b9.setBounds(30,180,50,40);
        b10.setBounds(90,180,50,40);
        b11.setBounds(150,180,50,40);
        b12.setBounds(210,180,50,40);

        b13.setBounds(30,230,50,40);
        b14.setBounds(90,230,50,40);
        b15.setBounds(150,230,50,40);
        b16.setBounds(210,230,50,40);

        // Add components
        f.add(t);
        f.add(b1); f.add(b2); f.add(b3); f.add(b4);
        f.add(b5); f.add(b6); f.add(b7); f.add(b8);
        f.add(b9); f.add(b10); f.add(b11); f.add(b12);
        f.add(b13); f.add(b14); f.add(b15); f.add(b16);

        // Variables
        final int[] num1 = new int[1];
        final int[] num2 = new int[1];
        final char[] op = new char[1];

        // Number buttons
        b1.addActionListener(e -> t.setText(t.getText() + "1"));
        b2.addActionListener(e -> t.setText(t.getText() + "2"));
        b3.addActionListener(e -> t.setText(t.getText() + "3"));
        b5.addActionListener(e -> t.setText(t.getText() + "4"));
        b6.addActionListener(e -> t.setText(t.getText() + "5"));
        b7.addActionListener(e -> t.setText(t.getText() + "6"));
        b9.addActionListener(e -> t.setText(t.getText() + "7"));
        b10.addActionListener(e -> t.setText(t.getText() + "8"));
        b11.addActionListener(e -> t.setText(t.getText() + "9"));
        b13.addActionListener(e -> t.setText(t.getText() + "0"));

        // Operators
        b4.addActionListener(e -> { num1[0] = Integer.parseInt(t.getText()); op[0] = '+'; t.setText(""); });
        b8.addActionListener(e -> { num1[0] = Integer.parseInt(t.getText()); op[0] = '-'; t.setText(""); });
        b12.addActionListener(e -> { num1[0] = Integer.parseInt(t.getText()); op[0] = '*'; t.setText(""); });
        b16.addActionListener(e -> { num1[0] = Integer.parseInt(t.getText()); op[0] = '/'; t.setText(""); });

        // Equal
        b15.addActionListener(e -> {
            num2[0] = Integer.parseInt(t.getText());
            int result = 0;

            switch(op[0]) {
                case '+': result = num1[0] + num2[0]; break;
                case '-': result = num1[0] - num2[0]; break;
                case '*': result = num1[0] * num2[0]; break;
                case '/': result = num1[0] / num2[0]; break;
            }

            t.setText(String.valueOf(result));
        });

        // Clear
        b14.addActionListener(e -> t.setText(""));

        // Frame settings
        f.setSize(320,350);
        f.setLayout(null);
        f.setVisible(true);
    }
}

```

<img width="362" height="414" alt="image" src="https://github.com/user-attachments/assets/9e4a37fb-91ee-449d-bad8-fb9d289740ac" />


## Assi-14
```
import javax.swing.*;
import java.awt.event.*;

class MatrixSwing {
    public static void main(String[] args) {
        JFrame f = new JFrame("Matrix Addition");

        JTextField a1 = new JTextField();
        JTextField a2 = new JTextField();
        JTextField b1 = new JTextField();
        JTextField b2 = new JTextField();
        JTextField r1 = new JTextField();

        JButton add = new JButton("Add");

        a1.setBounds(50,50,50,30);
        a2.setBounds(110,50,50,30);
        b1.setBounds(50,100,50,30);
        b2.setBounds(110,100,50,30);
        add.setBounds(50,150,100,30);
        r1.setBounds(50,200,100,30);

        f.add(a1); f.add(a2);
        f.add(b1); f.add(b2);
        f.add(add); f.add(r1);

        add.addActionListener(e -> {
            int x1 = Integer.parseInt(a1.getText());
            int x2 = Integer.parseInt(a2.getText());
            int y1 = Integer.parseInt(b1.getText());
            int y2 = Integer.parseInt(b2.getText());

            r1.setText((x1+y1) + " " + (x2+y2));
        });

        f.setSize(300,300);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```

<img width="353" height="363" alt="image" src="https://github.com/user-attachments/assets/a5f9ac03-959a-47f2-866a-8be82e19f660" />

## Assi-15
```
import javax.swing.*;
import java.awt.event.*;

class ShapeButtons {
    public static void main(String[] args) {
        JFrame f = new JFrame("Shapes");

        JButton b1 = new JButton("Circle");
        JButton b2 = new JButton("Rectangle");
        JButton b3 = new JButton("Oval");

        b1.setBounds(50,50,120,30);
        b2.setBounds(50,100,120,30);
        b3.setBounds(50,150,120,30);

        f.add(b1); f.add(b2); f.add(b3);

        b1.addActionListener(e -> System.out.println("Circle Selected"));
        b2.addActionListener(e -> System.out.println("Rectangle Selected"));
        b3.addActionListener(e -> System.out.println("Oval Selected"));

        f.setSize(300,300);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```

<img width="621" height="157" alt="image" src="https://github.com/user-attachments/assets/d141e979-b883-4a85-b1b1-5c7baa266c8e" />

## Assi-16
```
import javax.swing.*;
import java.awt.event.*;

class ShapeButtons {
    public static void main(String[] args) {
        JFrame f = new JFrame("Shapes");

        JButton b1 = new JButton("Circle");
        JButton b2 = new JButton("Rectangle");
        JButton b3 = new JButton("Oval");

        b1.setBounds(50,50,120,30);
        b2.setBounds(50,100,120,30);
        b3.setBounds(50,150,120,30);

        f.add(b1); f.add(b2); f.add(b3);

        b1.addActionListener(e -> System.out.println("Circle Selected"));
        b2.addActionListener(e -> System.out.println("Rectangle Selected"));
        b3.addActionListener(e -> System.out.println("Oval Selected"));

        f.setSize(300,300);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```

<img width="345" height="358" alt="image" src="https://github.com/user-attachments/assets/ac39cd41-2d65-47d0-bef7-dbd0715b2f7c" />

<img width="621" height="157" alt="image" src="https://github.com/user-attachments/assets/b8f177c6-d9d7-4d32-816d-6fb3489a28d4" />


## Assi-17
```
import javax.swing.*;
import java.awt.*;
import java.awt.event.*;

class PaintBrush extends JFrame {
    int x, y;

    PaintBrush() {
        addMouseMotionListener(new MouseMotionAdapter() {
            public void mouseDragged(MouseEvent e) {
                x = e.getX();
                y = e.getY();
                repaint();
            }
        });

        setSize(400,400);
        setTitle("Paint Brush");
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setVisible(true);
    }

    public void paint(Graphics g) {
        g.fillOval(x, y, 10, 10);
    }

    public static void main(String[] args) {
        new PaintBrush();
    }
}
```

<img width="470" height="479" alt="image" src="https://github.com/user-attachments/assets/cc4ec760-2822-47d0-829d-19a09e4728a6" />

## Assi-18
```
class ExceptionDemo {
    public static void main(String[] args) {

        try {
            int a = 10 / 0;
        } catch (Exception e) {
            System.out.println("Arithmetic Exception Occurred");
        }

        try {
            int arr[] = new int[5];
            arr[10] = 20;
        } catch (Exception e) {
            System.out.println("Array Index Out of Bounds");
        }
    }
}
```

<img width="633" height="137" alt="image" src="https://github.com/user-attachments/assets/1469ad7a-9205-49dc-8699-eaa1a91abd5a" />

## Assi-19
```
class AgeException extends Exception {
    AgeException(String msg) {
        super(msg);
    }
}

class TestAge {
    static void checkAge(int age) throws AgeException {
        if(age < 18)
            throw new AgeException("Age must be 18+");
        else
            System.out.println("Valid Age");
    }

    public static void main(String[] args) {
        try {
            checkAge(16);
        } catch (Exception e) {
            System.out.println(e.getMessage());
        }
    }
}
```

<img width="650" height="115" alt="image" src="https://github.com/user-attachments/assets/a720e3fc-40ec-4f17-a8e5-6ef74e9f386d" />

## Assi-20
```
import java.io.*;

class FileHandling {
    public static void main(String[] args) {
        try {
            FileWriter fw = new FileWriter("test.txt");
            fw.write("Hello File Handling");
            fw.close();

            BufferedReader br = new BufferedReader(new FileReader("test.txt"));
            String s;
            while((s = br.readLine()) != null) {
                System.out.println(s);
            }
            br.close();

        } catch(Exception e) {
            System.out.println(e);
        }
    }
}
```

<img width="642" height="123" alt="image" src="https://github.com/user-attachments/assets/f1efb52f-c20f-4304-ae55-33d246c4a909" />

## Assi-21
```
interface A {
    void show();
}

abstract class B {
    abstract void display();
}

class C extends B implements A {
    public void show() {
        System.out.println("Interface Method");
    }

    void display() {
        System.out.println("Abstract Method");
    }
}

class InheritanceDemo {
    public static void main(String[] args) {
        C obj = new C();
        obj.show();
        obj.display();
    }
}
```
<img width="644" height="139" alt="image" src="https://github.com/user-attachments/assets/c5e6d14b-229d-4762-b0eb-fbc9bef79481" />

## Assi-22
```
import java.io.*;

public class charFilecopy {
    public static void main(String[] args) {
        try {
            // Create source file (for testing)
            FileWriter test = new FileWriter("source.txt");
            test.write("Hello Java Character Copy");
            test.close();

            // File transfer (character stream)
            FileReader fr = new FileReader("source.txt");
            FileWriter fw = new FileWriter("dest_char.txt");

            int ch;
            while ((ch = fr.read()) != -1) {
                fw.write(ch);
            }

            fr.close();
            fw.close();

            System.out.println("File copied using character stream");

        } catch (Exception e) {
            System.out.println(e);
        }
    }
}
```
<img width="625" height="132" alt="image" src="https://github.com/user-attachments/assets/a5f1e782-3997-4817-b22d-9820d7fbe1ff" />

## Assi-23
```
import java.io.*;

public class byteFilecopy {
    public static void main(String[] args) {
        try {
            // Create source file (for testing)
            FileOutputStream test = new FileOutputStream("source.txt");
            String data = "Hello Java Byte Copy";
            test.write(data.getBytes());
            test.close();

            // File transfer (byte stream)
            FileInputStream fis = new FileInputStream("source.txt");
            FileOutputStream fos = new FileOutputStream("dest_byte.txt");

            int b;
            while ((b = fis.read()) != -1) {
                fos.write(b);
            }

            fis.close();
            fos.close();

            System.out.println("File copied using byte stream");

        } catch (Exception e) {
            System.out.println(e);
        }
    }
}
```
<img width="629" height="131" alt="image" src="https://github.com/user-attachments/assets/6a01ee96-cdf5-4a76-8d11-ed2d54ecd8aa" />

## Assi-24
```
import java.io.*;

public class CharCopy {
    public static void main(String[] args) {
        try {
            // Create source file
            FileWriter test = new FileWriter("source.txt");
            test.write("Hello Java Character Copy");
            test.close();

            // Character stream copy
            FileReader fr = new FileReader("source.txt");
            FileWriter fw = new FileWriter("dest_char.txt");

            int ch;
            while ((ch = fr.read()) != -1) {
                fw.write(ch);
            }

            fr.close();
            fw.close();

            System.out.println("Character file copied successfully");

        } catch (Exception e) {
            System.out.println(e);
        }
    }
}
```
<img width="576" height="116" alt="image" src="https://github.com/user-attachments/assets/a5451d6a-112f-4705-904e-8c82563f34c4" />

## Assi-25
```
import java.io.*;

public class ByteCopy {
    public static void main(String[] args) {
        try {
            FileInputStream fis = new FileInputStream("source.txt");
            FileOutputStream fos = new FileOutputStream("dest.txt");

            int b;
            while ((b = fis.read()) != -1) {
                fos.write(b);
            }

            fis.close();
            fos.close();

            System.out.println("Byte file copied successfully");

        } catch (Exception e) {
            System.out.println(e);
        }
    }
}
```
<img width="597" height="119" alt="image" src="https://github.com/user-attachments/assets/f6a0976c-ebe6-4225-9d9c-659b5bea390d" />

## Assi-26
```
import javax.swing.*;
import java.awt.event.*;

public class RegisterForm {
    public static void main(String[] args) {

        JFrame f = new JFrame("Registration Form");

        // Labels
        JLabel l1 = new JLabel("Name:");
        JLabel l2 = new JLabel("Email:");
        JLabel l3 = new JLabel("Password:");
        JLabel l4 = new JLabel("Gender:");
        JLabel l5 = new JLabel("DOB:");
        JLabel l6 = new JLabel("Phone:");
        JLabel l7 = new JLabel("Address:");
        JLabel l8 = new JLabel("Course:");
        JLabel l9 = new JLabel("Hobbies:");
        JLabel l10 = new JLabel("Country:");

        // TextFields
        JTextField t1 = new JTextField();
        JTextField t2 = new JTextField();
        JPasswordField t3 = new JPasswordField();
        JTextField t5 = new JTextField();
        JTextField t6 = new JTextField();
        JTextField t7 = new JTextField();

        // Radio Buttons (Gender)
        JRadioButton r1 = new JRadioButton("Male");
        JRadioButton r2 = new JRadioButton("Female");
        ButtonGroup bg = new ButtonGroup();
        bg.add(r1); bg.add(r2);

        // ComboBox (Course)
        String courses[] = {"B.Tech","BCA","MCA","MBA"};
        JComboBox c1 = new JComboBox(courses);

        // CheckBoxes (Hobbies)
        JCheckBox h1 = new JCheckBox("Reading");
        JCheckBox h2 = new JCheckBox("Music");
        JCheckBox h3 = new JCheckBox("Sports");

        // Country ComboBox
        String country[] = {"India","USA","UK","Canada"};
        JComboBox c2 = new JComboBox(country);

        // Button
        JButton b = new JButton("Submit");

        // Set Bounds
        l1.setBounds(50,30,100,30);   t1.setBounds(150,30,150,30);
        l2.setBounds(50,70,100,30);   t2.setBounds(150,70,150,30);
        l3.setBounds(50,110,100,30);  t3.setBounds(150,110,150,30);
        l4.setBounds(50,150,100,30);  r1.setBounds(150,150,70,30); r2.setBounds(220,150,80,30);
        l5.setBounds(50,190,100,30);  t5.setBounds(150,190,150,30);
        l6.setBounds(50,230,100,30);  t6.setBounds(150,230,150,30);
        l7.setBounds(50,270,100,30);  t7.setBounds(150,270,150,30);
        l8.setBounds(50,310,100,30);  c1.setBounds(150,310,150,30);
        l9.setBounds(50,350,100,30);  h1.setBounds(150,350,80,30); h2.setBounds(230,350,80,30); h3.setBounds(310,350,80,30);
        l10.setBounds(50,390,100,30); c2.setBounds(150,390,150,30);

        b.setBounds(150,440,100,30);

        // Add components
        f.add(l1); f.add(t1);
        f.add(l2); f.add(t2);
        f.add(l3); f.add(t3);
        f.add(l4); f.add(r1); f.add(r2);
        f.add(l5); f.add(t5);
        f.add(l6); f.add(t6);
        f.add(l7); f.add(t7);
        f.add(l8); f.add(c1);
        f.add(l9); f.add(h1); f.add(h2); f.add(h3);
        f.add(l10); f.add(c2);
        f.add(b);

        // Button Action
        b.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {
                JOptionPane.showMessageDialog(f, "Registration Successful");
            }
        });

        f.setSize(450,550);
        f.setLayout(null);
        f.setVisible(true);
    }
}
```
<img width="641" height="129" alt="image" src="https://github.com/user-attachments/assets/ef1859c9-e185-4643-a716-fdc96391ae39" />

## Assi-27
```
import java.io.*;

public class ByteFileDemo {
    public static void main(String[] args) {
        try {
            FileOutputStream fos = new FileOutputStream("bytefile.txt");
            fos.write("Hello".getBytes());
            fos.close();

            FileInputStream fis = new FileInputStream("bytefile.txt");

            int b;
            while ((b = fis.read()) != -1) {
                System.out.print((char) b);
            }

            fis.close();

        } catch (Exception e) {
            System.out.println(e);
        }
    }
}
```
<img width="623" height="118" alt="image" src="https://github.com/user-attachments/assets/fb412b0e-690e-47b7-b764-cc8f16662603" />








``````
