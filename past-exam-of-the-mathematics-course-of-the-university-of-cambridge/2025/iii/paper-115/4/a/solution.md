<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [horizontal lift](../../../../../../horizontal-lift.md) of $\gamma$ from $p$ is a curve $\widetilde\gamma$ in $E$ projecting to $\gamma$, starting at $p$, and tangent to the horizontal distribution of the connection. In a local frame write $\widetilde\gamma(t)=(\gamma(t),v(t))$. Horizontality is the linear ordinary differential equation

$$
v'(t)+A_{\gamma(t)}(\dot\gamma(t))v(t)=0,
$$

whose initial-value theorem gives local existence and uniqueness; successive trivializations continue the lift.

A [geodesic](../../../../../../geodesic.md) satisfies $\nabla_{\dot\gamma}\dot\gamma=0$, and

$$
\exp_p(v)=\gamma_v(1)
$$

for the geodesic with initial velocity $v$. Since $d(\exp_p)_0=1$, the [inverse function theorem](../../../../../../inverse-function-theorem.md) makes $\exp_p$ a diffeomorphism near zero; its inverse gives [normal coordinates](../../../../../../normal-coordinates.md). A geodesic sphere is $\exp_p(\{v:|v|=r\})$ inside such a normal neighborhood.

The [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) states

$$
\langle d(\exp_p)_v(v),d(\exp_p)_v(w)\rangle=\langle v,w\rangle.
$$

For the variation $\gamma_s(t)=\exp_p(t(v+sw))$, let $J=\partial_s\gamma_s|_{s=0}$. The coordinate vector fields commute, so metric compatibility and constant geodesic speed give

$$
\frac d{dt}\langle\dot\gamma,J\rangle
=\frac12\partial_s|\dot\gamma_s|^2\big|_{s=0}
=\langle v,w\rangle.
$$

Since $J(0)=0$, evaluation at $t=1$ proves the formula. In particular radial and spherical directions are orthogonal.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
