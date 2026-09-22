<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At second order the [Taylor-expanded no-slip boundary condition](../../../../../../taylor-expanded-no-slip-boundary-condition.md) is

$$
\psi_{2y}(0)=-\sin\theta\,\psi_{1yy}(0)=\sin^2\theta=\frac12(1-\cos2\theta),\qquad \psi_{2x}(0)=-\sin\theta\,\psi_{1xy}(0)=0,
$$

with $\nabla^4\psi_2=0$, $\psi_{2y}\to U_2$, and $\psi_{2x}\to0$ at infinity. Set the irrelevant boundary constant to zero. The general relevant solution contains a zero [Fourier mode](../../../../../../fourier-mode.md) and a second harmonic:

$$
\psi_2=A+By+Cy^2+Dy^3+\operatorname{Re}\{[E e^{-2y}+F e^{2y}+y(G e^{-2y}+J e^{2y})]e^{2i\theta}\}.
$$

Bounded velocity eliminates $C,D$ and growing harmonics. Averaging the tangential boundary condition gives $B=\langle\sin^2\theta\rangle=1/2$. This is the [mean boundary velocity determines Taylor-sheet swimming speed](../../../../../../mean-boundary-velocity-determines-taylor-sheet-swimming-speed.md) principle: the remaining mean velocity is uniform and equals the far-field velocity. Therefore

$$
\boxed{U_2=\frac12,\qquad \mathbf V_{\rm swim}=-\frac{\epsilon^2}{2}\mathbf e_x+O(\epsilon^4).}
$$

The absence of odd powers follows because changing the amplitude sign is just a half-wavelength translation. Although unnecessary for the speed, the oscillatory solution can also be written explicitly as $\psi_2=y/2-(y/2)e^{-2y}\cos2\theta$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 334](../../../paper-334-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
