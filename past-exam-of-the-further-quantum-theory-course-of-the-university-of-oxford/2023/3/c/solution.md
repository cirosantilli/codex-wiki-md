<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the amplitudes and positive [action integrals](../../../../action-integral.md) of part (a), and define the right-well phase

$$
\theta(E)=\frac1\hbar\int_{x_1(E)}^{x_2(E)}p(x)\,dx.
$$

Matching at the inner [classical turning point](../../../../classical-turning-point.md) gives $C=A$, $D=2B$. Matching the exterior decaying [wavefunction](../../../../wave-function-split.md) at the outer [classical turning point](../../../../classical-turning-point.md) gives

$$
\psi_{\rm II}(x)\simeq\frac{2F}{\sqrt{p(x)}}\sin\left(\frac1\hbar\int_x^{x_2}p(y)\,dy+\frac\pi4\right)=\frac{2F}{\sqrt{p(x)}}\sin(\theta-s(x)+\pi/4).
$$

The [trigonometric identity](../../../../trigonometric-identity.md)

$$
\sin(\theta-s+\pi/4)=\cos\theta\cos(s+\pi/4)+\sin\theta\sin(s+\pi/4)
$$

therefore yields

$$
\boxed{A=C=2F\cos\theta,\qquad B=F\sin\theta,\qquad D=2F\sin\theta.}
$$

All three pieces on $x>0$ are now fixed up to $E$ and $F$:

$$
\psi_R(x)\simeq\begin{cases}
\dfrac{F}{\sqrt{\chi(x)}}\bigl[2\cos\theta\,e^{K(x)}+\sin\theta\,e^{-K(x)}\bigr],&0<x<x_1,\\
\dfrac{2F}{\sqrt{p(x)}}\sin(\theta-s(x)+\pi/4),&x_1<x<x_2,\\
\dfrac{F}{\sqrt{\chi(x)}}e^{-U(x)},&x>x_2.
\end{cases}
$$

The [Airy function](../../../../airy-function.md) descriptions replace the apparent singularities at the [classical turning points](../../../../classical-turning-point.md). For the permitted [energy eigenvalues](../../../../energy-eigenvalue-split.md), part (d) extends this right-hand [wavefunction](../../../../wave-function-split.md) to the left by even or odd [parity](../../../../parity.md); $F$ is then determined by [wavefunction normalization](../../../../wavefunction-normalization.md). At arbitrary $E$, the decaying right-hand solution instead has a unique continuation by the [Schrödinger equation](../../../../schrodinger-equation.md), which need not decay at negative infinity.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further quantum theory course of the University of Oxford](../../../split.md)
5. [Further quantum theory course of the University of Oxford](../../../../further-quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
