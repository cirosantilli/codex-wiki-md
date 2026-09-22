<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix the indexing convention

$$
P_i^{\ell+1}=\sum_jM_{i-aj}P_j^\ell,\qquad t_i^\ell=i/a^\ell,
$$

where the [subdivision arity](../../../../../../subdivision-arity.md) $a>1$ is an [integer](../../../../../../integer.md). A change of the initial control $P_0^0$ can influence only indices $i=j_1$ after one step, where $M_{j_1}\ne0$. After $\ell$ steps the possible descendant indices are

$$
i=a^{\ell-1}j_1+a^{\ell-2}j_2+\cdots+j_\ell.
$$

Let $j_{\min},j_{\max}$ be the smallest and largest active [subdivision mask](../../../../../../subdivision-mask.md) indices. Dividing by $a^\ell$ gives the enclosure

$$
\frac{j_{\min}}{a-1}(1-a^{-\ell})\le t_i^\ell\le\frac{j_{\max}}{a-1}(1-a^{-\ell}).
$$

Therefore the [support of a stationary subdivision scheme](../../../../../../support-of-a-stationary-subdivision-scheme.md), in initial control-grid units, is enclosed by

$$
\boxed{\left[\frac{j_{\min}}{a-1},\frac{j_{\max}}{a-1}\right],\qquad\text{width }\frac{j_{\max}-j_{\min}}{a-1}.}
$$

For the stated symmetric [subdivision mask](../../../../../../subdivision-mask.md) with active extremes $-w,w$, the width is $2w/(a-1)$. For a nonzero compactly supported basic limit function $\phi$, this is an exact endpoint calculation: its refinement equation is $\phi(x)=\sum_jM_j\phi(ax-j)$. If $\beta$ is its right support endpoint, only the largest active [subdivision mask](../../../../../../subdivision-mask.md) index can contribute sufficiently close to the rightmost point of this sum; all smaller indices have argument beyond $\beta$. Hence $\beta=(\beta+j_{\max})/a$, giving $\beta=j_{\max}/(a-1)$. The left endpoint follows in the same way. This argument also excludes cancellation at an extreme for signed [subdivision masks](../../../../../../subdivision-mask.md). The support for initial control $P_k$ is translated by $k$. If the nominal [subdivision mask](../../../../../../subdivision-mask.md) was padded by zero coefficients, use its actual extremes; and a limiting [subdivision curve](../../../../../../subdivision-curve.md) has to exist before its support is meaningful. This calculation describes the entire possible influence region, rather than the width of a single refinement stencil on its finer grid.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
