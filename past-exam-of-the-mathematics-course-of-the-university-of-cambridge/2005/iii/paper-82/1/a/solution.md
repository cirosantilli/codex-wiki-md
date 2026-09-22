<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $Z=\rho\beta=\sqrt{\rho\mu}>0$, the [seismic impedance](../../../../../../seismic-impedance.md). In a uniform medium, define $w_+=v-\sigma/Z$ and $w_-=v+\sigma/Z$. The field equations give

$$
(\partial_t+\beta\partial_x)w_+=0,\qquad(\partial_t-\beta\partial_x)w_-=0.
$$

Thus $w_+=2F(x-\beta t)$ and $w_-=2G(x+\beta t)$, with arbitrary independent profiles $F,G$. Reconstruction gives

$$
\boxed{v=F+G,\qquad\sigma=-ZF+ZG.}
$$

The two characteristic components therefore have $v_+=F$, $\sigma_+=-Zv_+$ and $v_-=G$, $\sigma_-=Zv_-$.

The kinetic plus [elastic energy](../../../../../../elastic-energy.md) [mass density](../../../../../../density.md) is $e=\rho v^2/2+\sigma^2/(2\mu)$. Multiplying the equations by $v$ and $\sigma/\mu$ yields $e_t=(v\sigma)_x$. Hence the [elastic-wave energy flux](../../../../../../elastic-wave-energy-flux.md) is $S=-v\sigma$. For a pure forward wave $S_+=Zv_+^2\geq0$; for a pure backward wave $S_-=-Zv_-^2\leq0$. In the mixture the cross terms cancel, giving **$S=Z(v_+^2-v_-^2)$**. Strict sign holds for nonzero components.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
