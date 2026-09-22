<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The function $U(x)=1/|x|$ is [locally integrable](../../../../../../locally-integrable-function.md) in $\mathbb R^3$, so it defines a [distribution](../../../../../../distribution-mathematical-analysis.md). The claimed [distributional identity](../../../../../../distributional-identity.md) means that for every $\varphi\in C_c^\infty(\mathbb R^3)$,

$$
-\int_{\mathbb R^3}\frac1{|x|}\Delta\varphi(x)\,dx=4\pi\varphi(0).
$$

Choose a ball containing the support and remove $B_\varepsilon(0)$. On the punctured region $\Delta U=0$. [Green's second identity](../../../../../../green-second-identity.md) gives

$$
\int_{|x|>\varepsilon}U\Delta\varphi\,dx
=\int_{|x|=\varepsilon}
\left(-\frac1\varepsilon\partial_r\varphi-\frac1{\varepsilon^2}\varphi\right)\,dS.
$$

The outer boundary contributes zero. On the inner boundary, the outward normal for the punctured region is $-\widehat r$, so $\partial_nU=+1/\varepsilon^2$, fixing the sign.

The first term is $O(\varepsilon)$; the second equals $-\int_{S^2}\varphi(\varepsilon\omega)\,d\omega\to-4\pi\varphi(0)$. Local integrability allows the left side to converge to its full-space integral. Therefore $\boxed{-\Delta(1/|x|)=4\pi\delta_0}$. In this sign convention, $1/(4\pi|x|)$ is the [fundamental solution of the Laplace equation](../../../../../../fundamental-solution-of-the-laplace-equation.md) for the operator $-\Delta$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
