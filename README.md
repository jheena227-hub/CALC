# CALC
[PROGRAM 01 WAP to make a calculator](#code1)
[PROGRAM 02 WAP to check the age is valid or not](#code2)
[PROGRAM 03 WAP to add two distances](#code3)
## code1
```

class calc{
    public static int add(int a,int b){
        return (a+b);
    }
    public static int sub(int a,int b){
        return (a-b);
    }
    public static int mul(int a,int b){
        return (a*b);
    }
    public static int div(int a,int b){
        return (a/b);
    }
     public static void main(String args[]){
        int num1=Integer.parseInt(args[0]);
        int num2=Integer.parseInt(args[1]);
        System.out.println(add(num1, num2));
        System.out.println(sub(num1, num2));
        System.out.println(mul(num1, num2));
        System.out.println(div(num1, num2));
        
       
    }
}
```
<img width="1013" height="253" alt="Screenshot 2026-02-20 122258" src="https://github.com/user-attachments/assets/b4a348ab-55fe-405f-b091-e444a8e54873" />

## code2
```
public  static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter your age: ");
        int age = sc.nextInt();

        if (age >= 1 && age <= 120) {
            System.out.println("Valid Age");
        } 
        else {
            System.out.println("Invalid Age");
        }

        sc.close();
    
}
```
<img width="819" height="205" alt="Screenshot 2026-02-20 123333" src="https://github.com/user-attachments/assets/d70ef64c-4c28-4f8e-baf2-5485817b61e3" />

##code3

'''

    public static void main(String args[])
    {
        Distance d1=new Distance(3,02,40);
        Distance d2=new Distance(4,55,60);
        Distance result=new Distance();
        result.add(d1,d2);
        result.display();
    }

'''
<img width="473" height="66" alt="image" src="https://github.com/user-attachments/assets/6da54077-abe6-4755-8723-d0175d05fda0" />
