<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [period lattice](../../../../../period-lattice.md) $\Lambda$, define the [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) by

$$
\wp(z)=z^{-2}+\sum_{\omega\in\Lambda\setminus\{0\}}\bigl((z-\omega)^{-2}-\omega^{-2}\bigr).
$$

The summands on a compact set away from the lattice are $O(|\omega|^{-3})$, and that lattice sum converges. Thus the series and its termwise derivative converge normally. The function is even, and $\wp'=-2\sum_{\omega\in\Lambda}(z-\omega)^{-3}$ is odd and periodic by reindexing its absolutely convergent series. Hence $\wp(z+\omega_j)-\wp(z)$ is constant; evaluation at $-\omega_j/2$ and evenness make this constant zero for each basis period. The only poles of wp are double lattice poles, with principal part $(z-\omega)^{-2}$.

Let $G_r=\sum_{\omega\ne0}\omega^{-r}$ for the convergent weights used here. Expanding around zero gives

$$
\wp(z)=z^{-2}+3G_4z^2+5G_6z^4+O(z^6),\qquad
\wp'(z)=-2z^{-3}+6G_4z+20G_6z^3+O(z^5).
$$

Therefore

$$
(\wp')^2-4\wp^3=-60G_4z^{-2}-140G_6+O(z^2).
$$

Put $g_2=60G_4$ and $g_3=140G_6$. The elliptic function $(\wp')^2-4\wp^3+g_2\wp+g_3$ has a removable singularity at zero and hence at every lattice point. It is entire and periodic, thus bounded on the plane and constant by the [Liouville theorem](../../../../../liouville-theorem.md). Its zero constant term makes that constant zero. This proves the [Weierstrass elliptic differential equation](../../../../../weierstrass-elliptic-differential-equation.md)

$$
\boxed{\wp'(z)^2=4\wp(z)^3-g_2\wp(z)-g_3.}
$$

The three classes $\omega_i/2$, with $\omega_3=-\omega_1-\omega_2$, are the three distinct nonzero two-torsion classes. Oddness and periodicity give $\wp'(\omega_i/2)=-\wp'(\omega_i/2)$, so they are zeros of the derivative. Their [half-period values of the Weierstrass elliptic function](../../../../../half-period-values-of-the-weierstrass-elliptic-function.md) $e_i$ are therefore roots of $4X^3-g_2X-g_3$.

They are distinct. If $e_i=e_j=e$ with $i\ne j$, the elliptic function $\wp-e$ would have a zero of multiplicity at least two at each of those distinct point classes, since its derivative vanishes there. It has only one pole on the torus, of order two. The [argument principle](../../../../../argument-principle.md) on a fundamental cell equates its total zero and pole orders, contradicting at least four zeros. Thus $e_1,e_2,e_3$ are distinct, and the cubic factors as

$$
\boxed{\wp'(z)^2=4\prod_{i=1}^3(\wp(z)-e_i).}
$$

For the monic cubic $X^3-(g_2/4)X-g_3/4$, the polynomial discriminant is $(g_2^3-27g_3^2)/16=\prod_{i<j}(e_i-e_j)^2$. Hence the [nonvanishing discriminant of a complex lattice](../../../../../nonvanishing-discriminant-of-a-complex-lattice.md) is

$$
\boxed{\Delta(\Lambda)=g_2^3-27g_3^2=16\prod_{i<j}(e_i-e_j)^2\ne0.}
$$

Here $\Delta(\Lambda)$ is the lattice discriminant, not the normalized q-series of Question 1. For $\Lambda=\mathbb Z+\mathbb Z\tau$, the normalizations give $g_2=(4\pi^4/3)E_4$ and $g_3=(8\pi^6/27)E_6$, so $\Delta(\Lambda)=(2\pi)^{12}\Delta(\tau)$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
