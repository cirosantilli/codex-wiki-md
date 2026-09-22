<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\tau=x+iy$. The modular transformation law and

$$
\operatorname{Im}(\gamma\tau)=\frac{y}{|c\tau+d|^2}
$$

show that the [invariant norm of a modular form](../../../../../../invariant-norm-of-a-modular-form.md)

$$
y^{k/2}|f(\tau)|
$$

is invariant under $\Gamma(1)$. On the region from part (a), it is bounded: it is continuous on every truncated region, while the [cusp form](../../../../../../cusp-form.md) condition makes it tend to zero as $y\to\infty$. Thus

$$
|f(x+iy)|\leq C_0y^{-k/2}
$$

for all $x\in\mathbb R$ and $y>0$.

The [Fourier coefficient](../../../../../../fourier-coefficient.md) formula on one period gives

$$
a_n=e^{2\pi ny}\int_0^1f(x+iy)e^{-2\pi inx}\,dx,
$$

and hence

$$
|a_n|\leq C_0e^{2\pi ny}y^{-k/2}.
$$

Choosing $y=1/n$ yields

$$
|a_n|\leq C_0e^{2\pi}n^{k/2}.
$$

This proves the [Fourier coefficient bound for a cusp form](../../../../../../fourier-coefficient-bound-for-a-cusp-form.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
