<h1 id="14g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

After choosing a basis of $V$, a linear [endomorphism](../../../../../../endomorphism.md) is specified by an $n$ by $n$ matrix, with $n^2$ freely chosen coefficients. Therefore

$$
\boxed{\dim\operatorname{End}(V)=n^2}.
$$

The $n^2+1$ [endomorphisms](../../../../../../endomorphism.md) $I,\alpha,\ldots,\alpha^{n^2}$ are linearly dependent. Some nonzero coefficient list gives a nonzero [polynomial](../../../../../../polynomial-split.md) $p$ satisfying $p(\alpha)=0$.

For nonzero $V$, the [minimal polynomial](../../../../../../minimal-polynomial.md) $m_\alpha$ is the monic [polynomial](../../../../../../polynomial-split.md) of least degree annihilating $\alpha$. It is unique: subtracting two monic least-degree choices would give a lower-degree annihilator. More generally division of any annihilator $p$ by $m_\alpha$ gives $p=qm_\alpha+r$, with $\deg r<\deg m_\alpha$, and evaluation implies $r(\alpha)=0$. Minimality forces $r=0$, so every annihilator is divisible by $m_\alpha$. If $V=\{0\}$, the convention $m_\alpha=1$ handles the degenerate case.

The arguments work over the underlying scalar field. In part (b), roots in that field correspond to [eigenvalues](../../../../../../eigenvalue.md) there; to discuss other roots one extends scalars, for example by complexifying a real [vector space](../../../../../../vector-space-split.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14G](../../14g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
