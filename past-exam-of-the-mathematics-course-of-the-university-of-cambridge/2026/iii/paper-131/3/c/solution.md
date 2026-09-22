<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On $p$-forms in dimension $n$, the defining identity for the [Hodge star operator](../../../../../../hodge-star-operator.md) gives

$$
*^2=(-1)^{p(n-p)}.
$$

For $n=4$ and $p=2$, therefore, $*^2=1$. For every $\alpha\in\Omega^2(N)$ define

$$
\alpha_+=\frac12(\alpha+*\alpha),
\qquad
\alpha_-=\frac12(\alpha-*\alpha).
$$

Then $*\alpha_+=\alpha_+$, $*\alpha_-=-\alpha_-$, and $\alpha=\alpha_++\alpha_-$. The two eigenspaces of the involution $*$ have zero intersection, which proves uniqueness. They are respectively the spaces of [self-dual](../../../../../../self-dual-differential-form.md) and [anti-self-dual](../../../../../../anti-self-dual-differential-form.md) two-forms.

Now suppose $N$ is compact and let $\beta$ be an [exact](../../../../../../exact-differential-form.md) three-form, say $\beta=d\theta$. Apply the [Hodge decomposition theorem](../../../../../../hodge-decomposition-theorem.md) to the two-form $\theta$:

$$
\theta=h+d\varphi+\delta\psi.
$$

Set $a=\delta\psi$. Then $da=d\theta=\beta$ and $\delta a=\delta^2\psi=0$. For a two-form in dimension four, $\delta=-*d*$, so $d*a=0$. The self-dual form

$$
\eta=a+*a
$$

satisfies

$$
*\eta=*a+*^2a=\eta,
\qquad
d\eta=da+d*a=\beta.
$$

**Thus every exact three-form is the [exterior derivative](../../../../../../exterior-derivative.md) of a self-dual two-form.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 131](../../../paper-131-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
