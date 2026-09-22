<h1 id="11d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
m=\frac{f(b)-f(a)}{b-a},\qquad
h(x)=f(x)-f(a)-m(x-a).
$$

Then $h(a)=h(b)=0$. Since $f$ is not linear, $h(c)\ne0$ for some $c\in(a,b)$. If $h(c)>0$, the [mean value theorem](../../../../../../mean-value-theorem.md) on $[a,c]$ gives a point $\xi$ with

$$
h'(\xi)=\frac{h(c)-h(a)}{c-a}>0.
$$

If $h(c)<0$, apply it on $[c,b]$ to obtain

$$
h'(\xi)=\frac{h(b)-h(c)}{b-c}>0.
$$

In either case $h'=f'-m$, and therefore

$$
\boxed{f'(\xi)>\frac{f(b)-f(a)}{b-a}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11D](../../11d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
