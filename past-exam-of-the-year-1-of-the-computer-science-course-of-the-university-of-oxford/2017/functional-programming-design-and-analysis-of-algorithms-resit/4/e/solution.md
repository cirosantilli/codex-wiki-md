<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Store two consecutive [Fibonacci numbers](../../../../../fibonacci-number.md) as the state:

```
fibs :: [Integer]
fibs = unfold (const False) fst step (0,1)
  where
    step (a,b) = (b,a+b)
```

The invariant is that the state is $(F_n,F_{n+1})$, with $F_0=0,F_1=1$. Emitting its first component and updating the pair therefore produces **$0,1,1,2,3,5,8,\ldots$**. `Integer` avoids fixed-width overflow; the bit cost of adding increasingly large integers is separate from the number of unfold steps.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
