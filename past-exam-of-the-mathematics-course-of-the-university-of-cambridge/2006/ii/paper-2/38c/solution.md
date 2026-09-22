<h1 id="38c/solution">Solution</h1>

↑ **Parent:** [38C](../38c.md)

Assume the consistency regularity implicit in the requested rate, for example $u\in C^4$ on the closed square. Bounded fourth derivatives and [Taylor's theorem](../../../../../taylor-theorem.md) give a uniform residual $\tau_{ij}=\Delta_hu(ih,jh)-f(ih,jh)$ with $|\tau_{ij}|\le C_0h^2$. Subtracting the exact grid values from the numerical equations gives $\Delta_he=-\tau$, with zero boundary error.

Let $A=-h^2\Delta_h$ be the unscaled positive Dirichlet matrix. Its [eigenvectors](../../../../../eigenvector.md) are products of discrete sine vectors, which form an [orthogonal basis](../../../../../orthogonal-basis.md); direct substitution gives [eigenvalues](../../../../../eigenvalue.md)

$$
\lambda_{pq}=4\sin^2\frac{p\pi h}{2}+4\sin^2\frac{q\pi h}{2}\quad(1\le p,q\le M).
$$

Since $\sin(\pi h/2)\ge h$ for $0<h\le1$, $\lambda_{11}\ge8h^2$. Therefore $\|A^{-1}\|_2\le1/(8h^2)$. The error equation is $Ae=h^2\tau$, and its residual has [norm](../../../../../norm.md) $\|\tau\|_2\le MC_0h^2\le C_0h$. Combining the bounds yields

$$
\boxed{\left(\sum_{i,j=1}^M|e_{ij}|^2\right)^{1/2}\le\frac{C_0}{8}h.}
$$

This is the [unweighted grid error for the five-point Poisson formula](../../../../../unweighted-grid-error-for-the-five-point-poisson-formula.md). The unweighted [norm](../../../../../norm.md) loses one power of $h$ because the grid has order $h^{-2}$ points; the area-weighted [norm](../../../../../norm.md) is second-order accurate. A regularity assumption is needed for the uniform truncation estimate and hence for this rate; the question does not specify it explicitly.

## ↑ Ancestors (10)

1. [38C](../38c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
