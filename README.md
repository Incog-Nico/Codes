recursive functions

fact(int n)
{
if(n==0)
return 1;
return n*fact(n-1);
}

fib(int n)
{
if(n==1)
return 0;
else if(n==2)
return 1;
return fib(n-1)+fib(n-2);
}

sum of digits(int n)
{
return (n%10)+sod(n/10);
}
