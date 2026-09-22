<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $\theta=\sqrt{p+\sqrt p}$. Then $(\theta^2-p)^2=p$, so $\theta$ is a root of

$$
F(X)=X^4-2pX^2+p^2-p.
$$

This [polynomial](../../../../polynomial-split.md) satisfies [Eisenstein's criterion](../../../../eisenstein-criterion.md) at $p$: every nonleading coefficient is divisible by $p$, while the constant coefficient $p(p-1)$ is not divisible by $p^2$. Therefore

$$
\boxed{m_\theta(X)=X^4-2pX^2+p^2-p,\qquad[\mathbb Q(\theta):\mathbb Q]=4.}
$$

Now suppose $p=n^2+1$, taking $n>0$ without loss of generality. Let $\beta=\sqrt{p-\sqrt p}$. Since $\theta\beta=n\sqrt p$ and $\sqrt p=\theta^2-p$,

$$
\beta=\frac{n(\theta^2-p)}\theta\in\mathbb Q(\theta).
$$

Consequently all four distinct roots $\pm\theta,\pm\beta$ lie in this [field](../../../../field.md). This gives a [cyclic quartic field from a nested quadratic radical](../../../../cyclic-quartic-field-from-a-nested-quadratic-radical.md). It is a [splitting field](../../../../splitting-field.md) in [characteristic zero](../../../../characteristic-zero.md), hence a [normal extension](../../../../normal-extension.md) and a [Galois extension](../../../../finite-galois-extension.md).

There is a [Galois automorphism](../../../../automorphism-of-a-field-extension.md) $\sigma$ sending $\theta$ to $\beta$: a root image defines an embedding, and normality makes it an automorphism of the [splitting field](../../../../splitting-field.md). It sends $\sqrt p=\theta^2-p$ to $-\sqrt p$, so

$$
\sigma(\beta)=\frac{-n\sqrt p}{\beta}=-\theta.
$$

Thus $\theta\mapsto\beta\mapsto-\theta\mapsto-\beta\mapsto\theta$ is a four-cycle. The [Galois group](../../../../galois-group.md) has order four and contains an element of order four, giving

$$
\boxed{\operatorname{Gal}(\mathbb Q(\theta)/\mathbb Q)\cong C_4.}
$$

For the requested lower degrees, $(q,r)=(3,4)$ gives $\sqrt{q+\sqrt r}=\sqrt5$ and degree two; $(q,r)=(3,1)$ gives $2$ and degree one. Both pairs use positive [integers](../../../../integer-split.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
