<h1 id="14c/solution">Solution</h1>

↑ **Parent:** [14C](../14c.md)

Near zero, expand $e^z-1=z(1+z/2+z^2/6+\cdots)$ and invert the parenthesized series. The first three nonzero [Laurent series](../../../../../laurent-series.md) terms are

$$
\boxed{f(z)=\frac1z-\frac12+\frac z{12}+O(z^3),\qquad0<|z|<2\pi.}
$$

The zero quadratic coefficient also follows from $f(-z)=-1-f(z)$, which makes $f(z)+1/2$ odd. The nearest other singularities are at $\pm2\pi i$.

All poles of $f$ occur at $2\pi i r$, $r\in\mathbb Z$, and have residue one, since the derivative of $e^z-1$ equals one at those zeros. Also

$$
\frac{2z}{z^2+4\pi^2r^2}=\frac1{z-2\pi ir}+\frac1{z+2\pi ir}.
$$

Thus $f_1$ subtracts the complete principal part at zero and at every pole with $1\le|r|\le n$. These are all the poles in the stated open disk; each singularity of $f_2=f-f_1$ there is removable.

For $|z|>2n\pi$, expanding each rational summand in inverse powers gives

$$
f_1(z)=\frac{2n+1}{z}+\sum_{r=1}^n\sum_{k=1}^\infty2(-4\pi^2r^2)^kz^{-2k-1}.
$$

This contributes no constant or positive-power term. To find the first Taylor coefficients of the analytic $f_2$, expand $f_1$ near zero as $z^{-1}+z\sum_{r=1}^n(2\pi^2r^2)^{-1}+O(z^3)$ and subtract it from the already calculated local series of $f$. Combining its Taylor series with the exterior series above yields **the three requested annular coefficients**:

$$
\boxed{a_{-1}=2n+1,\quad a_0=-\frac12,\quad
 a_1=\frac1{12}-\frac1{2\pi^2}\sum_{r=1}^n\frac1{r^2}.}
$$

Both series converge on $2n\pi<|z|<2(n+1)\pi$, so this combination is a valid Laurent expansion there.

For the [Basel sum from exponential poles](../../../../../basel-sum-from-exponential-poles.md), let $R_n=(2n+1)\pi$. The Laurent coefficient formula gives

$$
a_1=\frac1{2\pi i}\int_{|z|=R_n}\frac{f(z)}{z^2}\,dz.
$$

The function $f$ is bounded on these circles by one constant independent of $n$. Indeed, if $\operatorname{Re}z\ge1$, use $|e^z-1|\ge e-1$; if $\operatorname{Re}z\le-1$, use $|e^z-1|\ge1-e^{-1}$. In the remaining strip $|\operatorname{Re}z|\le1$, the imaginary part has magnitude $\sqrt{R_n^2-(\operatorname{Re}z)^2}$, within $1/R_n$ of the odd multiple $R_n$ of $\pi$. Its cosine is negative, so $|e^z-1|^2=e^{2\operatorname{Re}z}+1-2e^{\operatorname{Re}z}\cos(\operatorname{Im}z)\ge1$.

The contour length is $2\pi R_n$, hence $|a_1|\le C/R_n\to0$. Taking the limit in the coefficient formula proves

$$
\boxed{\sum_{r=1}^{\infty}\frac1{r^2}=\frac{\pi^2}{6}.}
$$

## ↑ Ancestors (10)

1. [14C](../14c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
