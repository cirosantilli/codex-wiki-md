<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

[matrix](../../../../../matrix.md) multiplication gives $\sigma_i\sigma_j=\delta_{ij}I+i\epsilon_{ijk}\sigma_k$, hence $[\sigma_i,\sigma_j]=2i\epsilon_{ijk}\sigma_k$. For physical [neutron](../../../../../neutron-split.md) [spin](../../../../../spin.md), use $\mathbf S=(\hbar/2)\boldsymbol\sigma$, so $[S_i,S_j]=i\hbar\epsilon_{ijk}S_k$, $S^2=3\hbar^2/4$, and measurement along any axis gives **$\pm\hbar/2$**.

For the specified field, $H=(\alpha B\hbar/2)\sigma_y$. The [Time-dependent Schrödinger equation](../../../../../time-dependent-schrodinger-equation.md) is $i\hbar\dot\psi=H\psi$ with $\psi(0)=(1,0)^T$. The [uniform-field spin precession](../../../../../uniform-field-spin-precession.md) follows from $\sigma_y^2=I$:



$$
\psi(t)=e^{-i\alpha Bt\sigma_y/2}\binom10
=\boxed{\binom{\cos\phi}{\sin\phi}},\qquad
\boxed{\phi(t)=\alpha Bt/2}.
$$

The sign of the precession is contained in the given $\alpha$. The normalized $x$-axis eigenstates are **$(1,1)^T/\sqrt2$ and $(1,-1)^T/\sqrt2$**.

The measurement direction is $\mathbf n=(0,\sin\theta,\cos\theta)$, as confirmed by the original diagram. Write $c=\cos(\theta/2)$ and $s=\sin(\theta/2)$. The spinors $\chi_+=(c,is)^T$ and $\chi_-=(is,c)^T$ have unit norm and [inner product](../../../../../inner-product-split.md) $ics-isc=0$. Applying $\mathbf n\cdot\boldsymbol\sigma$ gives [eigenvalues](../../../../../eigenvalue.md) $+1$ and $-1$. At $\theta=0$ they are the usual $z$ basis; at $\pi/2$ they are the $y$ basis up to a [phase](../../../../../phase-waves.md); at $\pi$ the $z$ up/down roles are exchanged, with a factor $i$; and at $2\pi$ both return with a minus sign. A spinor changes sign under a full rotation, while its isolated-state measurement [probabilities](../../../../../probability.md) are unchanged.

For [spin measurement in the yz plane](../../../../../spin-measurement-in-the-yz-plane.md), projection gives

$$
P_+=|c\cos\phi-is\sin\phi|^2
=\boxed{\frac{1+\cos\theta\cos(\alpha Bt)}2},\qquad
\boxed{P_-=\frac{1-\cos\theta\cos(\alpha Bt)}2}.
$$

For $\theta=0$ these are $\cos^2\phi,\sin^2\phi$; for $\pi/2$ both are $1/2$ at all times; for $\pi$ they are exchanged; and for $2\pi$ they are the same as at zero angle. The constant $y$ [probabilities](../../../../../probability.md) also follow from conservation of $S_y$.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
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
