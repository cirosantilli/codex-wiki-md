<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Diagonalizing the $J_1$ [matrix](../../../../../matrix.md) gives the normalized [eigenvectors](../../../../../eigenvector.md)

$$
v_+=\frac12\begin{pmatrix}1\\\sqrt2\\1\end{pmatrix},\qquad
v_0=\frac1{\sqrt2}\begin{pmatrix}1\\0\\-1\end{pmatrix},\qquad
v_-=\frac12\begin{pmatrix}1\\-\sqrt2\\1\end{pmatrix},
$$

with [eigenvalues](../../../../../eigenvalue.md) $+\hbar,0,-\hbar$, respectively. The first [projective measurement](../../../../../projective-measurement.md) prepares $v_+$ up to [global phase](../../../../../global-phase.md), regardless of the earlier state, conditional on obtaining $+\hbar$.

The [unitary time evolution](../../../../../unitary-time-evolution.md) under $H=\omega J_3$ gives, with $\theta=\omega t$,

$$
|\Psi(t)\rangle=\operatorname{diag}(e^{-i\theta},1,e^{i\theta})v_+
=\frac12\begin{pmatrix}e^{-i\theta}\\\sqrt2\\e^{i\theta}\end{pmatrix}.
$$

The [probability amplitudes](../../../../../probability-amplitude.md) for the second [projective measurement](../../../../../projective-measurement.md) are

$$
\langle v_+|\Psi(t)\rangle=\frac{1+\cos\theta}{2},\qquad
\langle v_0|\Psi(t)\rangle=-\frac{i\sin\theta}{\sqrt2},\qquad
\langle v_-|\Psi(t)\rangle=\frac{\cos\theta-1}{2}.
$$

The [Born rule](../../../../../born-rule.md) therefore gives the general [spin-one transverse measurement after axial precession](../../../../../spin-one-transverse-measurement-after-axial-precession.md):

$$
\Pr(+\hbar)=\cos^4\frac\theta2,\qquad
\Pr(0)=\frac12\sin^2\theta,\qquad
\Pr(-\hbar)=\sin^4\frac\theta2.
$$

At the specified times $t_k=\pi k/\omega$, $\theta=\pi k$, so

$$
\boxed{\Pr(+\hbar)=\frac{1+(-1)^k}{2},\qquad
\Pr(0)=0,\qquad
\Pr(-\hbar)=\frac{1-(-1)^k}{2}.}
$$

For even $k$, the result is certainly $+\hbar$; for odd $k$, it is certainly $-\hbar$. Although zero belongs to the spectrum of the [observable](../../../../../observable.md), it never occurs at these times. Indeed, for even $k$ the evolved vector is $v_+$, while for odd $k$ it is $-v_-$, where the minus sign is a [global phase](../../../../../global-phase.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
