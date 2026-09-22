<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Recurse on the first argument for [addition](../../../../../addition.md) and [multiplication](../../../../../multiplication.md), and on the exponent for [exponentiation](../../../../../exponentiation.md):

```
add :: Natural -> Natural -> Natural
add Zero     n = n
add (Succ m) n = Succ (add m n)

mul :: Natural -> Natural -> Natural
mul Zero     n = Zero
mul (Succ m) n = add n (mul m n)

power :: Natural -> Natural -> Natural
power m Zero     = Succ Zero
power m (Succ n) = mul m (power m n)
```

The defining arithmetic identities are

$$
\boxed{0+n=n,\quad(m+1)+n=1+(m+n),\quad0n=0,\quad(m+1)n=n+mn,\quad m^0=1,\quad m^{n+1}=m\,m^n.}
$$

Each recursive call consumes one constructor. The base of [exponentiation](../../../../../exponentiation.md) makes `power Zero Zero` equal to one, the empty-product convention. Applying `convert` and using [structural induction](../../../../../structural-induction.md) verifies all three operations.

## ↑ Ancestors (12)

1. [B](../b.md)
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
