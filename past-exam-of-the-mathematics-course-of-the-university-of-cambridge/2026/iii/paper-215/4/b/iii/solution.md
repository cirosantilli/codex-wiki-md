<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Give the state graph the unit-edge [path metric](../../../../../../../path-metric.md). The construction in part (i) shows that its diameter is at most $2s$. It remains to couple one step from neighbouring states $X=A\cup\{x\}$ and $Y=A\cup\{y\}$.

Pair the choice $x$ in the first chain with $y$ in the second, and pair every $a\in A$ with itself; use the same proposed vertex $v$ in both chains. When the pair $(x,y)$ is removed, the chains coalesce whenever $v$ is not in the closed neighbourhood of $A$. This has probability at least

$$
C=\frac{n-(s-1)(\Delta+1)}{sn}.
$$

When a common $a\in A$ is removed, the distance can increase from one to at most two only if $v$ lies in one of the closed neighbourhoods of $x$ and $y$, an event of probability at most

$$
B=\frac{2(\Delta+1)}n.
$$

Therefore

$$
\mathbb E[\rho(X_1,Y_1)]
\leq1-C+B
\leq1-\frac1{sn},
$$

where the last inequality uses $n\geq3s(\Delta+1)$. The [Path coupling theorem](../../../../../../../path-coupling-theorem.md) extends this contraction to arbitrary starting distributions. Since $1-1/(sn)\leq e^{-1/(sn)}$, part (a) with diameter at most $2s$ yields

$$
\boxed{t_{\mathrm{mix}}(\varepsilon)
\leq sn\log\frac{2s}{\varepsilon}
\lesssim sn\log(s/\varepsilon).}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 215](../../../../paper-215-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
