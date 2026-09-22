<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $H_n=\sum_{k=0}^{\lfloor n/2\rfloor}\binom{n-k}{k}$; the other summands in the printed sum vanish. The initial values are $H_0=1=F_1$ and $H_1=1=F_2$. For $n\geq2$, [Pascal's identity](../../../../../pascal-s-rule.md) gives

$$
H_n=\sum_{k=0}^{\lfloor n/2\rfloor}\binom{n-1-k}{k}
+\sum_{k=1}^{\lfloor n/2\rfloor}\binom{n-1-k}{k-1}
=H_{n-1}+H_{n-2}.
$$

For the first sum, when $n$ is even its final term is zero; otherwise its range already agrees with $H_{n-1}$. In the second sum put $j=k-1$, obtaining $\binom{n-2-j}{j}$ for $0\leq j\leq\lfloor(n-2)/2\rfloor$. Thus both range identifications hold without negative upper arguments in a [binomial coefficient](../../../../../binomial-coefficient-split.md).

Now [strong induction](../../../../../strong-induction.md) gives $H_n=F_n+F_{n-1}=F_{n+1}$ from the two preceding cases and the [Fibonacci recurrence](../../../../../fibonacci-recurrence.md). Hence

$$
\boxed{\sum_{k=0}^n\binom{n-k}{k}=F_{n+1}\quad(n\geq0).}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
