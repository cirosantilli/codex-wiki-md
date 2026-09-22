<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Expanding the matrix [determinant](../../../../../../determinant.md) from part (b) gives

$$
\det M=ik(\alpha-\alpha^2)\Delta(k)=-\sqrt3k\Delta(k),\qquad
\Delta(k)=e^{-ikL}+\alpha e^{-i\alpha kL}+\alpha^2e^{-i\alpha^2kL}.
$$

The [finite-interval Airy spectral determinant](../../../../../../finite-interval-airy-spectral-determinant.md) obeys $\Delta(\alpha k)=\alpha^2\Delta(k)$. At the origin,

$$
\Delta(k)=-\frac32L^2k^2+O(k^5).
$$

This zero comes from coalescence of the three rotated equations; it is removable in the underlying boundary system. Indeed, $v'''=0$ with $v(0)=v(L)=v'(L)=0$ has only the zero quadratic solution.

For $k\ne0$, a zero of $\Delta$ is equivalent to the existence of a nonzero combination $v(x)=\sum_{j=0}^2c_je^{i\alpha^jkx}$ satisfying the homogeneous endpoint conditions. This can be checked by expanding the determinant of those three endpoint equations. Such a function satisfies $v'''=\omega(k)v$, so it is an [eigenfunction](../../../../../../eigenfunction.md) of $A$ with [eigenvalue](../../../../../../eigenvalue.md) $-\omega(k)$. [Integration by parts](../../../../../../integration-by-parts.md) yields

$$
-\operatorname{Re}\omega(k)\,\|v\|_2^2=\operatorname{Re}\langle v,Av\rangle=-\frac12|v'(0)|^2,
$$

so every nonzero zero has $\operatorname{Re}\omega(k)\geq0$. None lies on the boundary $\operatorname{Re}\omega=0$: by a cube-root rotation it suffices to take $K=kL$ real. With $u=\sqrt3K/2$, the determinant equation becomes

$$
e^{-3iK/2}=\cosh u-i\sqrt3\sinh u.
$$

The right-hand side has squared modulus $1+4\sinh^2u>1$ for $K\ne0$, whereas the left-hand side has modulus one. Therefore **there are no nonremovable spectral poles in $\overline D$**, and the contour representation has no discrete residue contribution from that domain.

Taken literally as a claim about the operator's [discrete spectrum](../../../../../../discrete-spectrum.md), however, the printed assertion is false. To see this constructively, put $k=-is/L$, $s>0$. Then

$$
\Delta(-is/L)=e^{-s}-2e^{s/2}\cos(\sqrt3s/2+\pi/3).
$$

Thus zeros occur when

$$
e^{-3s/2}=2\cos(\sqrt3s/2+\pi/3).
$$

Between successive positive cosine maxima and adjacent negative minima the difference changes sign. There are consequently infinitely many positive roots, producing genuine negative [eigenvalues](../../../../../../eigenvalue.md) $-s^3/L^3$ of $A$. The third-order resolvent maps into $H^3(0,L)$, whose inclusion into $L^2(0,L)$ is compact, so these are indeed [discrete spectrum](../../../../../../discrete-spectrum.md) of an operator with [compact resolvent](../../../../../../compact-resolvent.md). **The valid conclusion is absence of poles in the reconstruction sectors, not absence of operator eigenvalues.**

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
