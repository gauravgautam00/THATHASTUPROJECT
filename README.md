# THATHASTUPROJECT
This contain java code 
*Q1
******************************************************************

package com.company;
import java.util.Scanner;

Q1

 public class thathastuscholarnovcohort {
   public static void main(String[] args) {
        Scanner sc = new Scanner (System.in);


        while(true){
            System.out.println("Enter two no. to perform the task given below");

            double n=sc.nextDouble();
            double m=sc.nextDouble();



            System.out.println("write the task you want to do via this calculator");
           char mm=sc.next().charAt(1);
           switch(mm){
               case '+':
                   System.out.println(n+m);
                   break;
               case '-':
                   System.out.println(n-m);
                   break;
               case '*':
                   System.out.println(n*m);
                   break;
               case '/':
                   System.out.println(n/m);

                   break;

           }
            System.out.println("enter 1 for continue or 0 for dismiss");
           short nn=sc.nextShort();

           if(nn==0){
               break;
           }
        }
    */
/*Q2
****************************************************************
public class thathastuscholarnovcohort {
    public static int fabonacciSeries(int n){
        if(n<=1){
            return n;
        }
        return fabonacciSeries(n-1)+fabonacciSeries(n-2);
        }

          public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
    int N=sc.nextInt();
    for(int i=0;i<=N;i++){
        System.out.println(fabonacciSeries(i));
    }















    }
}*/
/*Q3
**********************************************************************8
public class thathastuscholarnovcohort {
    public static int calculateFactorial(int b) {
        if(b==0 || b==1){
            return 1;
        }
      return b*calculateFactorial((b-1));
    }

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int bb=sc.nextInt();
        System.out.println(calculateFactorial((bb)));
  */
/*
Q4
*************************************************************************
public class thathastuscholarnovcohort {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        String kk=sc.nextLine();
        StringBuilder sb=new StringBuilder(kk);

        for(int i=0;i<kk.length()/2;i++){
            int g=i;
            int h=kk.length()-i-1;
            char frontm=sb.charAt(i);
            char backn=sb.charAt(sb.length()-i-1);
            sb.setCharAt(g,backn);
            sb.setCharAt(h,frontm);


        }
    String jl=new String(sb);


        System.out.println(kk.equals(jl));

    }


    */
/*
Q5
******************************************************************
public class thathastuscholarnovcohort {
    public static int factorial(int b) {
        if(b==0 || b==1){
            return 1;
        }
        return b*factorial((b-1));
    }
    public static void main(String[] args) {
            System.out.println("Permutation \n enter two numbers as of format first N  and then R as NpR");
    Scanner sc=new Scanner(System.in);
    int m=sc.nextInt();
        int mn=sc.nextInt();
        if(m>mn) {
            double fact1 = factorial(m);
            double fact2 = factorial(m - mn);
            System.out.println("permutation of above no. is"+fact1 / fact2);

            double fact3 = factorial((mn));
            System.out.println("combination of above no. is"+(fact1 / (fact2 * fact3)));

        }
        else{
            System.out.println("invalid");
        }
    }
}*/
/*
Q6
******************************************************************
public class thathastuscholarnovcohort {
    public static void main(String[] args) {
        Scanner sc=new Scanner (System.in);
        int n=sc.nextInt();
        for(int i=0;i<=n;i++){
            for(int j=0;j<n-i;j++){
                System.out.print(" ");
            }
            for(int k=0;k<=i;k++){
                System.out.print("*");
            }
            for(int ll=0;ll<i;ll++){
                System.out.print("*");
            }

            System.out.println();
        }
        for(int i=n;i>=1;i--){
            for(int j=0;j<=n-i;j++){
                System.out.print(" ");
            }
            for(int k=0;k<i;k++){
                System.out.print("*");
            }
            for(int ll=1;ll<i;ll++){
                System.out.print("*");
            }

            System.out.println();

        }

    }

}*/

/*Q7
*************************************************************************
public class thathastuscholarnovcohort {
    public static void main(String[] args) {

        Scanner sc=new Scanner(System.in);
        String kk=sc.nextLine();
        StringBuilder sb=new StringBuilder(kk);

        for(int i=0;i<kk.length()/2;i++){
            int g=i;
            int h=kk.length()-i-1;
            char frontm=sb.charAt(i);
            char backn=sb.charAt(sb.length()-i-1);
            sb.setCharAt(g,backn);
            sb.setCharAt(h,frontm);


        }
        System.out.println(sb);
    }

    }
*/
/* Q8
***********************************************************************
public class thathastuscholarnovcohort {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter size of array");
        int n=sc.nextInt();
        int [] arr=new int[n];
        int [] arr1=new int[n];
        System.out.println("Now enter all elements of array via line separated");
        for(int i=0;i<arr.length;i++){
            arr[i]=sc.nextInt();
        }
        for(int i=0;i<arr.length;i++){
            arr1[i]=arr[arr.length-i-1];

        }
boolean hh=true;
        for(int i=0;i<arr.length;i++){
            if(arr1[i]!=arr[i]){
                hh=false;
                break;
            }
        }
        if(hh){
            System.out.println("yes it's mirror inverse");
        }
    else{
            System.out.println("no it's not mirror inverse");
        }

    }
}
 */
/* Q9
*******************************************************************
import java.util.ArrayList;
import java.util.Collection;
import java.util.Scanner;
public class thathastuscholarnovcohort {
    public static void main(String[] args) {
        ArrayList<Integer> hh= new ArrayList<Integer>();
        Scanner sc=new Scanner(System.in);
        System.out.println("enter 10 number of your choice which you want to be add in the array list");
        int [] arr=new int [10];
        for(int i=0;i<arr.length;i++){
            arr[i]=sc.nextInt();
        }
        for(int i=0;i<arr.length;i++){
            hh.add(arr[i]);
        }
        System.out.println(hh);
        System.out.println("Now enter the index of particular element which you want to remove from the arraylist");
int j=sc.nextInt();
hh.remove(j);
        System.out.println("New arraylist will be  "+hh);
    }


    }*/
/*Q10
***********************************************************************
public class thathastuscholarnovcohort {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int m=sc.nextInt();
        int [][] arr=new int[n][m];
        for(int i=0;i<n;i++){
            for(int j=0;j<m;j++){
                arr[i][j]=sc.nextInt();
            }
        }
        for(int i=0;i<m;i++){
            for(int j=0;j<n;j++){
                System.out.print(arr[j][i]+" ");
            }
            System.out.println();

        }


    }
}*/
