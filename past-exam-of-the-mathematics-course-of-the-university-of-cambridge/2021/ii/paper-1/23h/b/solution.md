<h1 id="23h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every [Lebesgue measurable set](../../../../../../lebesgue-measurable-set.md) $A$ differs from a [Borel set](../../../../../../borel-set.md) $B$ by a [Lebesgue-null](../../../../../../lebesgue-measure.md) set $N$. The given function $h$ is a [homeomorphism](../../../../../../homeomorphism.md) from $\mathbb R$ onto the interval $h(\mathbb R)$. Hence $h(B)$ is Borel relative to $h(\mathbb R)$ and therefore Lebesgue measurable in $\mathbb R$. Moreover,

$$
h(A)\mathbin{\triangle}h(B)\subseteq h(A\mathbin{\triangle}B)\subseteq h(N),
$$

and $h(N)$ is null by [Lusin condition N](../../../../../../lusin-condition-n.md). The [Completeness of Lebesgue measure](../../../../../../completeness-of-lebesgue-measure.md) now shows that $h(A)$ is measurable, so

$$
\nu(A):=\lambda(h(A))
$$

is defined for every $A\in\mathcal M$.

Because $h$ is [injective](../../../../../../injective-function.md), it maps pairwise disjoint sets to pairwise disjoint sets and commutes with arbitrary unions. The [countable additivity](../../../../../../countable-additivity.md) of $\lambda$ therefore gives

$$
\nu\left(\bigcup_{j=1}^{\infty}A_j\right)
=\lambda\left(\bigcup_{j=1}^{\infty}h(A_j)\right)
=\sum_{j=1}^{\infty}\lambda(h(A_j))
=\sum_{j=1}^{\infty}\nu(A_j).
$$

Thus $\nu$ is the [image-length measure of a strictly increasing continuous function](../../../../../../image-length-measure-of-a-strictly-increasing-continuous-function.md). If $\lambda(A)=0$, the null-set hypothesis gives $\nu(A)=\lambda(h(A))=0$, so

$$
\boxed{\nu\ll\lambda}.
$$

The measure is [sigma-finite](../../../../../../sigma-finite-measure.md), since

$$
\nu([-m,m])=h(m)-h(-m)<\infty.
$$

The [Radon-Nikodym theorem](../../../../../../radon-nikodym-theorem.md) consequently supplies a nonnegative locally integrable function $f$ such that

$$
\nu(A)=\int_Af\,d\lambda.
$$

For $a<x$, strict increase and continuity give

$$
h([a,x])=[h(a),h(x)]
$$

and hence

$$
h(x)-h(a)=\nu([a,x])=\int_a^x f(t)\,dt.
$$

The analogous oriented identity holds for $x<a$. By [differentiation of an indefinite Lebesgue integral](../../../../../../differentiation-of-an-indefinite-lebesgue-integral.md),

$$
\boxed{h'(x)=f(x)\quad\text{for almost every }x}.
$$

**Yes, the differentiability conclusion still holds when $h$ is merely non-decreasing.** In fact, the [Lebesgue theorem on differentiability of monotone functions](../../../../../../lebesgue-theorem-on-differentiability-of-monotone-functions.md) says that every [monotone function](../../../../../../monotonic-function.md) is differentiable almost everywhere; neither continuity nor the null-set hypothesis is needed for that conclusion. Flat intervals mean that the preceding image-set argument no longer gives disjoint images, so its natural replacement is the [Lebesgue-Stieltjes measure](../../../../../../lebesgue-stieltjes-measure.md) determined by

$$
\boxed{\mu_h((a,b])=h(b)-h(a).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [23H](../../23h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
