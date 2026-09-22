<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The clamped energy space is

$$
\mathcal H=H_0^2(-1,1)
=\{u\in H^2(-1,1):u(\pm1)=u'(\pm1)=0\}.
$$

Twice applying [integration by parts](../../../../../../integration-by-parts.md), with the boundary terms killed by the clamped conditions, gives the symmetric bilinear form

$$
a(u,v)=\int_{-1}^1
\left(pu''v''+qu'v'+ruv\right)dx.
$$

Consequently

$$
\langle Lu,u\rangle=a(u,u)
=\int_{-1}^1\left(p|u''|^2+q|u'|^2+r|u|^2\right)dx>0
$$

for every nonzero $u\in\mathcal H$: equality forces $u''=0$ almost everywhere, and the clamped boundary values then force $u=0$. Hence $L$ is symmetric and positive definite.

Strictly under the stated assumption $p\in L^2$ rather than $L^\infty$, the first integral need not be finite for every $u\in H_0^2$. The literal energy domain is therefore $\{u\in H_0^2:\sqrt p\,u''\in L^2\}$; under the usual coefficient assumption $0<p_0\leq p\leq p_1<\infty$, it is exactly $H_0^2$ and the form is coercive there.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
