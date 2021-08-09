# Codes
This consists of the various codes right from basic I've learnt throughout my life in various languages.

Here I have a code to a guessing game that I made(JAVA)

import java.util.*;
public class Game
{int n;
 int s;
 int i;
public Game()
{n=0;
 s=8; 
i=1;
}    
public void Welcome()    
{System.out.println("\t\tWelcome to Bryan's Guessing game");  
 System.out.println();
 System.out.println("Try out your luck by guessing the secret number");
 System.out.println();
 System.out.println("You have 3 chances"); 
 System.out.println();
}
public void Input()
{Scanner sc=new Scanner(System.in);
 while(i<=3)
 {i++;
  System.out.print("Guess: ");
  n=sc.nextInt();
  if(n==s)
  {System.out.println("Congratulations You Won!!");
   break;}
  else System.out.println("Try again "); }}
   
 public void main()
 {Game G=new Game();
    G.Welcome();
    G.Input();}}
  
    
 
