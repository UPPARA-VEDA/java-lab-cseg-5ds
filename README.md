# java-lab-cseg-5ds
experiments
## Title:1a(DefaultPrimitiveTypes)
```
class DefaultPrimitiveType {
    byte primbyte;
    short primshort;
    int primint;
    double primdouble;
    char primchar;
    float primfloat;
    long primlong;
    boolean primboolean;
    public static void main(String args[]) {
        DefaultPrimitiveType dDpt = new DefaultPrimitiveType();
        System.out.println("default value of byte:" + dDpt.primbyte);
        System.out.println("default value of short:" + dDpt.primshort);
        System.out.println("default value of int:" + dDpt.primint);
        System.out.println("default value of double:" + dDpt.primdouble);
        System.out.println("default value of char:" + dDpt.primchar + " '");
        System.out.println("default value of float:" + dDpt.primfloat);
        System.out.println("default value of long:" + dDpt.primlong);
        System.out.println("default value of boolean:" + dDpt.primboolean);
    }
}
```
## Output :
![output for 1a](https://github.com/UPPARA-VEDA/java-lab-cseg-5ds/blob/85119def5e4c3fcc258f483a433b756a57e3f11c/exp1a.png)

## Title:1b(Quadratic Equation)
```
import java.util.Scanner;
class Quadraticequation{
     public static void main(String args[]){
         Scanner sc=new Scanner(System.in);
         System.out.println("Enter value of a:");
         double a=sc.nextDouble();
          System.out.println("Enter value of b:");
         double b=sc.nextDouble();
          System.out.println("Enter value of c:");
         double c=sc.nextDouble();
         double D=b*b-4*a*c;
         if(D>0){
            System.out.println("Roots are real and distinct");
            double root1=(-b+Math.sqrt(D))/(2*a);
            double root2=(-b-Math.sqrt(D))/(2*a);
            System.out.println("Root1:"+root1);
            System.out.println("Root2:"+root2);
            }
         else if(D==0){
            System.out.println("Roots are equal and real");
            double root=-b/(2*a);
            System.out.println("Root:"+root);
            }
         else{
            System.out.println("Roots are complex and imaginary");
            double realpart=-b/(2*a);
            double imaginarypart=Math.sqrt(-D)/(2*a);
            System.out.println("Roots are complex and imaginary");
            System.out.println("Root1="+realpart+"+i"+imaginarypart);
            System.out.println("Root2="+realpart+"-i"+imaginarypart);
            }
        sc.close();
        }
   }
```

   ## Output :
![output for 1b](https://github.com/UPPARA-VEDA/java-lab-cseg-5ds/blob/6062d27a164d7f057725ad8e3ba7ccd1c8bdaf50/exp1b.png)

## Title:2a(Class Mechanism)
```
class Rectangle{
  double l;
  double b;
  double area(){
    return l*b;
  }
  double perimeter(){
   return 2*(l+b);
   }
 }
class main{
  public static void main(String args[]){
    Rectangle rect =new Rectangle();
    rect.l=6;
    rect.b=12;
    double area = rect.area();
    double perimeter =rect.perimeter();
    System.out.println("area is:" +area);
    System.out.println("perimeter is:" +perimeter);
    }
  }
```
 ## Output :
![output for 2a](https://github.com/UPPARA-VEDA/java-lab-cseg-5ds/blob/058e5184b77959e81ef10f3ded4fe6e68604439f/exp2a.png)

## Title:2b(Method Overloading)
```
class sum{
  int sum(int a ,int b){
    return a+b;
  }
  int sum(int a ,int b,int c){
  return a+b+c;
  }
  double sum(double a ,double b){
   return a+b;
  }
}
class main{
 public static void main(String args[]){
   sum s= new sum();
   System.out.println("sum of 2 integers:"+s.sum(20,16));
   System.out.println("sum of 3 integers:"+s.sum(20,16,17));
   System.out.println("sum of two real numbers:"+s.sum(30.465,15.675));
  }
}
```

 ## Output :
![output for 2b](










