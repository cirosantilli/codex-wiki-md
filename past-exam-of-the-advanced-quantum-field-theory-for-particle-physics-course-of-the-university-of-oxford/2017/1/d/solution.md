<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply the [dimensionally regulated](../../../../dimensional-regularization.md) [tadpole](../../../../tadpole-diagram.md) integral before removing the [infrared regulator](../../../../infrared-regularization.md):

$$
I_\gamma(m_\gamma)=\mu^\epsilon\int\frac{d^dl}{(2\pi)^d}\frac1{l^2+m_\gamma^2}
=\frac{i\mu^\epsilon}{(4\pi)^{2-\epsilon/2}}\Gamma\left(-1+\frac\epsilon2\right)(m_\gamma^2)^{1-\epsilon/2}.
$$

At fixed regulator $0<\operatorname{Re}\epsilon<2$ away from [gamma-function poles](../../../../gamma-function.md), the power of $m_\gamma^2$ has positive real part. Consequently

$$
\boxed{\lim_{m_\gamma\to0}I_\gamma(m_\gamma)=0.}
$$

Both the correctly weighted [tadpole](../../../../tadpole-diagram.md) and the source's doubled version vanish. This is the near-four-dimensional limit appropriate to the question; the order of limits is important. Equivalently the exactly massless [tadpole](../../../../tadpole-diagram.md) is a [scaleless integral](../../../../scaleless-integral.md) and is zero in [dimensional regularization](../../../../dimensional-regularization.md). The statement is not valid for every arbitrary fixed dimension: for example, $\epsilon=5/2$ gives a nonzero prefactor and growth as $m_\gamma^{-1/2}$. One must keep the regulator in its stated near-four-dimensional domain.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
