<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $\tau\in\mathbb H$ and let $\Lambda=\mathbb Z+\mathbb Z\tau$. We use the binary convention for the [theta function with characteristics](../../../../../../theta-function-with-characteristics.md) in the PDF. Its nonzero exponential prefactor does not change the zeros of the translated $\vartheta_{00}$. The four characteristic functions are entire in $z$, by normal convergence of their Gaussian series.

We first prove their zero information, rather than assume that the quotient has no poles. Pair the terms with indices $n$ and $-n-1$ to get

$$
\vartheta_{00}\!\left(\frac{1+\tau}2,\tau\right)=\sum_{n\in\mathbb Z}(-1)^nq^{n(n+1)/2}=0.
$$

The logarithmic derivative $D(z)=\vartheta_{00}'(z)/\vartheta_{00}(z)$ is periodic under $z\mapsto z+1$ and satisfies $D(z+\tau)=D(z)-2\pi i$, by the spatial transformation formulas. Choose a fundamental parallelogram with zero-free boundary. Its vertical-side integrals cancel, and subtracting the top horizontal integral from the bottom one gives $2\pi i$. The [argument principle](../../../../../../argument-principle.md) therefore counts exactly one zero inside, with multiplicity. Thus the displayed zero is simple and is the unique one modulo $\Lambda$. The [zeros of theta functions with characteristics](../../../../../../zeros-of-theta-functions-with-characteristics.md) are consequently

$$
\begin{array}{c|cccc}
\text{function}&\vartheta_{00}&\vartheta_{01}&\vartheta_{10}&\vartheta_{11}\\\hline
\text{zero modulo }\Lambda&(1+\tau)/2&\tau/2&1/2&0.
\end{array}
$$

All are simple. In particular the three even theta constants are nonzero and $\vartheta_{11}'(0)\ne0$.

Let $R(z)$ be the product of these four functions divided by $\vartheta_{11}(2z)$. The denominator's simple zeros occur exactly at the four half-periods modulo $\Lambda$, and each is cancelled by the corresponding simple numerator zero. Hence $R$ extends to an [entire function](../../../../../../entire-function.md). Under $z\mapsto z+1$, the four numerator signs multiply to one, as do the two successive shifts of the denominator. Under $z\mapsto z+\tau$, the numerator has multiplier $q^{-2}t^{-4}$, where $t=e^{2\pi iz}$; the denominator, whose argument shifts by $2\tau$, has the same multiplier. Thus $R$ is an entire [elliptic function](../../../../../../elliptic-function.md) with periods $1,\tau$. It is bounded on a fundamental parallelogram and hence on the plane, so [Liouville's theorem](../../../../../../liouville-theorem.md) makes it constant.

At $z=0$, the simple odd zero gives $\vartheta_{11}(z)/\vartheta_{11}(2z)\to1/2$. Therefore the [Jacobi theta duplication identity](../../../../../../jacobi-theta-duplication-identity.md) is

$$
\boxed{R(z)=\frac12\vartheta_{00}(0,\tau)\vartheta_{01}(0,\tau)\vartheta_{10}(0,\tau).}
$$

At a zero of the displayed denominator, this is interpreted by removable continuation. Equivalently, multiply through by the denominator to obtain an entire product identity valid for every $z$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
