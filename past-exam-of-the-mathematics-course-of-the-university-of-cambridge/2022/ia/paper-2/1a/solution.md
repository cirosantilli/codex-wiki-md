<h1 id="1a/solution">Solution</h1>

↑ **Parent:** [1A](../1a.md)

[Differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) first gives

$$
I'(x)=\int_0^\pi \cos\theta\,e^{x\cos\theta}\,d\theta.
$$

On the other hand,

$$
\frac d{d\theta}\left(\sin\theta\,e^{x\cos\theta}\right)
=\cos\theta\,e^{x\cos\theta}
-x\sin^2\theta\,e^{x\cos\theta}.
$$

Its integral is zero because $\sin\theta$ vanishes at both endpoints. Hence

$$
\boxed{I'(x)=\int_0^\pi x\sin^2\theta\,e^{x\cos\theta}\,d\theta}.
$$

Differentiating once more,

$$
I''(x)=\int_0^\pi\cos^2\theta\,e^{x\cos\theta}\,d\theta.
$$

For $x\ne0$, the preceding identity and $\sin^2\theta+\cos^2\theta=1$ give

$$
I''+\frac1xI'-I
=\int_0^\pi(\cos^2\theta+\sin^2\theta-1)e^{x\cos\theta}\,d\theta=0.
$$

The equation extends through $x=0$ in its regular limiting form.

## ↑ Ancestors (10)

1. [1A](../1a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
