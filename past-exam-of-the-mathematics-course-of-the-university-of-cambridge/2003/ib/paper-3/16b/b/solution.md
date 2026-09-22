<h1 id="16b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiating the Rodrigues representation directly gives the identity

$$
H_{n+1}=2xH_n-H_n'.
$$

We prove simultaneously by [induction](../../../../../../mathematical-induction.md) that $H_n'=2nH_{n-1}$ for $n\geq1$. It holds for $H_0=1$, $H_1=2x$. Suppose it holds at $n$. Differentiating the preceding identity and using the same identity at $n-1$ gives

$$
\begin{aligned}
H_{n+1}'&=2H_n+2xH_n'-H_n''\\
&=2H_n+4nxH_{n-1}-2nH_{n-1}'\\
&=2H_n+4nxH_{n-1}-2n(2xH_{n-1}-H_n)=2(n+1)H_n.
\end{aligned}
$$

The induction is complete. Substituting the derivative identity into the first formula proves the [Hermite polynomial](../../../../../../hermite-polynomial.md) three-term [recurrence relation](../../../../../../recurrence-relation.md)

$$
\boxed{H_{n+1}(x)=2xH_n(x)-2nH_{n-1}(x)\quad(n\geq1).}
$$

The initial step $H_1=2xH_0$ supplies the recurrence at $n=0$ without needing to define $H_{-1}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16B](../../16b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
