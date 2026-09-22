<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [reflection extension from a half-space](../../../../../../reflection-extension-from-a-half-space.md)

$$
(Eu)(x,y)=u(|x|,y).
$$

It is plainly linear and restricts to $u$ on $U$. For a smooth $u$, the [chain rule](../../../../../../chain-rule.md) gives

$$
D_x(Eu)(x,y)=\operatorname{sgn}(x)(D_xu)(|x|,y),
\qquad
D_y(Eu)(x,y)=(D_yu)(|x|,y).
$$

A change of variables therefore gives

$$
\|Eu\|_{W^{1,p}(\mathbb R^2)}^p
=2\|u\|_{W^{1,p}(U)}^p
$$

for $p<\infty$, with the evident equality of essential suprema for $p=\infty$. Approximate a general $u$ by the smooth functions from part c. The estimate makes their reflections Cauchy in $W^{1,p}(\mathbb R^2)$, and their limit defines a bounded [Sobolev extension operator](../../../../../../sobolev-extension-operator.md) with $\|E\|\leq2^{1/p}$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
