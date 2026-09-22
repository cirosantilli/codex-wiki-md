<h1 id="5k/solution">Solution</h1>

↑ **Parent:** [5K](../5k.md)

The [normal linear model](../../../../../normal-linear-model.md) is $Y=X\beta+\varepsilon$ with $\varepsilon\sim N(0,\sigma^2I_n)$. Full column rank gives

$$
\widehat\beta=(X^TX)^{-1}X^TY.
$$

With hat [matrix](../../../../../matrix.md) $H=X(X^TX)^{-1}X^T$, the $i$th [regression leverage](../../../../../regression-leverage.md) is $h_{ii}$. Since $e=(I-H)Y=(I-H)\varepsilon$ and $I-H$ is an orthogonal projection,

$$
\operatorname{Var}(e_i)=\sigma^2(1-h_{ii}).
$$

High-leverage observations can move their own fitted values strongly and may exert disproportionate influence; residual size alone can therefore conceal them.

## ↑ Ancestors (10)

1. [5K](../5k.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
