<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use just the parameters $1$ and $-1$. Positivity and adaptation of their local [martingales](../../../../../../martingale-split.md) give

$$
X_t=\tfrac12(\log Z_t^{(1)}-\log Z_t^{(-1)}),\qquad A_t=-\log Z_t^{(1)}-\log Z_t^{(-1)}.
$$

Thus both processes are adapted. A positive continuous local [martingale](../../../../../../martingale-split.md) has a [semimartingale](../../../../../../semimartingale.md) logarithm, by [Itô formula](../../../../../../ito-s-lemma.md) after localization away from zero. Since $X=\log Z^{(1)}+A/2$ and $A$ has [finite variation](../../../../../../total-variation-of-a-function.md), $X$ is a [continuous semimartingale](../../../../../../continuous-semimartingale.md). Write $X=N+V$, where $N$ is a zero-starting [continuous local martingale](../../../../../../continuous-local-martingale.md) and $V$ is continuous [finite variation](../../../../../../total-variation-of-a-function.md), also starting from zero.

Apply [Itô formula](../../../../../../ito-s-lemma.md) to each exponential:

$$
dZ^{(\theta)}=\theta Z^{(\theta)}\,dN+Z^{(\theta)}\left(\theta\,dV+\tfrac12\theta^2(d[N]-dA)\right).
$$

Because $Z^{(\theta)}$ is itself a local [martingale](../../../../../../martingale-split.md), the finite-variation term is zero by part (a). Divide its finite signed measure by the strictly positive $Z^{(\theta)}$. For $\theta=1,-1$, respectively,

$$
dV+\tfrac12(d[N]-dA)=0,\qquad -dV+\tfrac12(d[N]-dA)=0.
$$

Adding and subtracting show $V=0$ and $[N]=A$. Therefore the [exponential criterion for a continuous local martingale and its bracket](../../../../../../exponential-criterion-for-a-continuous-local-martingale-and-its-bracket.md) gives

$$
\boxed{X\text{ is a continuous local martingale},\qquad [X]=A\text{ indistinguishably}.}
$$

The [semimartingale](../../../../../../semimartingale.md) property was established before applying Itô's formula to $X$; it was not assumed from the outset.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
