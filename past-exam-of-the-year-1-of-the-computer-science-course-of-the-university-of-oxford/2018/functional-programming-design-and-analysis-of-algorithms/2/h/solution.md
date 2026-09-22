<h1 id="2/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

The derivative relations and initial values give $S'=C$, $S(0)=0$, $C'=-S$ and $C(0)=1$. Integrating from zero yields $S=\int_0^x C$ and $C=1-\int_0^x S$. Thus use mutually recursive [lazy lists](../../../../../lazy-list.md):

```
sinx, cosx :: Fractional a => [a]
sinx = integral cosx
cosx = minus one (integral sinx)
```

Both heads are available immediately, and later coefficients depend on earlier coefficients of the other stream. The resulting [formal power series](../../../../../formal-power-series.md) are **$S=x-x^3/3!+x^5/5!-\cdots$** and **$C=1-x^2/2!+x^4/4!-\cdots$**. Their zero coefficients and alternating signs follow directly from the coupled [recurrence relations](../../../../../recurrence-relation.md), providing a coefficientwise proof without assumptions about analytic [convergence](../../../../../convergence.md).

## ↑ Ancestors (12)

1. [H](../h.md)
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
