<h1 id="2/vii/solution">Solution</h1>

↑ **Parent:** [Vii](../vii.md)

Differentiate the [Noether charge](../../../../../../noether-charge.md) and use $\dot\phi_a=\pi_a$ and the [Klein-Gordon equation](../../../../../../klein-gordon-equation.md) for each species. The momentum products cancel because the two species commute:

$$
\begin{aligned}
\dot Q&=\int d^3x\,[\pi_2\pi_1+\phi_2(\nabla^2-m_1^2)\phi_1
-\pi_1\pi_2-\phi_1(\nabla^2-m_2^2)\phi_2]\\
&=\int d^3x\,[\phi_2\nabla^2\phi_1-\phi_1\nabla^2\phi_2]
+(m_2^2-m_1^2)\int d^3x\,\phi_1\phi_2.
\end{aligned}
$$

The first integral is the boundary flux of $\phi_2\nabla\phi_1-\phi_1\nabla\phi_2$, so it vanishes under the same boundary condition used for charge conservation. Hence

$$
\boxed{\frac{dQ}{dt}=(m_2^2-m_1^2)\int d^3x\,\phi_1\phi_2.}
$$

Conservation must hold for arbitrary configurations, rather than only a state in which this particular integral happens to vanish. Thus the [internal rotation symmetry of two real scalar fields](../../../../../../internal-rotation-symmetry-of-two-real-scalar-fields.md) requires

$$
\boxed{m_1^2=m_2^2,\qquad\text{and therefore }m_1=m_2\text{ for nonnegative masses}.}
$$

Equivalently, the local divergence is $\partial_\mu j^\mu=(m_2^2-m_1^2)\phi_1\phi_2$, exhibiting exactly how unequal masses break the symmetry.

## ↑ Ancestors (11)

1. [Vii](../vii.md)
2. [2](../../2.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
