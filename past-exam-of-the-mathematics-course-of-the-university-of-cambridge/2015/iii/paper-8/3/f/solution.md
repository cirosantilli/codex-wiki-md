<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use the zero entropy limit supplied in this subpart. By the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) and the [entropy dissipation identity for Ornstein-Uhlenbeck flow](../../../../../../entropy-dissipation-identity-for-ornstein-uhlenbeck-flow.md),

$$
H(f_t\mid\gamma)=\int_t^\infty I(f_s\mid\gamma)\,ds.
$$

Apply the [relative Fisher information](../../../../../../relative-fisher-information.md) decay estimate starting at time $t$:

$$
H(f_t\mid\gamma)\leq I(f_t\mid\gamma)
\int_t^\infty e^{-2(s-t)}\,ds=\frac12I(f_t\mid\gamma).
$$

Thus **the requested entropy-dissipation inequality is**

$$
\boxed{H(f_t\mid\gamma)\leq-\frac12\frac d{dt}H(f_t\mid\gamma).}
$$

It is the [Gaussian logarithmic Sobolev inequality](../../../../../../gaussian-logarithmic-sobolev-inequality.md) along this evolution. Since $H'\leq-2H$, an integrating factor gives **the [entropy convergence rate for Ornstein-Uhlenbeck flow](../../../../../../entropy-convergence-rate-for-ornstein-uhlenbeck-flow.md)**:

$$
\boxed{H(f_t\mid\gamma)\leq e^{-2t}H(f_0\mid\gamma).}
$$

For finite initial entropy, $f_t$ therefore converges to the stationary [Gaussian density](../../../../../../multivariate-normal-density.md) in [relative entropy](../../../../../../kullback-leibler-divergence.md) at rate $2$. If desired, [Pinsker's inequality](../../../../../../pinsker-s-inequality.md) also converts this to the density estimate $\|f_t-\gamma\|_{L^1}\leq\sqrt{2H(f_0\mid\gamma)}e^{-t}$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
