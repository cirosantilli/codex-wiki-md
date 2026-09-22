<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
D(x)=x(x+\varepsilon)+\varepsilon^3e^{-x^2},
\qquad
D_0(x)=x(x+\varepsilon)+\varepsilon^3.
$$

The inequality $|1-e^{-x^2}|\leq x^2$ and a split into $0<x<\varepsilon^2$, $\varepsilon^2<x<\varepsilon$, and $\varepsilon<x<1$ show that

$$
\int_0^1\left|\frac1D-\frac1{D_0}\right|dx
\leq C\int_0^1\frac{\varepsilon^3x^2}{D_0(x)^2}\,dx
=O(\varepsilon^2).
$$

Thus replacing the exponential by one does not affect any term through $O(1)$.

Factor

$$
D_0(x)=(x+a)(x+b),
$$

where

$$
a=\frac{\varepsilon}{2}
\left(1-\sqrt{1-4\varepsilon}\right),
\qquad
b=\frac{\varepsilon}{2}
\left(1+\sqrt{1-4\varepsilon}\right).
$$

[Partial fraction decomposition](../../../../../../partial-fraction-decomposition.md) gives

$$
\int_0^1\frac{dx}{D_0(x)}
=\frac{1}{\varepsilon\sqrt{1-4\varepsilon}}
\left[
\log\frac ba+
\log\frac{1+a}{1+b}
\right].
$$

The required [asymptotic expansion](../../../../../../asymptotic-expansion.md) follows from

$$
\frac1{\sqrt{1-4\varepsilon}}
=1+2\varepsilon+O(\varepsilon^2),
$$



$$
\log\frac ba=-\log\varepsilon-2\varepsilon
+O(\varepsilon^2),
\qquad
\log\frac{1+a}{1+b}=-\varepsilon+O(\varepsilon^2).
$$

Therefore

$$
\boxed{
I(\varepsilon)
=\frac{\log(1/\varepsilon)}{\varepsilon}
+2\log(1/\varepsilon)-3+o(1).}
$$

The two small roots reveal the same nested scales $x=O(\varepsilon^2)$ and $x=O(\varepsilon)$ that a [divide-and-conquer asymptotic expansion](../../../../../../divide-and-conquer-asymptotic-expansion.md) would match explicitly.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
