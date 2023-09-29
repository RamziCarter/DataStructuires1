Recursion

- a method that calls itself
- turn the problem into a smaller version of the same problem
- then ytou call the same method to complete the solution
- you also need a base case or base cases so the recursion stops

The stack

- when a method calls itself, all its data must be saved 

```Java
public int factorial(int n)
{
  
  if (n == 1)
  {
    return 1;
  }

  return n * factorial(n - 1);

}


fibbionacci (int n)
{
  if(n <= 2)
    return 1;
  return fibonacci(n-1) + fibonacci(n-2);
}

public void moveDisks(int n, int startPole, int endPole, int sparePole)
{
  
}
```
