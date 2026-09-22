<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The derivative fixed-point equation is unsuitable as an executable definition: requesting its first coefficient asks for the second coefficient of the same stream, then the third, indefinitely. It is not [productive](../../../../../stream-productivity.md). As an algebraic equation it is also missing the constant coefficient: every scalar multiple of the [formal power series exponential](../../../../../formal-power-series-exponential.md), including zero, satisfies it.

The integral equation gives the useful definition:

```
expx :: Fractional a => [a]
expx = plus one (integral expx)
```

The initial coefficient is available as `1 + 0`; each subsequent coefficient needs only a previously determined coefficient. The [recurrence relation](../../../../../recurrence-relation.md) is $a_0=1$ and $a_{n+1}=a_n/(n+1)$, so **$a_n=1/n!$**. This proves both uniqueness of the formal solution and [productivity](../../../../../stream-productivity.md) of every finite coefficient [list prefix](../../../../../prefix-of-a-list.md).

## ↑ Ancestors (12)

1. [G](../g.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
