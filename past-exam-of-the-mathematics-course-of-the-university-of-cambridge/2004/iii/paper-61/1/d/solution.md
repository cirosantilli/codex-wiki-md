<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [cubic dispersion symmetry with negative transport](../../../../../../cubic-dispersion-symmetry-with-negative-transport.md) supplies two other roots of $w(\nu)=w(k)$:

$$
\nu_{1,2}(k)=\frac{-k\pm\sqrt{-3k^2-4}}2,\qquad \nu_1+\nu_2=-k,\qquad\nu_1\nu_2=k^2+1.
$$

Both lie in the lower half-plane when $k\in D_+$. For example this is immediate at large positive imaginary $k$. A root could leave that half-plane only by becoming real, where $\operatorname{Re}w(\nu)=0$, contradicting $\operatorname{Re}w(k)<0$. Connectedness of $D_+$ completes the argument; a coalescence merely exchanges the two roots.

Evaluate the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) at these roots. Because their dispersion values equal $w(k)$, the same boundary transforms occur, and

$$
G_2+i\nu_jG_1=(\nu_j^2+1)G_0-F(\nu_j)+e^{wt}\widehat q(\nu_j,t),\qquad j=1,2.
$$

Interpolate this linear polynomial in $\nu$ at $\nu_1,\nu_2$. Define

$$
\mathcal TF(k)=\frac{(k-\nu_2)F(\nu_1)+(\nu_1-k)F(\nu_2)}{\nu_1-\nu_2},
$$

and similarly $\mathcal T\widehat q(k,t)$. Substitution gives

$$
G_2+ikG_1-(k^2+1)G_0=-\mathcal TF(k)-(3k^2+1)G_0(k,t)+e^{wt}\mathcal T\widehat q(k,t).
$$

Indeed, interpolation of $\nu^2+1$ yields $(\nu_1+\nu_2)k-\nu_1\nu_2+1=-2k^2$, which proves the coefficient $-(3k^2+1)$ after subtracting $k^2+1$.

The final-state term has zero contour integral. After cancelling $e^{wt}$ its integrand is $e^{ikx}\mathcal T\widehat q(k,t)$, holomorphic in $D_+$ and decaying upon closing the contour upward for $x>0$. The possible square-root singularities are removable: the expression is unchanged by exchanging the roots, and when they coalesce at $\nu$, its limit is $F(\nu)+(k-\nu)F'(\nu)$, with the same formula for the final-state transform. Thus the [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) eliminates this unknown term.

We obtain the fully specified [Dirichlet spectral formula for Airy flow with negative transport](../../../../../../dirichlet-spectral-formula-for-airy-flow-with-negative-transport.md)

$$
\boxed{q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-wt}F(k)\,dk-\frac1{2\pi}\int_{\partial D_+}e^{ikx-wt}\bigl[\mathcal TF(k)+(3k^2+1)G_0(k,t)\bigr]dk.}
$$

Only the initial [Fourier transform](../../../../../../fourier-transform.md) and the given boundary-value time transform remain.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
