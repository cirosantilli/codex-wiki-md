<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

Expanding with the [angular momentum](../../../../../angular-momentum.md) [commutators](../../../../../commutator.md) gives

$$
\begin{aligned}
[\hat L_z,\hat L_\pm]&=[\hat L_z,\hat L_x]\pm i[\hat L_z,\hat L_y]=\pm\hbar\hat L_\pm,\\
\hat L_-\hat L_+&=(\hat L_x-i\hat L_y)(\hat L_x+i\hat L_y)=\hat L_x^2+\hat L_y^2+i[\hat L_x,\hat L_y]=\hat L^2-\hat L_z^2-\hbar\hat L_z.
\end{aligned}
$$

For $\hat L_z|\psi\rangle=\alpha\hbar|\psi\rangle$, commuting $\hat L_z$ past a [ladder operator](../../../../../ladder-operator.md) gives

$$
\hat L_z\hat L_\pm|\psi\rangle=(\alpha\pm1)\hbar\hat L_\pm|\psi\rangle.
$$

Thus the raised or lowered vector, **if nonzero**, is an [eigenvector](../../../../../eigenvector.md) with the shifted [eigenvalue](../../../../../eigenvalue.md); an [angular momentum ladder endpoint](../../../../../angular-momentum-ladder-endpoint.md) can instead be annihilated. Also $[\hat L^2,\hat L_\pm]=0$, so $\hat L^2\hat L_\pm|\psi\rangle=\Lambda\hbar^2\hat L_\pm|\psi\rangle$ for every nonzero ladder result.

For [orbital angular momentum](../../../../../orbital-angular-momentum.md), $\hat L_z=-i\hbar\partial_\phi$ gives an azimuthal factor $e^{i\alpha\phi}$. Single-valuedness under $\phi\mapsto\phi+2\pi$ requires **integer $\alpha$**. Positivity of ladder norms gives

$$
\|\hat L_+|\Lambda,m\rangle\|^2=\hbar^2[\Lambda-m(m+1)],\qquad
\|\hat L_-|\Lambda,m\rangle\|^2=\hbar^2[\Lambda-m(m-1)]
$$

for normalized states. A fixed finite $\Lambda$ therefore has upper and lower endpoints. Writing the upper endpoint as $m=\ell$, its vanishing raising norm gives $\Lambda=\ell(\ell+1)$; the lower endpoint is $m=-\ell$. Consequently

$$
\boxed{\hat L^2|\ell,m\rangle=\ell(\ell+1)\hbar^2|\ell,m\rangle,\quad \hat L_z|\ell,m\rangle=m\hbar|\ell,m\rangle,\quad m=-\ell,-\ell+1,\ldots,\ell,}
$$

with $\ell=0,1,2,\ldots$. This integer conclusion is for [orbital angular momentum](../../../../../orbital-angular-momentum.md); [spin](../../../../../spin.md) representations can also have half-integer labels.

For the specified Gaussian-radial state, use a [Cartesian p-orbital decomposition](../../../../../cartesian-p-orbital-decomposition.md): write $x+y+z=r(\sin\theta\cos\phi+\sin\theta\sin\phi+\cos\theta)$. Its angular factor is

$$
\sqrt{\frac{2\pi}{3}}\left[(1+i)Y_{1,-1}+\sqrt2Y_{1,0}+(-1+i)Y_{1,1}\right].
$$

Only $\ell=1$ occurs. The squared angular coefficients are $2,2,2$ before common normalization, so each allowed $m$ has probability one third. Therefore the simultaneous outcome is

$$
\boxed{P(L^2=2\hbar^2,L_z=\hbar)=\frac13.}
$$

The common normalized radial factor cancels from this ratio. The standard symmetric $m$ sequence used above resolves the duplicated central positive entry in the printed list.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
