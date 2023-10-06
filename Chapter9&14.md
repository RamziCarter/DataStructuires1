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



---
## Chapter 14

Recurrence relations

> Deriving a recurrence relation from a list

```Java
public void countDown(int n)
{
  System.out.println(n);
  if (n > 1)
  {
    countDown(n - 1);
  }
}
```

t(n) = time required for n
t(1) = 1 due to the if 
t(n) = 1 + t(n - 1)


> Solving the recurrence relation
We start by listing the first four times
t(1) = 1
t(2) = 1 + t(2 - 1) = 1 + 1 = 2
t(3) = 1 + t(3 - 1) = 1 + t(2) = 3 
t(4) = 1 + t(4 - 1) = 1 + t(3) = 4

t(n) = n ----> closed form 

__verifying the pattern:__
* you know that t(1) = 1
* t(n) = 1 + (n - 1)
* Need to show t(n) = n for every choice of n
* assume t(n) = n
  * we have to prove t(n + 1) = n + 1
  * t(n + 1) = 1 + t(n)
  * = 1 + n
    * done 
Another example of the recurrence relation
* a truly sneak y way to evaluate x^n is by recursion
* the hardware does something similar to this for division
* If n is an even number, then x^n = 
