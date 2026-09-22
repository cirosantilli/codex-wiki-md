<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The expansion is singular near the moving lower limit, so expanding $e^{-\varepsilon/x}$ throughout the original [integral](../../../../../../integral.md) would lose its constant term. Introduce the symmetric [exponential integral](../../../../../../exponential-integral.md)

$$
J(\varepsilon)=\int_0^\infty\frac{e^{-x-\varepsilon/x}}x\,dx.
$$

Under $x=\varepsilon/t$, the discarded piece becomes

$$
J-I=\int_1^\infty\frac{e^{-t-\varepsilon/t}}t\,dt=\beta-\varepsilon\int_1^\infty\frac{e^{-t}}{t^2}\,dt+O(\varepsilon^2)=\beta-\varepsilon(e^{-1}-\beta)+O(\varepsilon^2).
$$

This is a uniform [Taylor expansion](../../../../../../taylor-expansion.md) because $t\geq1$. To derive the [logarithmic expansion of a symmetric exponential integral](../../../../../../logarithmic-expansion-of-a-symmetric-exponential-integral.md) without needing another special function, first exploit the same substitution to write

$$
J=2\int_{\sqrt\varepsilon}^\infty\frac{e^{-x-\varepsilon/x}}x\,dx=2E(\sqrt\varepsilon)+O(\sqrt\varepsilon)=-\log\varepsilon-2\gamma+o(1).
$$

The estimate follows from $0\leq1-e^{-\varepsilon/x}\leq\varepsilon/x$. Here $\gamma$ is [Euler's constant](../../../../../../euler-s-constant.md) and the [small-argument expansion of the exponential integral](../../../../../../small-argument-expansion-of-the-exponential-integral.md) fixes the constant as well as the logarithm.

Differentiate under the integral and integrate the derivative of $e^{-x-\varepsilon/x}/x$ over $(0,\infty)$; the exponentially small endpoint terms vanish. This gives the [ordinary differential equation](../../../../../../ordinary-differential-equation.md)

$$
\varepsilon J''+J'=J.
$$

For the [Frobenius method](../../../../../../frobenius-method.md) at its [regular singular point](../../../../../../regular-singular-point.md), write $J=A\log\varepsilon+B+\varepsilon(C_1\log\varepsilon+D)+\cdots$. Substitution gives $C_1=A$ and $D=B-2A$. The preceding leading calculation sets $A=-1$, $B=-2\gamma$, hence

$$
J=-\log\varepsilon-2\gamma+\varepsilon[-\log\varepsilon+2-2\gamma]+O(\varepsilon^2|\log\varepsilon|).
$$

Subtracting the [moving-cutoff correction to a symmetric exponential integral](../../../../../../moving-cutoff-correction-to-a-symmetric-exponential-integral.md) yields the requested answer, including the logarithmically enhanced first-order term:

$$
\boxed{I(\varepsilon)=-\log\varepsilon-2\gamma-\beta+\varepsilon[-\log\varepsilon+2-2\gamma+e^{-1}-\beta]+O(\varepsilon^2|\log\varepsilon|).}
$$

Thus the $\varepsilon\log\varepsilon$ [switchback term](../../../../../../switchback-term.md) must be retained when asking for all contributions through order $\varepsilon$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
