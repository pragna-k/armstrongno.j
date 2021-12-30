# armstrongno.j
import java.util.*;
import java.lang.Math;
public class armstrongno
{
public static void main(String[] args)
{
Scanner knnc=new Scanner(System.in);
System.out.println("enter n value");
int n=knnc.nextInt();
int i,c=0;
int m,l,x;
double y=0;
m=n;
l=n;
while(m>0)
{
c++;
m=m/10;
}
while(l>0)
{
x=l%10;
y=y+Math.pow(x,c);
l=l/10;
}
if (y==n)
{
System.out.println(n+" is a armstrong number");
}
else
{
System.out.println(n+" is not a armstrong number");
}
}
}
