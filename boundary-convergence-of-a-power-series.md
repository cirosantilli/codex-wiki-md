# Boundary convergence of a power series

↑ **Parent:** [Radius of convergence](radius-of-convergence.md)

Knowing the [radius of convergence](radius-of-convergence.md) does not settle convergence on its boundary. The three [power series](power-series.md)

$$
\sum_{n=0}^{\infty}z^n,\qquad
\sum_{n=1}^{\infty}\frac{z^n}{n},\qquad
\sum_{n=1}^{\infty}\frac{z^n}{n^2}
$$

all have radius one, but behave differently on $|z|=1$.

<a id="image-the-same-radius-of-convergence-permits-three-different-behaviours-on-the-unit-circle"></a>
![](power-series-boundary-behavior.png)

**[Figure 15](#image-the-same-radius-of-convergence-permits-three-different-behaviours-on-the-unit-circle). The same radius of convergence permits three different behaviours on the unit circle**. Green denotes [absolute convergence](absolute-convergence.md), orange [conditional convergence](conditional-convergence.md), and red divergence. All three series converge absolutely in the open [unit disk](unit-disk.md). On its boundary, the geometric series diverges everywhere; the $1/n$ series converges conditionally except at $z=1$; the $1/n^2$ series converges absolutely everywhere.

For the [geometric series](geometric-series.md), boundary terms all have [complex modulus](complex-modulus.md) one, violating the [term test for divergence](term-test-for-divergence.md). For the second series, absolute values give the divergent [harmonic series](harmonic-series.md) at every boundary point. At $z=1$ the series itself is harmonic and diverges. At any other point on the [unit circle](complex-unit-circle.md), its geometric [partial sums](partial-sum.md) obey

$$
\left|\sum_{k=1}^{N}z^k\right|
=\left|\frac{z(1-z^N)}{1-z}\right|
\le\frac2{|1-z|}.
$$

The [Dirichlet test](dirichlet-test.md) with the decreasing [sequence](sequence.md) $1/n\to0$ therefore gives [conditional convergence](conditional-convergence.md). In particular, $z=-1$ gives the negative of the [alternating harmonic series](alternating-harmonic-series.md), with sum $-\ln2$. For the third series, the convergent [p-series](p-series.md) $\sum_{n\ge1}1/n^2$ bounds the absolute values at every boundary point, giving [absolute convergence](absolute-convergence.md) by the [comparison test for series](comparison-test-for-series.md).

At $z=-1$, the [rational function](rational-function.md) $1/(1-z)$ is well defined and equals $1/2$, yet its [geometric series](geometric-series.md) diverges there. A formula for a [function](function-split.md) and a particular series representation can have different domains. Likewise, applying [termwise differentiation of a power series](termwise-differentiation-of-a-power-series.md) preserves the radius but need not preserve the boundary convergence.

## ↑ Ancestors (8)

1. [Radius of convergence](radius-of-convergence.md)
2. [Power series](power-series.md)
3. [Sequence and series](sequence-and-series-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Radius of convergence](radius-of-convergence.md)
