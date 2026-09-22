<h1 id="1/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [heat equation](../../../../../../../heat-equation.md), viewed as a second-order equation in all $(t,x)$ variables, the [principal symbol](../../../../../../../principal-symbol-of-a-partial-differential-equation.md) is $|\xi|^2$. It vanishes on $dt$, so $t=0$ is a [characteristic hypersurface](../../../../../../../characteristic-hypersurface.md) and

$$
\boxed{\text{the ordinary Cauchy-Kovalevskaya theorem does not apply at }t=0.}
$$

Writing $u_t=\Delta_xu$ does not repair its hypotheses: the right side has second spatial [derivatives](../../../../../../../derivative.md), exceeding the first-order normal-form allowance. Indeed [real analytic](../../../../../../../real-analytic-function.md) initial data need not produce a jointly [real analytic](../../../../../../../real-analytic-function.md) solution through time zero. In one dimension, $u_0(x)=(1+x^2)^{-1}$ would force

$$
\partial_t^ku(0,0)=\partial_x^{2k}u_0(0)=(-1)^k(2k)!.
$$

The time Taylor coefficients $(-1)^k(2k)!/k!$ have zero radius of convergence.

Nevertheless the forward [heat equation](../../../../../../../heat-equation.md) has [Hadamard well-posedness](../../../../../../../well-posed-problem.md) in standard $L^2$ or [Sobolev space](../../../../../../../sobolev-space-split.md) classes for $t\ge0$; its [Fourier multiplier](../../../../../../../fourier-multiplier.md) $e^{-t|\xi|^2}$ gives stable smoothing. Backward evolution has the growing multiplier $e^{|t||\xi|^2}$ and is unstable. Neither forward stability nor backward instability is decided simply by whether the [real analytic](../../../../../../../real-analytic-function.md) theorem applies.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
