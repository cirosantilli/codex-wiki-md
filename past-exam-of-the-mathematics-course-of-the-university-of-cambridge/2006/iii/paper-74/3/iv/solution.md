<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For disturbances varying only along the imposed [magnetic field](../../../../../../magnetic-field.md), set $k=0$ and $x=m^2>0$. The steady [horizontal-field magnetoconvection dispersion relation](../../../../../../horizontal-field-magnetoconvection-dispersion-relation.md) becomes

$$
\boxed{R=\frac{(m^2+\pi^2)^3}{m^2}+Q(m^2+\pi^2).}
$$

Expand it in powers of $x$:

$$
R(x)=\pi^2Q+(Q+3\pi^2)x+x^2+3\pi^4+\frac{\pi^6}{x}.
$$

Its derivative and second derivative are

$$
R'(x)=Q+3\pi^2+2x-\frac{\pi^6}{x^2},\qquad
R''(x)=2+\frac{2\pi^6}{x^3}>0.
$$

Because $R$ diverges as $x\to0$ and $x\to\infty$, the unique minimum is determined by

$$
x^2(Q+3\pi^2+2x)=\pi^6.
$$

For large [Chandrasekhar number](../../../../../../chandrasekhar-number.md), this equation first gives $x\sim\pi^3Q^{-1/2}$ and hence the requested [strong-field steady magnetoconvection varying along the field](../../../../../../strong-field-steady-magnetoconvection-varying-along-the-field.md) selection law:

$$
\boxed{m_c^4\sim\frac{\pi^6}{Q}.}
$$

For the threshold through order unity, the leading $Qx+\pi^6/x$ contribution at its optimum is $2\pi^3\sqrt Q$. More precisely, the stationary equation gives

$$
x=\pi^3Q^{-1/2}\left[1-\frac{3\pi^2}{2Q}+O(Q^{-3/2})\right].
$$

The correction to $Qx+\pi^6/x$ has no first-order contribution because that expression is already stationary at its leading minimizer. Also $3\pi^2x=O(Q^{-1/2})$ and $x^2=O(Q^{-1})$. Therefore

$$
\boxed{R_{\min}(Q)=\pi^2Q+2\pi^3\sqrt Q+3\pi^4+O(Q^{-1/2}).}
$$

The constant term $3\pi^4$ must be retained. This restricted family bends [magnetic field lines](../../../../../../magnetic-field-line.md), so its large stationary threshold is compatible with the unrestricted field-aligned minimum in the preceding part.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
