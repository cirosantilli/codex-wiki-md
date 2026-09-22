<h1 id="20h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $T_k$ be the expected capture time starting from $D_0=k$, so $T_0=0$. The [Strong Markov property](../../../../../../strong-markov-property.md) at successive first passages to lower levels and part (a) give

$$
T_k=T_1+(k-1)\mu,
\qquad k\ge1.
$$

At $D_n=1$, the next state is zero with probability $r/2$, one with probability $1/2$, and two with probability $(1-r)/2$. [First-step analysis](../../../../../../first-step-analysis.md) therefore gives

$$
T_1=1+\frac12T_1+\frac{1-r}{2}T_2,
$$

or

$$
T_1=2+(1-r)(T_1+\mu).
$$

Solving,

$$
T_1=\frac2r+\left(\frac1r-1\right)\mu.
$$

Substituting $\mu=2/(2q-1)$ now yields

$$
\boxed{
T_m=\frac2r+\left(m+\frac1r-2\right)\frac2{2q-1}},
$$

which is the required expected capture time.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20H](../../20h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
