<h1 id="11/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The literal expression in the original PDF is undefined. Indeed, [hyperbolic tangent](../../../../../../hyperbolic-tangent.md) satisfies $\tanh w=\sinh w/\cosh w$, and

$$
\cosh(in\pi/4)=\cos(n\pi/4)=0\quad\text{when }n\equiv2\pmod4.
$$

Already the $n=2$ summand contains $\tanh(i\pi/2)$, a [pole](../../../../../../pole.md). The shifted term has the same issue when $n\equiv3\pmod4$. Thus this is not a finite sum of defined [complex numbers](../../../../../../complex-number.md), and it has **no literal real or imaginary part**. Cancelling two undefined terms is not ordinary arithmetic.

There is nevertheless a natural interpretation by [meromorphic telescoping cancellation](../../../../../../meromorphic-telescoping-cancellation.md). Insert the same small positive real shift $\varepsilon$ into every [hyperbolic tangent](../../../../../../hyperbolic-tangent.md) argument. Each term is then finite, and the [telescoping sum](../../../../../../telescoping-sum.md) is

$$
S(\varepsilon)=\tanh(\varepsilon+121i\pi/4)-\tanh\varepsilon.
$$

Since [hyperbolic tangent](../../../../../../hyperbolic-tangent.md) has period $i\pi$, its first argument can be reduced to $\varepsilon+i\pi/4$. Taking the [limit](../../../../../../limit-of-a-function.md) gives

$$
\boxed{\lim_{\varepsilon\to0^+}S(\varepsilon)=i,\qquad\Re=0,\quad\Im=1.}
$$

This is a common-shift continuation of the sum, plausibly the intended telescoping answer. It requires that additional convention; it is not the value of the expression as printed.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [11](../../../11.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
