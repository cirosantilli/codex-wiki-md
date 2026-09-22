<h1 id="algebra/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $p(t)=\prod_{j=1}^m(t-\mu_j)$ and define the [Lagrange interpolation polynomials](../../../../lagrange-polynomial.md)

$$
\ell_j(t)=\prod_{k\ne j}\frac{t-\mu_k}{\mu_j-\mu_k}.
$$

Their denominators are nonzero and $\ell_j(\mu_i)=\delta_{ij}$. The [polynomial](../../../../polynomial-split.md) $\sum_j\ell_j-1$ has degree at most $m-1$ and vanishes at all $m$ distinct [scalars](../../../../scalar.md), so it is zero. Suppose condition (a) holds, and put $E_j=\ell_j(T)$. Since $(t-\mu_j)\ell_j(t)$ is a constant multiple of $p(t)$,

$$
(T-\mu_jI)E_j=0,\qquad\sum_jE_j=I.
$$

Thus each $E_jv$ lies in $V_j$, and every [vector](../../../../vector.md) is a sum of such [vectors](../../../../vector.md). If $\sum_jv_j=0$ with $v_j\in V_j$, applying $E_i$ gives $v_i=0$, because $\ell_i(T)v_j=\ell_i(\mu_j)v_j$. Hence the sum is direct, proving (b). Conversely, on each $V_j$ the factor $T-\mu_jI$ vanishes; the factors commute, so $p(T)$ vanishes on every summand and therefore on $V$. This proves the equivalence **without invoking primary decomposition**.

If $ST=TS$ and $v\in V_j$, then $(T-\mu_jI)Sv=S(T-\mu_jI)v=0$, so $S[V_j]\subseteq V_j$. Conversely, if each summand is preserved, then on $V_j$ both $ST$ and $TS$ act as $\mu_jS$. They agree on all summands and hence on $V$. Therefore

$$
\boxed{ST=TS\iff S[V_j]\subseteq V_j\text{ for every }j.}
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Algebra](../../algebra.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
