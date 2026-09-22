<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The nullspace in the [Fourier diffraction theorem](../../../../../../fourier-diffraction-theorem.md) already prevents uniqueness, and the rapid decay of evanescent high-frequency information prevents stable recovery. Both make this an [ill-posed inverse problem](../../../../../../ill-posed-inverse-problem.md).

Let $A_\pm$ be the linear [Born approximation](../../../../../../born-approximation.md) operators mapping a real contrast supported in a known region $D$ to the measured fields on the two observation planes. For data $d_\pm$, a suitable [Tikhonov reconstruction from two-plane scattering data](../../../../../../tikhonov-reconstruction-from-two-plane-scattering-data.md) minimizes

$$
\boxed{J_\alpha(V)=\|A_+V-d_+\|_{L^2(S_+)}^2
+\|A_-V-d_-\|_{L^2(S_-)}^2+\alpha\|V\|_{L^2(D)}^2,
\qquad \alpha>0.}
$$

A [Sobolev norm](../../../../../../sobolev-norm.md) penalty can instead express a smoothness preference. Reality, known support and $n=1-V/k>0$ can be imposed as constraints. For the unconstrained complex Hilbert-space problem with the displayed quadratic penalty, write $A=(A_+,A_-)$ and $d=(d_+,d_-)$. Its [Tikhonov normal equation](../../../../../../tikhonov-normal-equation.md) is

$$
(A^*A+\alpha I)V_\alpha=A^*d,
\qquad V_\alpha=(A^*A+\alpha I)^{-1}A^*d.
$$

[Tikhonov regularization](../../../../../../tikhonov-regularization.md) selects a stable preferred estimate; it does not establish that the original two-plane data uniquely determine the true contrast.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
