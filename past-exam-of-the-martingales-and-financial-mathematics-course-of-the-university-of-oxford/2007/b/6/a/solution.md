<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the SDE has the required solution and $f$ is sufficiently smooth. [Itô's formula](../../../../../ito-s-lemma.md) along that solution gives

$$
df(u,X_u)=
\left(f_t+\mu f_x+\tfrac12\sigma^2f_{xx}\right)(u,X_u)du
+\sigma(u,X_u)f_x(u,X_u)dW_u.
$$

The PDE cancels the first term. Integrating from $t$ to $T$ gives

$$
\Psi(X_T)-f(t,X_t)
=\int_t^T\sigma(u,X_u)f_x(u,X_u)dW_u.
$$

If this integral is a true [martingale](../../../../../martingale-split.md), for example if its integrand has finite expected integrated square, its [conditional expectation](../../../../../conditional-expectation.md) at time $t$ is zero. For the diffusion started at $x$ at time $t$, this yields

$$
\boxed{f(t,x)=\mathbb E_{t,x}\Psi(X_T).}
$$

The notation in the question is the same Markov [conditional expectation](../../../../../conditional-expectation.md). The [martingale](../../../../../martingale-split.md) or corresponding uniform-integrability growth hypothesis is part of the usual [Feynman-Kac formula](../../../../../feynman-kac-formula.md) justification: a [local martingale](../../../../../local-martingale.md) alone does not automatically have zero expected increment. Standard smooth solutions with the customary integrability bounds satisfy this requirement.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
