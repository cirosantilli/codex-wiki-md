<h1 id="32a/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The exact second-iterate equation factors as

$$
F(F(x))-x
=x(\lambda x^2-\lambda-1)(\lambda x^2-\lambda+1)
(\lambda^2x^4-\lambda^2x^2+1).
$$

The positive nonfixed period-two points come from the final factor. If $y=x^2$, their squared values are

$$
y_\pm=\frac{1\pm\sqrt{1-4/\lambda^2}}2,
\qquad
y_++y_-=1,
\qquad
y_+y_-=\frac1{\lambda^2}.
$$

They are real and distinct for $\lambda>2$.

The [multiplier of a periodic orbit of an iteration](../../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) is

$$
F'(x_+)F'(x_-)
=\lambda^2(1-3y_+)(1-3y_-)
=\lambda^2\left(1-3(y_++y_-)+9y_+y_-\right)
=9-2\lambda^2.
$$

For $\lambda=2+\mu$ with $0<\mu\ll1$,

$$
9-2\lambda^2=1-8\mu+O(\mu^2),
$$

whose modulus is less than one. The new two-cycle is therefore locally asymptotically stable.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [32A](../../32a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
