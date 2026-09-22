<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $m_g=GM/c^2$, $u=1/r$, and use a prime for $d/d\phi$. The [null geodesic](../../../../null-geodesic.md) first integral obtained above becomes

$$
(u')^2+u^2-2m_g u^3=\frac1{b^2}.
$$

Differentiating with respect to $\phi$ and dividing by $2u'$ away from a turning point gives

$$
\boxed{u''+u=3m_g u^2=\frac{3GM}{c^2}u^2.}
$$

The same [differential equation](../../../../differential-equation-split.md) holds at the turning point by continuity. When $m_g=0$, the general solution is $u_0=C_1\cos\phi+C_2\sin\phi$. Choose the angular origin so that the incoming asymptote has $\phi=0$ and the unperturbed closest approach has $\phi=\pi/2$. The [impact parameter](../../../../impact-parameter.md) then fixes

$$
\boxed{u_0=\frac{\sin\phi}{b},\qquad r\sin\phi=b.}
$$

This is the straight reference path, not a curved orbit.

For [perturbation theory](../../../../perturbation-theory.md) with $m_g/b\ll1$, write $u=u_0+u_1+O(m_g^2/b^3)$, where $u_1=O(m_g/b^2)$. Inserting this into the [differential equation](../../../../differential-equation-split.md) and discarding second-order terms gives

$$
u_1''+u_1=3m_g u_0^2
=\boxed{\frac{3GM}{c^2}\frac{1-\cos2\phi}{2b^2}.}
$$

A particular solution and the complementary solution are

$$
u_1=\frac{m_g}{2b^2}(3+\cos2\phi)+A_1\cos\phi+B_1\sin\phi.
$$

Choosing $A_1=B_1=0$ retains reflection symmetry about $\phi=\pi/2$ and the specified [impact parameter](../../../../impact-parameter.md) to first order. The two distant zeros of $u$ then occur at $\phi_{\rm in}\simeq-2m_g/b$ and $\phi_{\rm out}\simeq\pi+2m_g/b$. Their separation exceeds $\pi$ by $4m_g/b$, consistently giving the [Schwarzschild light deflection](../../../../schwarzschild-light-deflection.md) $\delta\simeq4GM/(bc^2)$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
