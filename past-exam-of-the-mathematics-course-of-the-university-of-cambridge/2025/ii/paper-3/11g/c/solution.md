<h1 id="11g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

From part (b), $a_{2m+1}=3$ and $a_{2m+2}=6$. Eliminating the intervening odd-indexed convergent from the standard recurrence shows that either sequence $x_m=p_{2m}$ or $x_m=q_{2m}$ obeys

$$
x_{m+2}=20x_{m+1}-x_m.
$$

The initial even convergents are

$$
\frac{p_0}{q_0}=\frac31,
\qquad
\frac{p_2}{q_2}=\frac{63}{19}.
$$

Put $u=10+3\sqrt{11}$. Since $N(u)=100-99=1$ and $u+u^{-1}=20$, the sequence

$$
w_m=(3+\sqrt{11})u^m
$$

satisfies the same recurrence. Its first two values are $3+\sqrt{11}$ and $63+19\sqrt{11}$, so

$$
p_{2m}+q_{2m}\sqrt{11}=(3+\sqrt{11})(10+3\sqrt{11})^m.
$$

Taking norms in $\mathbb Q(\sqrt{11})$ yields

$$
p_{2m}^2-11q_{2m}^2
=(9-11)(100-99)^m
=\boxed{-2}.
$$

This applies in particular whenever the original index $n=2m\geq2$ is even.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11G](../../11g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
