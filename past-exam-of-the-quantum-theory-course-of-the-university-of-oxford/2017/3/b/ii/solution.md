<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Starting from $f_{-1}=\sin\theta\,e^{-i\phi}$, part (i) gives $L^2f_{-1}=2\hbar^2f_{-1}$ and $L_3f_{-1}=-\hbar f_{-1}$. Apply the [angular momentum raising operator](../../../../../angular-momentum-raising-operator.md) explicitly:

$$
L_+f_{-1}=\hbar e^{i\phi}\left(\cos\theta e^{-i\phi}+i\cot\theta(-i\sin\theta e^{-i\phi})\right)=2\hbar\cos\theta.
$$

A second application gives

$$
L_+\cos\theta=-\hbar\sin\theta e^{i\phi}.
$$

Since $L_+$ commutes with $L^2$, both raised functions retain the [eigenvalue](../../../../../eigenvalue.md) $2\hbar^2$. Their $L_3$ [eigenvalues](../../../../../eigenvalue.md) follow either by differentiating their $\phi$ dependence or from $[L_3,L_+]=\hbar L_+$. Thus three valid unnormalized functions, in the requested order, are

$$
\boxed{f_{-1}=\sin\theta e^{-i\phi},\qquad f_0=\cos\theta,\qquad f_{+1}=\sin\theta e^{i\phi}.}
$$

For later [Born rule](../../../../../born-rule.md) calculations, normalize with the [solid angle](../../../../../solid-angle.md) measure $d\Omega=\sin\theta\,d\theta\,d\phi$. Their squared [norms](../../../../../norm.md) are $8\pi/3$, $4\pi/3$, $8\pi/3$, respectively. For example $\int_0^\pi\sin^3\theta\,d\theta=4/3$ and $\int_0^\pi\cos^2\theta\sin\theta\,d\theta=2/3$. A convenient [orthonormal basis](../../../../../orthonormal-basis.md) is therefore

$$
\chi_{-1}=\sqrt{\frac3{8\pi}}\sin\theta e^{-i\phi},\qquad \chi_0=\sqrt{\frac3{4\pi}}\cos\theta,\qquad \chi_{+1}=\sqrt{\frac3{8\pi}}\sin\theta e^{i\phi}.
$$

[Orthogonality](../../../../../orthogonal-vectors.md) follows from the distinct Fourier factors in $\phi$. An overall phase of each basis function is arbitrary; these choices need not impose the usual phase convention for the [spherical harmonics](../../../../../spherical-harmonic.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
