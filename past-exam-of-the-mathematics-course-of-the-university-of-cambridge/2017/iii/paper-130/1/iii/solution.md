<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [cyclic logarithmic coloring](../../../../../../cyclic-logarithmic-coloring.md)

$$
\boxed{\rho(x)=\left\lfloor\log_{3/2}x\right\rfloor\pmod 3\qquad(x\geq1).}
$$

Here the [floor function](../../../../../../floor-function.md) places $x$ in the unique half-open [real interval](../../../../../../interval-mathematics.md) $[(3/2)^j,(3/2)^{j+1})$. If $y/x\in[1.9,2]$, then

$$
1<\log_{3/2}(y/x)<2,
$$

because $3/2<1.9\leq2<(3/2)^2$. For any real $t$ and $1<u<2$, $\lfloor t+u\rfloor-\lfloor t\rfloor$ is either $1$ or $2$. Applying this to the [logarithms](../../../../../../logarithm.md) of $x$ and $y$ shows that their bin indices differ by $1$ or $2$, and hence have different residues in [modular arithmetic](../../../../../../modular-arithmetic.md) modulo $3$. This proves the required separation, including both endpoints of the prescribed ratio interval. The half-open bins remove any ambiguity at their boundaries.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
