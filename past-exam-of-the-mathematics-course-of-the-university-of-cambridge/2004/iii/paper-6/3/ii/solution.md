<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A complex [Banach algebra](../../../../../../banach-algebra-split.md) is an associative complex algebra with a complete [norm](../../../../../../norm.md) satisfying [submultiplicativity](../../../../../../submultiplicativity.md), $\|ab\|\leq\|a\|\|b\|$. A [field](../../../../../../field.md) has a nonzero identity $e$, and every nonzero element is invertible. We derive the [Gelfand-Mazur theorem](../../../../../../gelfand-mazur-theorem.md) from these facts.

If $\|z\|<1$, the series $e+z+z^2+\cdots$ converges in the complete algebra. Multiplying its partial sums by $e-z$ and passing to the limit proves the [Neumann series](../../../../../../neumann-series.md) inverse. In particular, for any $x\in B$ and $|\lambda|>\|x\|$,

$$
R(\lambda)=(\lambda e-x)^{-1}
=\frac{e}{\lambda}+\sum_{n=1}^{\infty}\frac{x^n}{\lambda^{n+1}}.
$$

This [resolvent of an element](../../../../../../resolvent-of-an-element.md) tends to zero in [norm](../../../../../../norm.md) at infinity; the estimate follows from the geometric bound on $\|x^n\|$.

We next prove that the [spectrum of an element](../../../../../../spectrum-of-an-element.md) cannot be empty. Suppose every $\lambda e-x$ were invertible. At each $\lambda_0$, write

$$
\lambda e-x=(\lambda_0e-x)\big(e+(\lambda-\lambda_0)R(\lambda_0)\big).
$$

The [Neumann series](../../../../../../neumann-series.md) on a small disk about $\lambda_0$ proves that $R$ is analytic there. Consequently, for each [continuous linear functional](../../../../../../continuous-linear-functional.md) $\ell:B\to\mathbb C$, the function $\lambda\mapsto\ell(R(\lambda))$ is entire. It is bounded outside a large disk by the estimate above and bounded on that disk by [continuity](../../../../../../continuous-function.md). The [Liouville theorem](../../../../../../liouville-theorem.md) makes it constant; its zero limit at infinity makes the constant zero.

Continuous complex [linear functionals](../../../../../../linear-functional.md) separate points of $B$. Here is the needed consequence of the [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md): for $z\ne0$, define $g(tz)=t\|z\|$ on the real span of $z$ and extend it as a bounded real [linear functional](../../../../../../linear-functional.md) of [norm](../../../../../../norm.md) one. Then $\ell(w)=g(w)-ig(iw)$ is complex linear and continuous, and $\operatorname{Re}\ell(z)=\|z\|\ne0$. The real extension theorem is proved explicitly in Question 4(i) below. Thus $\ell(R(\lambda))=0$ for every $\ell$ forces $R(\lambda)=0$, contradicting $(\lambda e-x)R(\lambda)=e\ne0$. This proves the [nonemptiness of the Banach-algebra spectrum](../../../../../../nonemptiness-of-the-banach-algebra-spectrum.md).

Choose $\lambda\in\sigma_B(x)$. Since $B$ is a [field](../../../../../../field.md), the noninvertible element $x-\lambda e$ must be zero. Hence every $x\in B$ is a scalar multiple of $e$. The map

$$
\boxed{\Phi:\mathbb C\longrightarrow B,\qquad\Phi(\lambda)=\lambda e}
$$

is therefore a bijective unital complex-algebra homomorphism. It and its inverse are bounded, since $\|\lambda e\|=|\lambda|\|e\|$. Thus it is an isomorphism of [Banach algebras](../../../../../../banach-algebra-split.md). If the usual normalization $\|e\|=1$ is included in the definition, it is an isometry; without that normalization, it is still the required continuous algebra isomorphism.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
