<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Applying the [conditional multivariate normal distribution](../../../../../../conditional-multivariate-normal-distribution.md) to the two differences gives, more generally,

$$
D_1\mid D_2=d\sim N\!\left(\frac{b-c}{a-c}d,\ 2(a-c)-\frac{[2(b-c)]^2}{2(a-c)}\right).
$$

At $d=0$ the result is

$$
\boxed{X_1-Y_1\mid X_2-Y_2=0\sim N\!\left(0,\ \frac{2(a-b)(a+b-2c)}{a-c}\right).}
$$

Both this law and the marginal law have mean zero, but the [conditional variance](../../../../../../conditional-variance.md) is smaller. Specifically, with $\rho=(b-c)/(a-c)$, the [conditional variance](../../../../../../conditional-variance.md) is the marginal [variance](../../../../../../variance-split.md) times $1-\rho^2$. The assumptions imply $0<\rho<1$, so the decrease is strict. Matching the breadth differences to zero gives information about the correlated length differences; it does not force the length differences themselves to be zero. The residual uncertainty remains positive. The original PDF has the between-son differences used here; the self-subtractions in the converted TeX are transcription errors.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
