<h1 id="8/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

At the smaller [indicial root](../../../../../indicial-root.md) $\sigma=1/2$, the $k=1$ equation is $0=0$: it leaves $a_1$ free. For $k\geq2$, the valid recurrence is

$$
a_k=-\frac{k-1}{k}a_{k-1}.
$$

Choosing $a_1=0$ makes every later coefficient zero. The resulting [terminating Frobenius series](../../../../../terminating-frobenius-series.md) is therefore

$$
\boxed{y(x)=a_0\sqrt{x}.}
$$

Substitution gives $y'=a_0/(2\sqrt{x})$ and $y''=-a_0/(4x^{3/2})$; the three terms in the equation sum to $a_0\sqrt{x}[-(1+x)-2+(x+3)]=0$.

Termination is a permitted choice, not a condition forced on every smaller-root solution. Retaining the free $a_1$ adds the solution in part (e), so the general real solution on $x>0$ is $\boxed{y=\sqrt{x}[C_1+C_2\log(1+x)]}$. This is exactly the freedom explained by [undetermined coefficient at Frobenius resonance](../../../../../undetermined-coefficient-at-frobenius-resonance.md). On either negative interval avoiding $-1$ and $0$, analogous real formulas use $\sqrt{|x|}$ and $\log|1+x|$.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
