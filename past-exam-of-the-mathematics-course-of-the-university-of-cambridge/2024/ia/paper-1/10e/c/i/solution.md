<h1 id="10e/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Differentiability lets us write

$$
f(a+h)=f(a)+f'(a)h+r(h),
\qquad \frac{r(h)}h\to0,
$$

and, with $k\to0$,

$$
g(f(a)+k)=g(f(a))+g'(f(a))k+s(k),
\qquad \frac{s(k)}k\to0.
$$

Substitute $k=f(a+h)-f(a)=f'(a)h+r(h)$. Since $k=O(h)$, the remainder $s(k)$ is $o(h)$. Thus

$$
g(f(a+h))-g(f(a))
=g'(f(a))f'(a)h+o(h),
$$

and the [chain rule](../../../../../../../chain-rule.md) is

$$
\boxed{(g\circ f)'(a)=g'(f(a))f'(a)}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [10E](../../../10e.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
