<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

The standard name is the [Reed-Muller code](../../../../../reed-muller-code.md). For $0\leq d\leq m$, evaluate all multilinear [polynomials](../../../../../polynomial-split.md) over $\mathbb F_2$ of total degree at most $d$ at every point of $\mathbb F_2^m$. These evaluation vectors form $RM(m,d)$, of length $2^m$. Distinct multilinear [polynomials](../../../../../polynomial-split.md) have distinct evaluations: induct on the variables using $f=g+x_mh$ and the two restrictions $g,g+h$. Thus the monomials of degree at most $d$ are independent and

$$
\boxed{\dim RM(m,d)=\sum_{j=0}^d\binom mj,\qquad R=2^{-m}\sum_{j=0}^d\binom mj.}
$$

For minimum weight, use the same splitting. A nonzero $h$ has weight at least $2^{m-d}$ by induction, and $\operatorname{wt}(g)+\operatorname{wt}(g+h)\geq\operatorname{wt}(h)$. If $h=0$, the two identical halves give the same lower bound by induction on $g$. The endpoint $d=m$ has minimum weight one, and $d=0$ is the repetition code. A product of $d$ distinct variables has exactly $2^{m-d}$ nonzero evaluations, so

$$
\boxed{d_{\min}=\operatorname{wt}_{\min}=2^{m-d}.}
$$

Here distance equals minimum nonzero weight because the code is linear.

Every monomial of degree at most $d-1$ in $d$ variables has an even number of ones, and parity is additive over $\mathbb F_2$. Thus every word of $RM(d,d-1)$ has even weight. If $x\in RM(m,r)$ and $y\in RM(m,m-r-1)$, their coordinatewise product is an evaluation of degree at most $m-1$, even after reducing $X_i^2=X_i$. Its weight is therefore even, so $\langle x,y\rangle=0$. This proves the asserted inclusion in the [dual code](../../../../../dual-code.md). Finally

$$
\sum_{j=0}^{m-r-1}\binom mj=2^m-\sum_{j=0}^r\binom mj,
$$

by binomial symmetry. The dimensions agree with that of the [orthogonal](../../../../../orthogonal-vectors.md) complement, proving **$RM(m,r)^\perp=RM(m,m-r-1)$** for $0\leq r<m$.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
