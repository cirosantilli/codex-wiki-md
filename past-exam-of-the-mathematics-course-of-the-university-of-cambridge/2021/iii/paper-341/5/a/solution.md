<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the operator in [Sturm-Liouville form](../../../../../../sturm-liouville-form.md):

$$
Lu=-\bigl((1+x^2)u'\bigr)'+x^2u.
$$

The natural solution space is the [Sobolev space](../../../../../../sobolev-space-split.md) $H_0^1(0,1)$. Multiplication by a test function $v\in H_0^1(0,1)$ and integration by parts gives the symmetric bilinear form

$$
a(u,v)=\int_0^1
\left[(1+x^2)u'v'+x^2uv\right]dx.
$$

It is bounded and

$$
a(u,u)\geq\int_0^1|u'|^2dx
\geq C\|u\|_{H^1}^2
$$

by the [Poincaré inequality](../../../../../../poincare-inequality.md). Thus $L$ is positive definite and $a$ is coercive. The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) gives a unique weak solution of the variational problem

$$
\boxed{
\text{find }u\in H_0^1(0,1)
\text{ such that }
a(u,v)=\int_0^1fv\,dx
\quad\text{for every }v\in H_0^1(0,1).
}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
