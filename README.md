import java .util.Scanner;
class demo1 extends Thread
{
public  void run()
{
System.out.println("Banking activitystarted");
Scanner scan=new Scanner(System.in);
System.out.println("Enter the account number:");
int acc=scan.nextInt() 
System.out.println("Enter the password:");
int pwd=scan.nextInt();
Thread.sleep(5000);
System.out.println("collect your cash!");
System.out.println("Banking activity completed");
}
}

class demo2 extends Thread
{
public void run()
{
System.out.println("Addition activity started");
int num1=753427283;
int  num2=9972888810;
Thread.sleep(5000);
int res=num1+num2;
System.out.println("the sum is:"+res);
System.out.println("Addition activity completed");
}
}

class demo3 extends thread
{
public void run()
{
System.out.println("printing activity started");
for(int i=65;i<=69;++i);
{
   System.out.println((char)i);
Thread.sleep(5000);
}
System.out.println("printing  activity completed");
}
}
class launch
{
public static void main(String[]args)
{
demo1 d1=new demo1();
demo2 d2=new demo2();
demo3 d3=new demo3();

d1.start();
d2.start();
d3.start();
}
}




