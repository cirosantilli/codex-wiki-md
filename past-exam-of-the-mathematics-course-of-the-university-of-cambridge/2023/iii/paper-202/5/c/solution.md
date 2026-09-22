<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $v\in L^1(0,1)$, its [indefinite integral](../../../../../../antiderivative.md) $V$ is bounded, so $e^{-V}$ is bounded above and away from zero. Hence $\psi$ extends continuously and strictly increasingly to $[0,1]$. The quadratic-variation clock of $\psi(X)$ is

$$
\int_0^te^{-2V(X_s)}ds,
$$

whose rate is bounded above and away from zero before exit. The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) therefore identifies $\psi(X)$, up to an equivalent time change, with Brownian motion in the bounded interval $(0,\psi(1))$; in particular, $\mathcal T<\infty$ almost surely.

The bounded stopped local martingale $\psi(X_{t\wedge\mathcal T})$ is a martingale. If $q=\mathbb P_x(X_{\mathcal T}=0)$, the [optional sampling theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives

$$
\psi(x)=q\psi(0)+(1-q)\psi(1)=(1-q)\psi(1).
$$

Therefore

$$
\mathbb P_x(\mathcal T<\infty,X_{\mathcal T}=0)
=\frac{\psi(1)-\psi(x)}{\psi(1)}>0.
$$

This is the [boundary hitting probability from a diffusion scale function](../../../../../../boundary-hitting-probability-from-a-diffusion-scale-function.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
