<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

There is one four-gluon [tadpole diagram](../../../../../tadpole-diagram.md). Temporarily replace its internal [gluon propagator](../../../../../gluon-propagator.md) by $-ig_{\rho\sigma}\delta^{cd}/(l^2-m_g^2+i0)$. Contract the supplied four-gluon [Feynman vertex](../../../../../interaction-vertex.md) with $g_{\rho\sigma}\delta^{cd}$. Its first [colour factor](../../../../../color-factor.md) vanishes because $f^{cce}=0$. Each of the other two terms contributes $C_A\delta^{ab}(D-1)g^{\mu\nu}$, so

$$
\delta^{cd}g_{\rho\sigma}V_4^{\mu\nu\rho\sigma,abcd}=-2ig_D^2C_A\delta^{ab}(D-1)g^{\mu\nu}.
$$

Include the [symmetry factor](../../../../../feynman-diagram-symmetry-factor.md) $1/2$ and the factor $-i$ from the internal [gluon propagator](../../../../../gluon-propagator.md):

$$
i\Pi_{4g}^{\mu\nu,ab}=-g_D^2C_A\delta^{ab}(D-1)g^{\mu\nu}J_1(m_g^2).
$$

The exact regulated [tadpole integral](../../../../../tadpole-integral.md) is

$$
J_1(m_g^2)=-\frac{i}{(4\pi)^{D/2}}\Gamma(1-D/2)(m_g^2)^{D/2-1}.
$$

In particular,

$$
i\Pi_{4g}^{\mu\nu,ab}\big|_{\mathrm{UV}}=-\frac{i g^2C_A\delta^{ab}}{8\pi^2\epsilon}(D-1)m_g^2g^{\mu\nu}.
$$

The entire expression is proportional to $(m_g^2)^{1-\epsilon/2}$ and vanishes as the auxiliary [mass](../../../../../mass.md) tends to zero near four dimensions. Equivalently, its expanded terms are proportional to $m_g^2/\epsilon$, $m_g^2\log m_g^2$ and $m_g^2$, all of which disappear when the regulator is removed. Hence

$$
\boxed{\Pi_{4g}^{\mu\nu,ab}=0\qquad(m_g\to0).}
$$

This is the massless [scaleless integral](../../../../../scaleless-integral.md) result obtained directly in [dimensional regularization](../../../../../dimensional-regularization.md). The artificial [mass](../../../../../mass.md) is only an intermediate device for this graph; retaining it in the full theory would modify the [gauge symmetry](../../../../../gauge-invariance.md) and cannot be used when applying the massless transversality identity in part (iv).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
