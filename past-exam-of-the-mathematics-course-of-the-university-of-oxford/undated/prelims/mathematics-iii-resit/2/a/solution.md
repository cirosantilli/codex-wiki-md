<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $h(s)=\sin x(s)-\cos y(s)$. The [chain rule](../../../../../../chain-rule.md) gives

$$
h'=x'\cos x+y'\sin y,\qquad
f'=-h'\sin h=-(x'\cos x+y'\sin y)g.
$$

Apply the [product rule](../../../../../../product-rule.md) and the [chain rule](../../../../../../chain-rule.md) once more: $g'=h'\cos h=h'f$, and

$$
h''=x''\cos x-(x')^2\sin x+y''\sin y+(y')^2\cos y.
$$

Consequently $f''=-(h')^2f-h''g$, so the requested coefficients are

$$
\boxed{\begin{aligned}
a&=-(x'\cos x+y'\sin y)^2,\\
b&=-x''\cos x+(x')^2\sin x-y''\sin y-(y')^2\cos y.
\end{aligned}}
$$

This is the [second derivative chain rule](../../../../../../second-derivative-chain-rule.md) along the [parametric curve](../../../../../../parametric-curve.md) $(x(s),y(s))$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Mathematics III resit](../../../mathematics-iii-resit-split.md)
4. [Prelims](../../../split.md)
5. [Undated](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
