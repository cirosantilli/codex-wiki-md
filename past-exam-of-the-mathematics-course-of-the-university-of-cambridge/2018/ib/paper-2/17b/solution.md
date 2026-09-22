<h1 id="17b/solution">Solution</h1>

↑ **Parent:** [17B](../17b.md)

In atomic units the [Time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md) is

$$
\left(-\frac12\nabla^2-\frac1r\right)\psi=E\psi.
$$

The displayed equation is the [Radial Schrodinger equation for the hydrogen atom](../../../../../radial-schrodinger-equation-for-the-hydrogen-atom.md). Its radial derivative terms come from the [Laplacian in spherical coordinates](../../../../../laplacian-in-spherical-coordinates.md), the Coulomb term is the potential $-1/r$, and separation into [spherical harmonics](../../../../../spherical-harmonic.md) uses the [orbital angular momentum](../../../../../orbital-angular-momentum.md) eigenvalue $l(l+1)$, producing the centrifugal term $-l(l+1)R/r^2$.

For $E=-1/(2n^2)$, substitute $R=r^\alpha e^{-r/n}$. Dividing the equation by $R$ and comparing powers of $r$ gives

$$
\alpha(\alpha+1)=l(l+1),
\qquad
\frac{\alpha+1}{n}=1.
$$

The solution regular at the origin has $\alpha=l$, and when $l=n-1$ both equations agree. This is the [circular Coulomb bound state](../../../../../circular-coulomb-bound-state.md). Thus

$$
\boxed{\alpha=n-1.}
$$

The radial probability measure is $|R(r)|^2r^2\,dr$. With $a=2/n$ and the [Gamma integral](../../../../../gamma-integral.md), the [mean radius of a circular Coulomb bound state](../../../../../mean-radius-of-a-circular-coulomb-bound-state.md) is

$$
\langle r\rangle
=\frac{\int_0^\infty r^{2n+1}e^{-ar}\,dr}
{\int_0^\infty r^{2n}e^{-ar}\,dr}
=\frac{2n+1}{a}
=\boxed{\frac{n(2n+1)}2}.
$$

At fixed [principal quantum number](../../../../../principal-quantum-number.md) $n$, the allowed [orbital angular momentum](../../../../../orbital-angular-momentum.md) quantum numbers are $l=0,\ldots,n-1$, and each has [magnetic quantum number](../../../../../magnetic-quantum-number.md) $m=-l,\ldots,l$. Hence the orbital [quantum degeneracy](../../../../../degenerate-energy-levels.md) is

$$
\boxed{\sum_{l=0}^{n-1}(2l+1)=n^2.}
$$

Including electron spin would double this to $2n^2$, but spin is absent from the stated wavefunctions.

## ↑ Ancestors (10)

1. [17B](../17b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
