<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Suppose the starting steps satisfy the nonnegative-weight restrictions given below, the volatility is bounded away from zero, and the coefficients and pricing solution have the regularity needed for the usual error expansion at the monitored positive remaining maturity. The combined refinement $h\mapsto h/2$, $k\mapsto k/4$ preserves $k/h^2$, improves the spatial drift restriction, and yields

$$
u_{h,k}=u+C_xh^2+C_tk+o(h^2+k).
$$

If $k=\rho h^2$, put $C=C_x+\rho C_t$. Then $u_h=u+Ch^2+o(h^2)$, so the difference between successive refinement levels is $3Ch^2/4+o(h^2)$. Consequently **successive differences shrink by a factor of approximately four**, giving second-order convergence in space and first-order convergence in time. If the leading coefficient happens to vanish, a faster rate or an irregular ratio is possible.

The volatility bounds alone do not guarantee that expansion: coefficient smoothness, [stability](../../../../../../stability-of-a-numerical-method.md) and treatment of the nonsmooth terminal payoff matter. The statement applies at fixed positive remaining maturity after appropriate smoothing, not to Greeks at the terminal strike. If the starting diffusion [Courant number](../../../../../../courant-number.md) is already outside the stable range, the proposed coupled refinement preserves that defect and does not establish convergence.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
