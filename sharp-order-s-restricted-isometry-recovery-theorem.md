# Sharp order-s restricted-isometry recovery theorem

↑ **Parent:** [Restricted isometry constant](restricted-isometry-constant.md)

For $s\ge2$ and $\delta=\delta_s(A)<1/3$, noisy [basis pursuit](basis-pursuit.md) has error $\|\hat x-x_0\|_2\le C_1\eta+C_2\sigma_s(x_0)/\sqrt s$, with constants depending only on $\delta$. One admissible pair is

$$
C_1=\frac{2\sqrt{2(1+\delta)}}{1-3\delta},\qquad
C_2=\frac{2\sqrt2(2\delta+\sqrt{(1-3\delta)\delta})+2(1-3\delta)}{1-3\delta}.
$$

These constants follow from Theorem 3.3 of [the sharp restricted-isometry recovery analysis](https://arxiv.org/pdf/1302.1236), with the actual noise bounded by the tolerance $\eta$. The restriction $s\ge2$ is necessary: equal unit columns give $\delta_1=0$ without unique recovery. The coefficient of the approximation term cannot universally be one.

## ↑ Ancestors (9)

1. [Restricted isometry constant](restricted-isometry-constant.md)
2. [Restricted isometry property](restricted-isometry-property.md)
3. [Compressed sensing](compressed-sensing.md)
4. [Sparse optimization](sparse-optimization.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
