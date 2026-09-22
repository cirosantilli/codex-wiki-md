<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [Oberon](../../../../../oberon-programming-language.md) [recursive procedure](../../../../../recursive-procedure.md) can implement the defining [recurrence relation](../../../../../recurrence-relation.md) directly. Its [precondition](../../../../../precondition.md) is $n\geq1$; arithmetic is assumed to remain in the representable [integer](../../../../../integer-split.md) range.

```
PROCEDURE Fib(n: INTEGER): INTEGER;
  VAR result: INTEGER;
BEGIN
  IF n <= 2 THEN
    result := 1
  ELSE
    result := Fib(n-1) + Fib(n-2)
  END;
  RETURN result
END Fib;
```

Correctness follows by [strong induction](../../../../../strong-induction.md): the two base inputs give $1$, and for $n>2$ the returned sum is $F_{n-1}+F_{n-2}=F_n$. On each recursive branch the positive [integer](../../../../../integer-split.md) argument strictly decreases, while recursion stops at $1$ or $2$. The [well-ordering principle](../../../../../well-ordering-principle-for-the-natural-numbers.md) therefore proves [algorithm termination](../../../../../algorithm-termination.md).

$$
\boxed{\operatorname{Fib}(n)=F_n\quad(n\geq1).}
$$

The method repeats many subproblems and has exponential [time complexity](../../../../../time-complexity.md); termination alone does not make it efficient.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
