<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the convention

$$
P_\tau(x)=\operatorname{prox}_{\tau f}(x)
=\arg\min_u\left\{f(u)+\frac1{2\tau}\|x-u\|_2^2\right\}.
$$

This [proximal map](../../../../../../proximal-operator.md) is also the [resolvent of a monotone operator](../../../../../../resolvent-of-a-monotone-operator.md) $(I+\tau\partial f)^{-1}$. A proper [lower semicontinuous](../../../../../../lower-semicontinuity.md) [convex function](../../../../../../convex-function.md) has an [affine minorant](../../../../../../affine-minorant.md), so the quadratic term makes this minimization coercive and [strongly convex](../../../../../../strongly-convex-function.md). A unique minimizer exists for every $x$. Its [subgradient optimality condition](../../../../../../subgradient-optimality-condition.md) is

$$
\frac{x-P_\tau(x)}\tau\in\partial f(P_\tau(x)).
$$

The [Moreau–Yosida regularisation](../../../../../../moreau-envelope.md) is $f_\tau=f\mathbin\square g^\tau$. The [conjugate of an infimal convolution](../../../../../../conjugate-of-an-infimal-convolution.md) and the quadratic conjugate give

$$
f_\tau^*(p)=f^*(p)+\frac\tau2\|p\|_2^2.
$$

The factor $\tau$ here is essential. Apply [subgradient inversion under convex conjugacy](../../../../../../subgradient-inversion-under-convex-conjugacy.md), followed by the [subdifferential sum rule](../../../../../../subdifferential-sum-rule.md) with the everywhere differentiable quadratic:

$$
\begin{aligned}
p\in\partial f_\tau(x)
&\iff x\in\partial f_\tau^*(p)\\
&\iff x-\tau p\in\partial f^*(p)\\
&\iff p\in\partial f(x-\tau p)\\
&\iff x-\tau p=P_\tau(x).
\end{aligned}
$$

The last equivalence is precisely the unique proximal minimization condition. Thus

$$
\boxed{\partial f_\tau(x)=\left\{\frac{x-\operatorname{prox}_{\tau f}(x)}\tau\right\}}.
$$

This proves both existence and uniqueness of the [subgradient](../../../../../../subgradient.md), rather than only identifying a possible element. The finite [convex function](../../../../../../convex-function.md) $f_\tau$ is therefore differentiable, with **$\nabla f_\tau=(I-P_\tau)/\tau$**, the [gradient of a Moreau envelope](../../../../../../gradient-of-a-moreau-envelope.md).

For completeness, monotonicity of $\partial f$ applied to the two proximal conditions gives

$$
\langle P_\tau(x)-P_\tau(y),x-y\rangle\geq\|P_\tau(x)-P_\tau(y)\|_2^2.
$$

Hence $P_\tau$ is [firmly nonexpansive](../../../../../../firmly-nonexpansive-mapping.md). Expanding the same inequality shows that $I-P_\tau$ is [firmly nonexpansive](../../../../../../firmly-nonexpansive-mapping.md) too. In particular, **$\nabla f_\tau$ is $1/\tau$-Lipschitz continuous**. None of this requires a bounded [effective domain](../../../../../../effective-domain.md); the result applies to the next example as well.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
