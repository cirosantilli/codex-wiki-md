<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Expand the square root and quotient in the [logarithmic-height plume equations](../../../../../../logarithmic-height-plume-equations.md):

$$
\widehat M^{1/2}=1+\tfrac12\epsilon M'+O(\epsilon^2),\qquad\frac{\widehat F\widehat Q}{\widehat M}=1+\epsilon(F'+Q'-M')+O(\epsilon^2).
$$

The [linear stability analysis](../../../../../../linear-stability.md) gives

$$
\boxed{\frac d{d\xi}\begin{pmatrix}Q'\\M'\\F'\end{pmatrix}=J\begin{pmatrix}Q'\\M'\\F'\end{pmatrix},\qquad J=\begin{pmatrix}-q&q/2&0\\m&-2m&m\\f&0&-f\end{pmatrix}.}
$$

In particular, the second row contains $-2mM'$, since the reciprocal of $\widehat M$ contributes another $-M'$.

For the [growing mode of power-law plume similarity](../../../../../../growing-mode-of-power-law-plume-similarity.md), the [characteristic polynomial](../../../../../../characteristic-polynomial.md) is

$$
P(\lambda)=\lambda^3+(q+2m+f)\lambda^2+\left(\frac32qm+qf+2mf\right)\lambda+qmf.
$$

Within the physical interval $q,m>0$ and $f<0$, $P(0)<0$ while $P(\lambda)\to+\infty$ as $\lambda\to+\infty$. There is a positive real [eigenvalue](../../../../../../eigenvalue.md), so the similarity equilibrium is **unstable with increasing height**. Perturbations behave as $e^{\lambda\xi}\propto z^\lambda$; the result is not stability in physical time. Thus this exact positive-buoyancy similarity trajectory is not a generic attracting far field.

At the upper endpoint,

$$
\boxed{\beta\to-\frac83:\qquad f\to0^-,\quad q\to\frac53,\quad m\to\frac43.}
$$

The limiting polynomial is $\lambda(\lambda+1)(\lambda+10/3)$, reproducing the three stated [eigenvalues](../../../../../../eigenvalue.md). The positive [eigenvalue](../../../../../../eigenvalue.md) tends to zero, with $\lambda\sim-2f/3$. The two negative modes decay as $z^{-1}$ and $z^{-10/3}$; the remaining mode is neutral at the limiting linear system. Its [eigenvector](../../../../../../eigenvector.md) is $(1,2,3)$ in relative-flux coordinates.

The [neutral buoyancy-flux mode of a pure plume](../../../../../../neutral-buoyancy-flux-mode-of-a-pure-plume.md) has a simple interpretation: a constant surviving [buoyancy flux](../../../../../../buoyancy-flux.md) fixes the [amplitudes](../../../../../../wave-amplitude.md) of a [pure plume](../../../../../../pure-plume.md), with $Q\propto F^{1/3}z^{5/3}$ and $M\propto F^{2/3}z^{4/3}$. A small fractional change in $F$ produces changes in $Q,M$ in the ratio $1:2:3$. It is retained rather than damped out.

There is a qualification at the exact endpoint. For fixed nonzero $K$ and $\beta=-8/3$, taking $Q\propto z^{5/3}$ gives $F_z\propto-z^{-1}$, not zero. The flux coefficients above also diverge as $f\to0$. Thus the constant-flux powers are the formal limiting scaling, not an exact constant-buoyancy solution in a nonzero endpoint stratification; cumulative ambient effects can require logarithmic corrections.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 330](../../../paper-330-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
