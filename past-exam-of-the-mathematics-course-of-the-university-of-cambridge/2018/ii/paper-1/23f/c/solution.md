<h1 id="23f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The relation $1/q=1/p-\alpha/n>0$ implies $\alpha p<n$. Fix $r>0$ and split the [Riesz potential](../../../../../../riesz-potential.md) into the regions $|x-y|<r$ and $|x-y|\geq r$.

For the near part, decompose the ball into the dyadic annuli

$$
2^{-k-1}r\leq|x-y|<2^{-k}r,
\qquad k\geq0.
$$

The definition of the [Hardy-Littlewood maximal function](../../../../../../hardy-littlewood-maximal-function.md) then gives

$$
\int_{|x-y|<r}\frac{|f(y)|}{|x-y|^{n-\alpha}}\,dy
\leq C_{n,\alpha}r^\alpha Mf(x)
\sum_{k=0}^\infty2^{-k\alpha}
\leq C r^\alpha Mf(x).
$$

For the far part, [Hölder's inequality](../../../../../../holder-s-inequality.md) gives

$$
\begin{aligned}
\int_{|x-y|\geq r}\frac{|f(y)|}{|x-y|^{n-\alpha}}\,dy
&\leq\lVert f\rVert_p
\left(\int_{|z|\geq r}|z|^{-(n-\alpha)p'}\,dz\right)^{1/p'}\\
&\leq C\lVert f\rVert_p r^{\alpha-n/p},
\end{aligned}
$$

where convergence follows from $\alpha p<n$.

If $Mf(x)>0$, choose

$$
r^{n/p}=\frac{\lVert f\rVert_p}{Mf(x)}.
$$

The two bounds then have the same size. If $Mf(x)=0$, the result is immediate. Consequently the [Hedberg inequality](../../../../../../hedberg-inequality.md) is

$$
\boxed{\ I_\alpha|f|(x)
\leq C_{n,p,\alpha}
\lVert f\rVert_p^{\alpha p/n}
(Mf(x))^{1-\alpha p/n}.\ }
$$

Here the dimensional constant is required for the unnormalized kernel and Lebesgue measure used in the question.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [23F](../../23f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
