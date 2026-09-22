<h1 id="38c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Insert the [Fourier mode](../../../../../../fourier-mode.md) $u_m^n=g^ne^{im\theta}$ into the [leapfrog advection scheme](../../../../../../leapfrog-advection-scheme.md). The amplification roots satisfy

$$
g^2-2i\mu\sin\theta\,g-1=0,\qquad g_\pm=i\mu\sin\theta\pm\sqrt{1-\mu^2\sin^2\theta}.
$$

For $0<\mu<1$, both roots have modulus one and remain uniformly separated by at least $2\sqrt{1-\mu^2}$. The two-level Fourier amplification matrices are therefore uniformly diagonalizable, and their powers stay bounded. The [Parseval identity](../../../../../../parseval-identity.md) gives stability in the discrete two-norm. For $\mu>1$, some frequencies have $|\mu\sin\theta|>1$ and one root has modulus greater than one, giving instability.

For [two-level stability at the leapfrog Courant boundary](../../../../../../two-level-stability-at-the-leapfrog-courant-boundary.md), at $\mu=1$ and $\theta=\pi/2$, the repeated root is $i$ and the recurrence has solutions $a_n=(A+Bn)i^n$. For example $a_0=0,a_1=1$ gives $a_n=ni^{n-1}$. Thus arbitrary two-level perturbations grow without a uniform power bound. The precise answer for unrestricted starting data is

$$
\boxed{0<\mu<1\text{ is stable};\quad\mu>1\text{ is unstable};\quad\mu=1\text{ is a repeated-root boundary case}.}
$$

The often-used root-modulus CFL condition is $\mu\le1$, but by itself it misses this boundary Jordan growth. A startup that selects the exact translating branch at $\mu=1$ removes that growth for the selected data; it does not make the unrestricted two-level update power-bounded.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38C](../../38c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
