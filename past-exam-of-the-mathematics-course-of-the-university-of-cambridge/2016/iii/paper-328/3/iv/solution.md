<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Label the sides by $L,R,B,T$, and parametrize the two vertical sides by $s=y\in[-1,1]$, the horizontal sides by $s=x\in[-1,1]$. Their outward [normal derivatives](../../../../../../normal-derivative.md) are $q_L=-u_x(-1,s)$, $q_R=u_x(1,s)$, $q_B=-u_y(s,-1)$ and $q_T=u_y(s,1)$. Let $f_j$ denote the prescribed side values. Assume compatible, sufficiently regular boundary traces; the square's corners have zero arclength measure and do not require separate normal values.

For [sine collocation of square modified Helmholtz global relations](../../../../../../sine-collocation-of-square-modified-helmholtz-global-relations.md), use [Legendre polynomials](../../../../../../legendre-polynomial.md) for the known [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) and a [Fourier sine series](../../../../../../fourier-sine-series.md) for the unknown [normal derivative](../../../../../../normal-derivative.md):

$$
f_j(s)\simeq f_j^{(M)}(s)=\sum_{\ell=0}^M d_{j\ell}P_\ell(s),\qquad q_j(s)\simeq q_j^{(N)}(s)=\sum_{m=1}^N c_{jm}\phi_m(s),\qquad \phi_m(s)=\sin[p_m(s+1)],\quad p_m=\frac{m\pi}{2}.
$$

The known coefficients are $d_{j\ell}=(2\ell+1)\int_{-1}^1f_jP_\ell\,ds/2$. The sine functions have $\int_{-1}^1\phi_m\phi_n\,ds=\delta_{mn}$ and form a complete [basis](../../../../../../basis.md) in $L^2(-1,1)$. Choosing them for the [normal derivative](../../../../../../normal-derivative.md) does not impose zero flux at a corner: the expansion is an $L^2$ representation, and endpoint values are not determined by it. If preserving corner values of the approximated Dirichlet trace is necessary, subtract its endpoint-interpolating line before [polynomial](../../../../../../polynomial-split.md) approximation, and add that line back. All subsequent known-data integrals can alternatively be evaluated with the exact $f_j$.

Define the [entire function](../../../../../../entire-function.md) basis transforms

$$
\mathsf P_\ell(\tau)=\int_{-1}^1e^{\tau s}P_\ell(s)\,ds,\qquad \mathsf S_m(\tau)=\int_{-1}^1e^{\tau s}\phi_m(s)\,ds=\frac{p_m[e^{-\tau}-(-1)^me^\tau]}{\tau^2+p_m^2}.
$$

At $\tau=\pm ip_m$ the quotient is evaluated by its removable limit or by the defining integral. For example, $\mathsf P_0=2\sinh\tau/\tau$, and [polynomial](../../../../../../polynomial-split.md) expansion of $P_\ell$ expresses every $\mathsf P_\ell$ in derivatives of $\mathsf P_0$. Put

$$
F_j^{(M)}(\tau)=\sum_{\ell=0}^Md_{j\ell}\mathsf P_\ell(\tau),\qquad Q_j^{(N)}(\tau)=\sum_{m=1}^Nc_{jm}\mathsf S_m(\tau).
$$

For compactness write $A=A(\lambda)$ and $B=B(\lambda)$. Substituting these expansions into the first [global relation for a linear boundary value problem](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) gives

$$
\boxed{e^{-A}[Q_L^{(N)}(B)+AF_L^{(M)}(B)]+e^A[Q_R^{(N)}(B)-AF_R^{(M)}(B)]+e^{-B}[Q_B^{(N)}(A)+BF_B^{(M)}(A)]+e^B[Q_T^{(N)}(A)-BF_T^{(M)}(A)]\simeq0.}
$$

The signs are fixed by the outward [normal vectors](../../../../../../normal-vector.md), rather than by a choice of traversal direction. The second approximate [global relation for a linear boundary value problem](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) replaces $A$ by $-A$, leaving $B$ unchanged:

$$
\boxed{e^A[Q_L^{(N)}(B)-AF_L^{(M)}(B)]+e^{-A}[Q_R^{(N)}(B)+AF_R^{(M)}(B)]+e^{-B}[Q_B^{(N)}(-A)+BF_B^{(M)}(-A)]+e^B[Q_T^{(N)}(-A)-BF_T^{(M)}(-A)]\simeq0.}
$$

Here $\simeq0$ records omitted boundary-expansion tails. In a finite [spectral method](../../../../../../spectral-method.md) the selected equations are set equal to zero to solve for the $4N$ unknown real [coefficients](../../../../../../coefficient.md) $c_{jm}$. For real data the two families obey the same [complex conjugation](../../../../../../complex-conjugation.md) relation as their exact counterparts.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 328](../../../paper-328-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
