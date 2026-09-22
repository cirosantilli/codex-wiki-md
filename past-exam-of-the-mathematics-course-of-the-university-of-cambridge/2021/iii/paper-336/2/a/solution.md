<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Away from $x=1/2$, the [outer solution](../../../../../../outer-expansion.md) is obtained by setting $\varepsilon=0$:

$$
y_0(x)=\left|x-\frac12\right|.
$$

It already satisfies both endpoint conditions, but its derivative jumps at $x=1/2$. Introduce the [inner variable](../../../../../../inner-variable.md)

$$
\xi=\frac{x-\frac12}{\varepsilon}
$$

and write $y=\varepsilon Y(\xi)$. The inner equation is

$$
Y''-Y=-|\xi|.
$$

Matching to the outer cusp requires $Y\sim|\xi|$ as $|\xi|\to\infty$. The even solution is

$$
Y(\xi)=|\xi|+e^{-|\xi|}.
$$

Subtracting the common part $\varepsilon|\xi|$ gives the [composite asymptotic expansion](../../../../../../additive-composite-expansion.md)

$$
\boxed{
y(x;\varepsilon)\sim
\left|x-\frac12\right|
+\varepsilon
\exp\left(-\frac{|x-\frac12|}{\varepsilon}\right)
}.
$$

Its endpoint errors are exponentially small.

At $x=1/2$, the first and second derivatives from the two sides agree, but the third derivatives have opposite signs. The composite expansion is therefore $C^2$ but not $C^3$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
