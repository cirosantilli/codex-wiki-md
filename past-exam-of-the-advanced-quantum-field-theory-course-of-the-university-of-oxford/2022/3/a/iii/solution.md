<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For any fixed $r\geq0$, the source contribution obeys $c\phi_1\geq cr$, because $c<0$ and $\phi_1\leq r$. Equality occurs only at $(\phi_1,\phi_2,\phi_3)=(r,0,0)$ when $r>0$. Thus the global [ground state](../../../../../ground-state.md) lies on the positive first axis. Minimize there:

$$
f(r)=-\frac12\mu^2r^2+\frac14\lambda r^4+cr,\qquad
f'(r)=\lambda r^3-\mu^2r+c.
$$

For $0\leq r\leq v=\mu/\sqrt\lambda$, $f'(r)<0$. For $r>v$, $f''(r)=3\lambda r^2-\mu^2>0$, so $f'$ increases strictly from $c$ to $+\infty$. There is exactly one root $\tilde v>v$, and it is the unique global minimum. Therefore

$$
\boxed{\langle\boldsymbol\phi\rangle=(\tilde v,0,0),\qquad
\lambda\tilde v^3-\mu^2\tilde v+c=0,\qquad \tilde v>\frac\mu{\sqrt\lambda}>0.}
$$

This argument selects the true [ground state](../../../../../ground-state.md) even if the full cubic has additional negative stationary roots.

Expand $\phi_1=\tilde v+h$, $\phi_2=\pi_2$, $\phi_3=\pi_3$. The source is linear, so it shifts the expansion point but has zero [Hessian matrix](../../../../../hessian-matrix.md). The [scalar mass matrix](../../../../../scalar-mass-matrix.md) is diagonal at the new [vacuum expectation value](../../../../../vacuum-expectation-value.md):

$$
m_h^2=-\mu^2+3\lambda\tilde v^2,\qquad
m_{\pi_2}^2=m_{\pi_3}^2=-\mu^2+\lambda\tilde v^2.
$$

Eliminating $\lambda$ with the stationary equation gives

$$
\boxed{m_h^2=2\mu^2-\frac{3c}{\tilde v},\qquad
m_{\pi_2}^2=m_{\pi_3}^2=-\frac c{\tilde v}.}
$$

All three squared [masses](../../../../../mass.md) are positive. The [masses](../../../../../mass.md) themselves are the positive square roots of these expressions.

The source explicitly reduces the stated [SO(3)](../../../../../so-3-group.md) [symmetry](../../../../../symmetry-physics.md) to [SO(2)](../../../../../special-orthogonal-group-in-two-dimensions.md); the selected [vacuum state](../../../../../vacuum-state.md) preserves that remaining [SO(2)](../../../../../special-orthogonal-group-in-two-dimensions.md). There is consequently no spontaneously broken exact continuous [global symmetry in field theory](../../../../../global-symmetry-in-field-theory.md) to which the [Goldstone theorem](../../../../../goldstone-theorem.md) applies. For small $|c|$, the two angular excitations are [pseudo-Goldstone bosons](../../../../../pseudo-goldstone-boson.md). Their squared [masses](../../../../../mass.md) vanish as $c\to0^-$, while $\tilde v\to\mu/\sqrt\lambda$ and $m_h^2\to2\mu^2$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the advanced quantum field theory course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory course of the University of Oxford](../../../../../advanced-quantum-field-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
