<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In a unital [Banach algebra](../../../../../banach-algebra-split.md), the [Neumann series](../../../../../neumann-series.md) gives $(1-u)^{-1}=\sum_{k=0}^\infty u^k$ whenever $\|u\|<1$: the series converges in [norm](../../../../../norm.md) by [submultiplicativity](../../../../../submultiplicativity.md) and [completeness](../../../../../completeness.md), and multiplication of its partial sums on either side gives $1-u^{N+1}\to1$. Consequently, if $g$ is invertible and $\|g^{-1}\|\|h-g\|<1$, write

$$
h=g(1+v),\qquad v=g^{-1}(h-g).
$$

The second factor has a [Neumann series](../../../../../neumann-series.md) inverse, so $h$ is invertible. This exhibits a ball around each $g$ in the [group of invertible elements of a Banach algebra](../../../../../group-of-invertible-elements-of-a-banach-algebra.md), proving that group is an [open set](../../../../../open-set.md).

The same series proves [continuity of inversion in a Banach algebra](../../../../../continuity-of-inversion-in-a-banach-algebra.md), with the useful quantitative estimate

$$
\|h^{-1}-g^{-1}\|
=\|[(1+v)^{-1}-1]g^{-1}\|
\le\frac{\|g^{-1}\|^2\|h-g\|}{1-\|g^{-1}\|\|h-g\|}.
$$

The right side tends to zero as $h\to g$. Since applying inversion twice gives the original element, it is a [bijection](../../../../../bijection.md) whose inverse is the same [continuous](../../../../../continuous-function.md) map. Thus **inversion is a homeomorphism of the open group of invertibles onto itself**.

For the final unheaded request, define

$$
E=\{\lambda\in\mathbb C:1-\lambda a\text{ is invertible}\}.
$$

It is open by the preceding argument and contains $0$. If $\lambda_0$ were a [boundary](../../../../../boundary-of-a-set.md) point, a sequence $\lambda_n\in E$ would converge to $\lambda_0$, while openness gives $\lambda_0\notin E$. Then $1-\lambda_na\to1-\lambda_0a$ is a noninvertible limit of invertibles. The one-sided-inverse argument in part (ii) shows that this limit has neither a [left inverse of an algebra element](../../../../../left-inverse-of-an-algebra-element.md) nor a [right inverse of an algebra element](../../../../../right-inverse-of-an-algebra-element.md), contradicting the hypothesis. Therefore $E$ has empty [boundary](../../../../../boundary-of-a-set.md); it is both open and [closed](../../../../../closed-set.md) in the [connected](../../../../../connected-space.md) [complex plane](../../../../../complex-plane.md), and $E=\mathbb C$.

For every nonzero $\mu$, put $\lambda=\mu^{-1}$. The identity $\mu1-a=\mu(1-\lambda a)$ proves invertibility, so the [spectrum of an element](../../../../../spectrum-of-an-element.md) $a$ is contained in $\{0\}$. It is nonempty: if the [resolvent of an element](../../../../../resolvent-of-an-element.md) existed for all $\mu\in\mathbb C$, it would be an entire algebra-valued function tending to zero at infinity by the [Neumann series](../../../../../neumann-series.md). Applying any [bounded linear functional](../../../../../continuous-linear-functional.md) and then the [Liouville theorem](../../../../../liouville-theorem.md) would make it zero; the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) separates points and would force the resolvent itself to be zero, contradicting its inverse equation. Hence

$$
\boxed{\sigma_A(a)=\{0\}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
