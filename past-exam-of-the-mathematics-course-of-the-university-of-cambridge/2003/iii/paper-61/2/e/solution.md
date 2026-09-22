<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For a single spectral mass, the algebraic equation gives

$$
\Phi=\frac{E}{1+cE/(2\kappa)},\qquad E=e^{-\kappa x+\kappa^3t}.
$$

Differentiate the reconstruction, writing $r=cE/(2\kappa)$:

$$
q=\frac{\kappa cE}{[1+cE/(2\kappa)]^2}
=\frac{2\kappa^2r}{(1+r)^2}.
$$

With $x_0=\kappa^{-1}\log[c/(2\kappa)]$, the concise one-[soliton](../../../../../../soliton.md) answer is

$$
\boxed{q(x,t)=\frac{\kappa^2}{2}\operatorname{sech}^2\left[\frac\kappa2(x-\kappa^2t-x_0)\right].}
$$

Its speed is $\kappa^2$ and its maximum is $\kappa^2/2$. Equivalently, setting $\eta=\kappa/2$ gives $q=2\eta^2\operatorname{sech}^2[\eta(x-4\eta^2t-x_0)]$. To check the sign and speed independently, this profile obeys $q_{xx}=\kappa^2q-3q^2$ and $q_t=-\kappa^2q_x$; differentiation gives the stated [KdV equation](../../../../../../korteweg-de-vries-equation.md) exactly.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
