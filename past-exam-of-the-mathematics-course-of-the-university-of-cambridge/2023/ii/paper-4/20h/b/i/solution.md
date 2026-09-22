<h1 id="20h/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $K=\mathbb Q(\sqrt{10})$, the [ring of integers of a quadratic field](../../../../../../../ring-of-integers-of-a-quadratic-field.md) is

$$
\mathcal O_K=\mathbb Z[\sqrt{10}].
$$

The element

$$
\varepsilon=3+\sqrt{10}
$$

has [field norm](../../../../../../../field-norm.md) $9-10=-1$, so it is a [unit](../../../../../../../unit-from-norm-one-or-minus-one.md). We claim that

$$
\mathcal O_K^\times
=\{\mathord\pm\varepsilon^n:n\in\mathbb Z\}.
$$

Let $u$ be any unit. Its norm is $\pm1$. After changing its sign and replacing it by its inverse if necessary, its first real embedding satisfies $u\geq1$. Choose $n\in\mathbb Z$ so that

$$
1\leq v=u\varepsilon^{-n}<\varepsilon.
$$

Write $v=a+b\sqrt{10}$ with $a,b\in\mathbb Z$. Its conjugate is $v'=\pm v^{-1}$, so $|v'|\leq1$. Therefore

$$
|a|=\frac{|v+v'|}{2}<\frac{\varepsilon+1}{2}<4,
\qquad
|b|=\frac{|v-v'|}{2\sqrt{10}}
<\frac{\varepsilon+1}{2\sqrt{10}}<2.
$$

Thus $|a|\leq3$ and $|b|\leq1$. The equation $a^2-10b^2=\pm1$ now shows directly that the only value in $[1,\varepsilon)$ is $v=1$: if $b=0$ then $a=\pm1$, while if $|b|=1$ then $a=\pm3$ and the positive possibilities are either below $1$ or equal to $\varepsilon$. Hence $u=\varepsilon^n$ after normalization, proving the claimed description of the [units of Q of square root ten](../../../../../../../units-of-q-of-square-root-ten.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [20H](../../../20h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
