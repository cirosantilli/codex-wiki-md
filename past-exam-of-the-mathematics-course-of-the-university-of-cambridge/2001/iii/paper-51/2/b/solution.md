<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At conduction, $c$ and $e$ have stable [eigenvalues](../../../../../../eigenvalue.md) $-\varpi$ and $-(4-\varpi)\zeta$. The remaining [linearization](../../../../../../linearization.md) on $(a,b,d)$ is

$$
L=\begin{pmatrix}-\sigma&\sigma r&-\sigma\zeta q\\1&-1&0\\1&0&-\zeta\end{pmatrix}.
$$

Its [characteristic polynomial](../../../../../../characteristic-polynomial.md) is $m^3+Am^2+Bm+C$, where

$$
A=\sigma+1+\zeta,\qquad B=\sigma(1-r)+\sigma\zeta(1+q)+\zeta,\qquad C=\sigma\zeta(1+q-r).
$$

Consequently **the steady threshold is** $\boxed{r_s=1+q}$. The symmetry $(a,b,d)\mapsto(-a,-b,-d)$, with $(c,e)$ unchanged, gives a generic [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md), whose forward or backward direction is determined below. At threshold the other two critical-block [eigenvalues](../../../../../../eigenvalue.md) satisfy $m^2+Am+B_s=0$, where $B_s=\zeta(\sigma+1)-\sigma(1-\zeta)q$. They are stable if $B_s>0$; if $B_s<0$ there is already one unstable transverse direction. Degenerate zero cubic slope requires higher-order analysis and is not a generic pitchfork.

At a [Hopf bifurcation](../../../../../../hopf-bifurcation.md), $AB=C$, $B=\omega^2>0$. Solving the coefficient equation gives

$$
\boxed{r_H={ (\sigma+\zeta)(1+\zeta)\over\sigma}+{\zeta(\sigma+\zeta)\over\sigma+1}q,\qquad
\omega^2={\sigma\zeta(1-\zeta)\over\sigma+1}q-\zeta^2.}
$$

For physical $q\ge0$ the oscillatory threshold therefore exists exactly when $0<\zeta<1$ and $q>q_*$. The [conduction double-zero criterion for five-mode magnetoconvection](../../../../../../conduction-double-zero-criterion-for-five-mode-magnetoconvection.md) gives

$$
\boxed{q_*={\zeta(\sigma+1)\over\sigma(1-\zeta)},\qquad r_*=1+q_*,\qquad0<\zeta<1.}
$$

At this [Bogdanov–Takens bifurcation](../../../../../../bogdanov-takens-bifurcation.md), the polynomial is $m^2(m+A)$ and the zero [eigenspace](../../../../../../eigenspace.md) is one-dimensional. For $q<q_*$ conduction first loses stability at the steady threshold; for $q>q_*$ it first loses stability at $r_H<r_s$. For $\zeta\ge1$ no positive-$q$ double-zero or oscillatory threshold exists. These conclusions also follow from the [Routh-Hurwitz stability criterion](../../../../../../routh-hurwitz-stability-criterion.md), $B,C>0$ and $AB>C$. The [Hopf bifurcation](../../../../../../hopf-bifurcation.md) is transversal since $\partial_r(AB-C)=-\sigma(\sigma+1)\ne0$; its nonlinear criticality is not required by this linear onset calculation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
