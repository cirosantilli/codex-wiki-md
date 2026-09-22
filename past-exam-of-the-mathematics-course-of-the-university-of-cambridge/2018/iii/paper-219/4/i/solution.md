<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $v=\sigma_{\rm int}^2$, $r_s=\sigma_{O,s}^2$ and $o_s=\widehat O_s$. A flat density in $\log\tau$ means $p(\tau)\propto1/\tau$ with respect to $d\tau$; likewise $p(v)\propto1/v$. The [Jacobian determinant](../../../../../../jacobian-determinant.md) must therefore appear when using the original scale variables. The joint [hierarchical Bayesian model](../../../../../../hierarchical-bayesian-model.md) kernel, with respect to $d\mu_C\,dv\,d\tau\prod_sdo_s\,dC_s\,dE_s$, is

$$
\boxed{p(o,C,E,\mu_C,v,\tau)\propto\frac1{v\tau}\prod_{s=1}^{N}\left[(2\pi r_s)^{-1/2}e^{-(o_s-C_s-E_s)^2/(2r_s)}(2\pi v)^{-1/2}e^{-(C_s-\mu_C)^2/(2v)}\tau^{-1}e^{-E_s/\tau}\mathbf1_{\{E_s\ge0\}}\right]}.
$$

This is a kernel, not a normalized joint probability distribution, because the stated priors are improper. Conditioning on $o$ would still require [posterior propriety](../../../../../../posterior-propriety.md). In fact that check fails here, as shown in part (iii)(c); proper formal full conditionals alone do not repair it. The [Gaussian–exponential hierarchical colour model](../../../../../../gaussian-exponential-hierarchical-colour-model.md) distinguishes the intrinsic normal colour, positive [interstellar dust](../../../../../../interstellar-dust.md) reddening, and measurement noise.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
