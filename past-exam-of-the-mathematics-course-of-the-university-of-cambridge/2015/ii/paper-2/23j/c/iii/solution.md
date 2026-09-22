<h1 id="23j/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $h\ne0$, enlarge the nonnegative integral $I(h)$ to all of $\mathbb R$, and substitute $y=x+|h|t$. Reflection if necessary gives

$$
I(h)\leq |h|^{1-2\alpha}C_\alpha,\qquad C_\alpha=\int_{\mathbb R}\bigl(|t-1|^{-\alpha}-|t|^{-\alpha}\bigr)^2\,dt.
$$

Near $0$ and $1$, its integrand is bounded by a constant times $1+|t|^{-2\alpha}$ or $1+|t-1|^{-2\alpha}$, which is integrable. For large $|t|$, the [mean value theorem](../../../../../../../mean-value-theorem.md) bounds the difference by a constant times $|t|^{-\alpha-1}$, whose square is integrable. Thus $C_\alpha<\infty$. The preceding estimate yields

$$
\boxed{|g(x+h)-g(x)|\leq\|f\|_2\sqrt{C_\alpha}\,|h|^{1/2-\alpha}.}
$$

In particular **$g$ is continuous on all of $\mathbb R$**; the proof establishes [Hölder continuity of a one-dimensional fractional kernel integral](../../../../../../../holder-continuity-of-a-one-dimensional-fractional-kernel-integral.md) of exponent $1/2-\alpha$ uniformly in $x$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [23J](../../../23j.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
