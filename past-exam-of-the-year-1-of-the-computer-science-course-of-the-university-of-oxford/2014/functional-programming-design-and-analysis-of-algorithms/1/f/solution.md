<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let $T(n)=(F_n,F_{n+1})$. The equations derived in part (e) become $T(0)=(0,1)$ and $T(n+1)=s(T(n))$, where $s(a,b)=(b,a+b)$. Replacing zero and successor by that seed and step is exactly a [natural-number fold](../../../../../natural-number-fold.md):

```
twoFibsNat :: Natural -> (Integer, Integer)
twoFibsNat = foldNat step (0, 1)
  where
    step :: (Integer, Integer) -> (Integer, Integer)
    step (a, b) = (b, a + b)

fibNat :: Natural -> Integer
fibNat = fst . twoFibsNat
```

Consequently

$$
\boxed{\operatorname{fibNat}=\operatorname{fst}\circ\operatorname{foldNat}\bigl((a,b)\mapsto(b,a+b)\bigr)(0,1).}
$$

[Structural induction](../../../../../structural-induction.md) follows the constructors of `Natural`: the seed gives the first two [Fibonacci numbers](../../../../../fibonacci-number.md), and the successor step uses the [Fibonacci recurrence](../../../../../fibonacci-recurrence.md). The extra component carries exactly the information needed for the next update.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
