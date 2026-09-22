<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

The angular-momentum [commutators](../../../../../commutator.md) give

$$
\boxed{[L_+,L_z]=-\hbar L_+,\qquad
[L_-,L_z]=+\hbar L_-,\qquad
[L_+,L_-]=2\hbar L_z}.
$$

For example $[L_x+iL_y,L_z]=-i\hbar L_y+i(i\hbar L_x)=-\hbar L_+$. In the displayed basis $|1,1\rangle,|1,0\rangle,|1,-1\rangle$, the only nonzero upper entries of $L_+$ connect adjacent magnetic quantum numbers. Subtracting their column and row $L_z$ [eigenvalues](../../../../../eigenvalue.md) multiplies each by $-\hbar$, proving the first [matrix](../../../../../matrix.md) [commutator](../../../../../commutator.md); the lower [matrix](../../../../../matrix.md) similarly gives the second. Direct multiplication gives

$$
L_+L_-=2\hbar^2\operatorname{diag}(1,1,0),\quad
L_-L_+=2\hbar^2\operatorname{diag}(0,1,1),
$$

whose difference is $2\hbar L_z$. Also $L^2=L_z^2+(L_+L_-+L_-L_+)/2=2\hbar^2I$, confirming $\ell=1$.

A [rotation](../../../../../rotation-mathematics.md) changes the quantization axis without changing the spectrum, so **$L_{\mathbf n}$ has [eigenvalues](../../../../../eigenvalue.md) $+\hbar,0,-\hbar$**. Its dimensionless [matrix](../../../../../matrix.md) is

$$
\frac{L_{\mathbf n}}{\hbar}=
\begin{pmatrix}
\cos\theta&\sin\theta/\sqrt2&0\\
\sin\theta/\sqrt2&0&\sin\theta/\sqrt2\\
0&\sin\theta/\sqrt2&-\cos\theta
\end{pmatrix}.
$$

Solving $(L_{\mathbf n}-\hbar I)v=0$ and normalizing gives the [spin-one maximum-projection eigenvector](../../../../../spin-one-maximum-projection-eigenvector.md)

$$
\boxed{v_+(\theta)=
\begin{pmatrix}
\cos^2(\theta/2)\\
\sin\theta/\sqrt2\\
\sin^2(\theta/2)
\end{pmatrix}}.
$$

For instance the first equation is $(\cos\theta-1)\cos^2(\theta/2)+\sin^2\theta/2=0$, and the squared components sum to one. An overall [phase](../../../../../phase-waves.md) is immaterial.

At $\theta=\pi/3$, $v_+=(3/4,\sqrt6/4,1/4)^{\mathsf T}$. The [Born rule](../../../../../born-rule.md) therefore predicts, in the requested order,

$$
\boxed{P(L_z=-\hbar)=\frac1{16},\qquad P(L_z=0)=\frac38,\qquad P(L_z=+\hbar)=\frac9{16}}.
$$

This treats the [Stern-Gerlach experiment](../../../../../stern-gerlach-experiment.md) as the stipulated ideal measurement of orbital projection. In an actual atom, other [magnetic moments](../../../../../magnetic-dipole-moment.md) and [spin-orbit coupling](../../../../../spin-orbit-interaction.md) can change which [angular momentum](../../../../../angular-momentum.md) the apparatus resolves.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2010](../../../split.md)
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
