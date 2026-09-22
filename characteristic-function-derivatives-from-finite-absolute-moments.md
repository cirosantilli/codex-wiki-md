# Characteristic-function derivatives from finite absolute moments

↑ **Parent:** [Characteristic function](characteristic-function-split.md)

If $m\geq1$ is an [integer](integer-split.md) and $\mathbb E[|X|^m]<\infty$, the [characteristic function](characteristic-function-split.md) has continuous [derivatives](derivative.md) through order $m$, with

$$
\varphi_X^{(k)}(t)=\mathbb E[(iX)^ke^{itX}],\qquad
\varphi_X^{(k)}(0)=i^k\mathbb E[X^k],\qquad 1\leq k\leq m.
$$

Thus finite [absolute moments](absolute-moment.md) justify recovering [moments](moment.md) from [derivatives](derivative.md).[§3.3.3, Theorem 3.3.18, printed p. 134](probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

For a short justification of [differentiation under the integral sign](differentiation-under-the-integral-sign.md), the difference quotient for the $(k-1)$st [derivative](derivative.md) has integrand $(iX)^{k-1}e^{itX}(e^{ihX}-1)/h$. Its absolute value is at most $|X|^k$, since $|e^{iu}-1|\leq|u|$ for real $u$. Lower [absolute moments](absolute-moment.md) are finite because $|X|^k\leq1+|X|^m$. Apply the [dominated convergence theorem](dominated-convergence-theorem.md) successively, then use the same integrable bound to obtain [continuity](continuous-function.md) of each [derivative](derivative.md).

For the [Bernoulli distribution](bernoulli-distribution.md) with parameter $1/3$, direct [differentiation](differentiation.md) gives $\varphi_B'(0)=i/3$ and $\varphi_B''(0)=-1/3$, agreeing with $\mathbb E[B]=\mathbb E[B^2]=1/3$. Its [variance](variance-split.md) is therefore $1/3-(1/3)^2=2/9$. Existence and [continuity of a characteristic function](continuity-of-a-characteristic-function.md) alone do not authorize these [moment](moment.md) calculations: the standard [Cauchy distribution](cauchy-distribution.md), whose [expected value](expected-value-split.md) is undefined, still has a [characteristic function](characteristic-function-split.md). The stated finite [absolute moment](absolute-moment.md) hypothesis is a sufficient condition for the [derivative](derivative.md) formula, not an assumption built into the definition of a [characteristic function](characteristic-function-split.md).

## ↑ Ancestors (6)

1. [Characteristic function](characteristic-function-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
