<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The likelihood is

$$
p(d\mid x)=\frac1{\sqrt{2\pi\sigma^2}}
\exp\left[-\frac{(d-x)^2}{2\sigma^2}\right].
$$

Using the conditional independence $d\perp m\mid x$ and the joint prior $p(x,m)$,

$$
p(m\mid d)=
\frac{\int p(d\mid x)p(x,m)\,dx}
{\iint p(d\mid x)p(x,m)\,dx\,dm},
$$

and

$$
\mathbb E[m\mid d]=
\frac{\iint m,p(d\mid x)p(x,m)\,dx\,dm}
{\iint p(d\mid x)p(x,m)\,dx\,dm}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
