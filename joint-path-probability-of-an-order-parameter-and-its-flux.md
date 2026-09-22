# Joint path probability of an order parameter and its flux

↑ **Parent:** [Mixed conserved and nonconserved order-parameter dynamics](mixed-conserved-and-nonconserved-order-parameter-dynamics.md)

Put $u_j=\dot p_j+\partial_iW_{ij}$. The additive independent noises give the forward action

$$
S_F=\int\left[\frac{|u+\Gamma\mu|^2}{2\sigma^2}
+\frac{|W+M\nabla\mu|^2}{2\sigma_N^2}\right]d\mathbf r\,dt.
$$

For a time-even [order parameter](order-parameter.md) and time-odd flux, the backward action replaces $u,W$ by $-u,-W$ while keeping $\mu$ fixed on the corresponding configurations. Common normalization and [time-reversal invariance of a path Jacobian](time-reversal-invariance-of-a-path-jacobian.md) then give

$$
\log\frac{P_F}{P_B}
=-\frac{2\Gamma}{\sigma^2}\int\mu_j(\dot p_j+\partial_iW_{ij})
-\frac{2M}{\sigma_N^2}\int W_{ij}\partial_i\mu_j.
$$

At the two thermal noise strengths, periodic [boundary conditions](boundary-condition.md) cancel the two spatial terms by [integration by parts](integration-by-parts.md), leaving $-(F_2-F_1)/(k_BT)$. Thus the joint dynamics satisfies [microscopic reversibility](microscopic-reversibility.md).

## ↑ Ancestors (7)

1. [Mixed conserved and nonconserved order-parameter dynamics](mixed-conserved-and-nonconserved-order-parameter-dynamics.md)
2. [Order parameter](order-parameter.md)
3. [Critical phenomenon](critical-phenomenon-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/2/d/solution.md)
- [Time-reversal invariance of a path Jacobian](time-reversal-invariance-of-a-path-jacobian.md)
