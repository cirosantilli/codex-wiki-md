<h1 id="11e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First $g(b)\ne g(a)$: otherwise [Rolle's theorem](../../../../../../rolle-theorem.md) would produce a point with $g'=0$, contrary to the hypothesis. Define

$$
h(t)=[f(b)-f(a)][g(t)-g(a)]-[g(b)-g(a)][f(t)-f(a)].
$$

It is [continuous](../../../../../../continuous-function.md) on $[a,b]$, [differentiable](../../../../../../differentiable-function.md) inside, and vanishes at both endpoints. [Rolle's theorem](../../../../../../rolle-theorem.md) gives a $\xi\in(a,b)$ with

$$
[f(b)-f(a)]g'(\xi)-[g(b)-g(a)]f'(\xi)=0.
$$

The two denominators are nonzero, so this proves [Cauchy's mean value theorem](../../../../../../cauchy-mean-value-theorem.md):

$$
\boxed{\frac{f'(\xi)}{g'(\xi)}=\frac{f(b)-f(a)}{g(b)-g(a)}.}
$$

When $f(a)=g(a)=0$, apply that theorem on $[a,x]$ for each $a<x\leq b$. [Rolle's theorem](../../../../../../rolle-theorem.md) again ensures $g(x)\ne0$, and some $\xi_x\in(a,x)$ satisfies $f(x)/g(x)=f'(\xi_x)/g'(\xi_x)$. As $x\downarrow a$, the trapped point $\xi_x$ also tends to $a$. Therefore

$$
\boxed{\frac{f(x)}{g(x)}\longrightarrow\ell\quad\text{as }x\downarrow a.}
$$

This proves the stated endpoint case of [L'Hôpital's rule](../../../../../../l-hopital-s-rule.md). It does not assume [continuity](../../../../../../continuous-function.md) of the derivatives; only the indicated derivative-ratio limit is used. The same trapping argument also works for an extended infinite limit if that convention is allowed.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [11E](../../11e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
