<h1 id="23f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
w=e^{-\Phi},
\qquad
m_R=\min_{[-R,R]}w>0,
\qquad
E_R(h)=\int_{-R}^R|h'|^2w.
$$

The [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
|h(x)-h(y)|
\leq|x-y|^{1/2}\left(\int_{-R}^R|h'|^2\right)^{1/2}
\leq m_R^{-1/2}|x-y|^{1/2}E_R(h)^{1/2}.
$$

Thus the one-half [Hölder seminorm](../../../../../../holder-seminorm.md) is at most $m_R^{-1/2}E_R(h)^{1/2}$.

Writing $Z_R=\int_{-R}^Rw>0$ and using the zero weighted mean, for each $x$ we have

$$
h(x)=\frac1{Z_R}\int_{-R}^R(h(x)-h(y))w(y)\,dy.
$$

Since $|x-y|\leq2R$, the preceding estimate yields

$$
|h(x)|\leq(2R)^{1/2}m_R^{-1/2}E_R(h)^{1/2}.
$$

Consequently the required inequality holds, for example, with

$$
\boxed{C_R=(1+\sqrt{2R})m_R^{-1/2}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [23F](../../23f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
