<h1 id="26k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The integrands are absolutely integrable because $f$ has compact support, $g\in L^1(\mathbb R)$, and $|\varphi_Z|\leq1$. [Fubini's theorem](../../../../../../fubini-s-theorem.md) therefore permits us to insert $\varphi_Z(s)=\mathbb E[e^{isZ}]$ and interchange the expectation and integrals:

$$
\begin{aligned}
&\iint g(\varepsilon s)f(x)e^{-isx}\varphi_Z(s)\,ds\,dx\\
&=\mathbb E\left[
\iint g(\varepsilon s)f(x)e^{is(Z-x)}\,ds\,dx
\right].
\end{aligned}
$$

With $r=\varepsilon s$, the inner integral in $s$ is

$$
\int g(\varepsilon s)e^{is(Z-x)}\,ds
=\frac1\varepsilon
\widehat g\left(\frac{Z-x}{\varepsilon}\right).
$$

Now set $t=(Z-x)/\varepsilon$. The change of variables $x=Z-\varepsilon t$ gives

$$
\iint g(\varepsilon s)f(x)e^{-isx}\varphi_Z(s)\,ds\,dx
=\int\widehat g(t)\mathbb E[f(Z-\varepsilon t)]\,dt,
$$

which is the required identity.

Choose any $g$ with $g,\widehat g\in L^1$, $g(0)\ne0$, and for which [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md) applies, for example a [Gaussian function](../../../../../../gaussian-function.md). The left side factors through the [Fourier transform](../../../../../../fourier-transform.md) of $f$ as

$$
\int g(\varepsilon s)\widehat f(-s)\varphi_Z(s)\,ds.
$$

On the right side, $f(Z-\varepsilon t)\to f(Z)$ and

$$
|\widehat g(t)\mathbb E[f(Z-\varepsilon t)]|
\leq\lVert f\rVert_\infty|\widehat g(t)|.
$$

The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) and Fourier inversion at zero give

$$
\int\widehat g(t)\mathbb E[f(Z-\varepsilon t)]\,dt
\longrightarrow
2\pi g(0)\mathbb E[f(Z)].
$$

Consequently the [Fourier-cutoff recovery of expectations from a characteristic function](../../../../../../fourier-cutoff-recovery-of-expectations-from-a-characteristic-function.md) is

$$
\boxed{
\mathbb E[f(Z)]
=\lim_{\varepsilon\downarrow0}
\frac{1}{2\pi g(0)}
\int g(\varepsilon s)\widehat f(-s)\varphi_Z(s)\,ds.}
$$

The right side depends only on $\varphi_Z$. Equal [characteristic functions](../../../../../../characteristic-function.md) therefore give equal expectations for every compactly supported continuous $f$, and part a yields the [uniqueness theorem for characteristic functions](../../../../../../uniqueness-theorem-for-characteristic-functions.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26K](../../26k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
