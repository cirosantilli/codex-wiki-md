<h1 id="11e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A map $f:A\to\mathbb R^m$ is differentiable at $p\in A$ when there is a [linear map](../../../../../../linear-map.md) $Df(p):\mathbb R^n\to\mathbb R^m$ such that

$$
f(p+h)=f(p)+Df(p)h+r(h),
\qquad
\frac{|r(h)|}{|h|}\longrightarrow0.
$$

The linear map $Df(p)$ is the [Fréchet derivative](../../../../../../frechet-derivative.md) of $f$ at $p$.

The multivariable [chain rule](../../../../../../chain-rule.md) states that if $f$ is differentiable at $p$ and $g$ is differentiable at $f(p)$, then

$$
\boxed{D(g\circ f)(p)=Dg(f(p))\circ Df(p)}.
$$

Indeed, write $f(p+h)=f(p)+Ah+r(h)$ and $g(f(p)+k)=g(f(p))+Bk+s(k)$, where $r(h)=o(|h|)$ and $s(k)=o(|k|)$. Since $k=Ah+r(h)=O(|h|)$,

$$
g(f(p+h))=g(f(p))+BAh+Br(h)+s(Ah+r(h)),
$$

and the last two terms are $o(|h|)$. This proves the formula.

For matrix inversion near the [identity matrix](../../../../../../identity-matrix.md),

$$
(I+h)^{-1}=I-h+h^2(I+h)^{-1}.
$$

The last term is $O(\|h\|^2)$ because inversion is bounded near $I$. Therefore the inversion map is differentiable at $I$ and

$$
\boxed{Df(I)(h)=-h}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11E](../../11e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
