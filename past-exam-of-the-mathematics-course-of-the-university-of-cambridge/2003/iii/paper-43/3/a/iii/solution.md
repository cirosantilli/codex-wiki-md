<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A valid symmetric [proposal distribution](../../../../../../../proposal-distribution.md) is $v_i'=v_i+\eta$ with $\eta\sim N(0,s_{vi}^2)$ on the entire real line. Reject immediately if $v_i'\le0$. Otherwise use the [positive-parameter random walk with boundary rejection](../../../../../../../positive-parameter-random-walk-with-boundary-rejection.md). With

$$
D_j'=D_j+\omega_i\{\varphi(x_j;\mu_i,v_i')-\varphi(x_j;\mu_i,v_i)\},
$$

the [Metropolis–Hastings acceptance probability](../../../../../../../metropolis-hastings-acceptance-probability.md) is

$$
\boxed{a_i=\min\left\{1,\ \prod_{j=1}^n\frac{D_j'}{D_j}\left(\frac{v_i'}{v_i}\right)^{-\alpha-1}\exp\left[-\beta\left(\frac1{v_i'}-\frac1{v_i}\right)\right]\right\}.}
$$

No [Jacobian determinant](../../../../../../../jacobian-determinant.md) is needed for this additive proposal in $v_i$. Do not repeatedly redraw until $v_i'>0$: that would create a state-dependent truncated proposal and require an additional Hastings correction. Alternatively a symmetric walk in $u_i=\log v_i$ respects positivity, but then the transformed target has a factor $v_i$; equivalently the acceptance ratio in variance coordinates has the extra factor $v_i'/v_i$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
