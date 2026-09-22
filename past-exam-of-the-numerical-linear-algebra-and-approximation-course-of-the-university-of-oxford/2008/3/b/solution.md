<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Map $[a,b]$ to $[-1,1]$ by $z(r)=(2r-a-b)/(b-a)$. Since $a>0$, the normalization point $z(0)=-(a+b)/(b-a)$ lies outside that interval. The proposed [Chebyshev polynomial](../../../../chebyshev-polynomial.md) ratio has degree $k$ and equals one at zero. On the spectral interval its maximum absolute value is

$$
\boxed{\frac{|T_k(1)|}{|T_k(-(a+b)/(b-a))|}.}
$$

The [Chebyshev minimax polynomial with exterior normalization](../../../../chebyshev-minimax-polynomial-with-exterior-normalization.md) minimizes this maximum among degree-at-most-$k$ polynomials with $p(0)=1$. One may quote the minimax property. Its reason is the alternating $k+1$ extremal values: a strictly better competitor would force their difference to have at least $k$ roots in $[a,b]$ and the additional root at zero outside it, impossible for degree at most $k$.

The paper uses a monic normalization of $T_k$ for $k\geq1$, rather than the usual $T_k(1)=1$ convention. The common factor cancels in the ratio. With $\kappa=b/a>1$ and $q=(\sqrt\kappa-1)/(\sqrt\kappa+1)$, the hyperbolic-cosine formula gives the error factor $\boxed{2q^k/(1+q^{2k})\leq2q^k}$. This tends rapidly to zero when the spectral interval is well-conditioned. If $a=b$, use $p(r)=1-r/a$ for exact one-step termination instead of the displayed interval map.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the numerical linear algebra and approximation course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and approximation course of the University of Oxford](../../../../numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
