<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $q=1-p$. The count has the zero-based [geometric distribution](../../../../../../geometric-distribution.md), whose [probability generating function](../../../../../../probability-generating-function.md) is $G_N(z)=p/(1-qz)$. Hence the aggregate has a [compound geometric distribution](../../../../../../compound-geometric-distribution.md), with

$$
\boxed{\kappa_S(t)=\log p-\log\bigl(1-qM_{X_1}(t)\bigr).}
$$

This transform requires $qM_{X_1}(t)<1$; it holds for every $t\le0$. To differentiate explicitly, let $g(t)=M_{X_1}(t)$. Then

$$
\kappa_S'(t)=\frac{qg'}{1-qg},\qquad \kappa_S''(t)=\frac{qg''}{1-qg}+\frac{q^2(g')^2}{(1-qg)^2},
$$

and

$$
\kappa_S'''(t)=\frac{qg'''}{1-qg}+\frac{3q^2g'g''}{(1-qg)^2}+\frac{2q^3(g')^3}{(1-qg)^3}.
$$

At zero, $g=1$ and $g^{(j)}=m_j$, giving

$$
\boxed{\kappa_{S,3}=\frac qp m_3+\frac{3q^2}{p^2}m_1m_2+\frac{2q^3}{p^3}m_1^3.}
$$

Every term is positive for $0<p<1$ and strictly positive claim sizes. Therefore **the unstandardized skewness is positive**, even if the claim-size third [central moment](../../../../../../central-moment.md) itself is negative. The zero-based convention matters: there is no factor $M_{X_1}(t)$ in the numerator of this aggregate transform.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
