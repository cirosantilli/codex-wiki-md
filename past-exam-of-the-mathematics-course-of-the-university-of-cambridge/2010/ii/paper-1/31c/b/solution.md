<h1 id="31c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix an integer $N\geq0$ and write

$$
f(x)=\sum_{j=0}^Na_jx^{\alpha+j\beta}+r_N(x),\qquad
r_N(x)=o(x^{\alpha+N\beta}).
$$

For each power, substitute $y=\lambda x$ and extend the upper limit to infinity; the discarded tail is exponentially small. Since $\alpha+j\beta>-1$, the [Gamma integral](../../../../../../gamma-integral.md) gives

$$
\int_0^\infty x^{\alpha+j\beta}e^{-\lambda x}\,dx
=\Gamma(\alpha+j\beta+1)\lambda^{-\alpha-j\beta-1}.
$$

To control the remainder, choose $\delta>0$ such that $|r_N(x)|\leq\epsilon x^{\alpha+N\beta}$ for $0<x<\delta$. Its integral there is at most $\epsilon\Gamma(\alpha+N\beta+1)\lambda^{-\alpha-N\beta-1}$. On $[\delta,b]$ the remainder is bounded and its integral is $O(e^{-\lambda\delta})$. Since $\epsilon$ is arbitrary, we have the full [Watson lemma](../../../../../../watson-s-lemma.md) expansion

$$
\boxed{I(\lambda)\sim\sum_{j=0}^\infty
\frac{a_j\Gamma(\alpha+j\beta+1)}{\lambda^{\alpha+j\beta+1}}.}
$$

More precisely, after the term $j=N$, the remainder is $o(\lambda^{-\alpha-N\beta-1})$. This proof uses neither differentiability of $f$ nor convergence of its asymptotic series.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [31C](../../31c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
