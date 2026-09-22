<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Schwartz function](../../../../../schwartz-function.md) is a smooth function for which every [seminorm](../../../../../seminorm.md)

$$
p_{\alpha\beta}(\varphi)=\sup_{x\in\mathbb R^n}|x^\alpha\partial^\beta\varphi(x)|
$$

is finite. These [seminorms](../../../../../seminorm.md) define the Fréchet topology of the [Schwartz space](../../../../../schwartz-space.md) $\mathcal S(\mathbb R^n)$. The [tempered distributions](../../../../../tempered-distribution.md) form its continuous linear dual $\mathcal S'$. We use bilinear [distribution](../../../../../distribution-mathematical-analysis.md) pairing, with no complex conjugation on the [test function](../../../../../test-function.md).

Differentiation under the Fourier integral and [integration by parts](../../../../../integration-by-parts.md) give

$$
\partial_\xi^\beta\widehat\varphi=\mathcal F[(-ix)^\beta\varphi],\qquad\xi^\alpha\widehat f=\mathcal F[D^\alpha f],\quad D=-i\partial.
$$

Therefore each [Schwartz seminorm](../../../../../schwartz-seminorm.md) of $\widehat\varphi$ is bounded by a finite sum of $L^1$ norms of polynomially weighted [derivatives](../../../../../derivative.md) of $\varphi$. Insert the integrable weight $\langle x\rangle^{-n-1}$ to bound those norms by finitely many [Schwartz seminorms](../../../../../schwartz-seminorm.md). This proves that $\mathcal F:\mathcal S\to\mathcal S$ is continuous.

To justify inversion without a merely formal exchange of integrals, insert $e^{-\varepsilon|\xi|^2/2}$ in the inverse integral. The Gaussian Fourier integral gives

$$
(2\pi)^{-n}\int e^{ix\cdot\xi}e^{-\varepsilon|\xi|^2/2}\widehat\varphi(\xi)d\xi=(\varphi*g_\varepsilon)(x),\qquad g_\varepsilon(x)=(2\pi\varepsilon)^{-n/2}e^{-|x|^2/(2\varepsilon)}.
$$

The normalized Gaussian is an approximate identity, so the right side tends to $\varphi(x)$; the left side converges by [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) since $\widehat\varphi$ is integrable. It follows that

$$
\boxed{\varphi(x)=(2\pi)^{-n}\int e^{ix\cdot\xi}\widehat\varphi(\xi)d\xi,\qquad\mathcal F^2\varphi=(2\pi)^n\varphi(-\cdot).}
$$

Reflection is continuous in [Schwartz seminorms](../../../../../schwartz-seminorm.md), so $\mathcal F^{-1}=(2\pi)^{-n}\mathcal R\mathcal F$ is continuous as well. This proves the [Fourier transform isomorphism of the Schwartz space](../../../../../fourier-transform-isomorphism-of-the-schwartz-space.md).

Define the [distributional Fourier transform](../../../../../fourier-transform-of-a-tempered-distribution.md) by

$$
\boxed{\langle\widehat u,\varphi\rangle=\langle u,\widehat\varphi\rangle.}
$$

It agrees with the ordinary integral transform whenever Fubini applies. Transposing the Schwartz inverse gives an inverse on $\mathcal S'$, and the same squared-transform identity holds. For the usual strong dual topology, a [seminorm](../../../../../seminorm.md) is $p_B(u)=\sup_{\varphi\in B}|\langle u,\varphi\rangle|$ for a bounded set $B\subset\mathcal S$. Since a continuous linear Schwartz map takes bounded sets to bounded sets, $p_B(\widehat u)=p_{\mathcal F B}(u)$ proves [continuity](../../../../../continuous-function.md), and similarly for the inverse. [Continuity](../../../../../continuous-function.md) also holds in the weak dual topology. Thus the transform is a continuous isomorphism on [tempered distributions](../../../../../tempered-distribution.md), with the stated normalization.

For a real symmetric [positive-definite matrix](../../../../../positive-definite-matrix.md) $G$, there is $c>0$ with $g(x)=x^TGx\geq c|x|^2$. The reciprocal is locally integrable in dimension three: the radial factor near zero is $r^2r^{-2}dr$. At infinity, rapid decay of a Schwartz [test function](../../../../../test-function.md) makes it integrable. More quantitatively,

$$
\left|\int\frac{\varphi(x)}{g(x)}dx\right|\leq C\sup_x\langle x\rangle^2|\varphi(x)|\int_{\mathbb R^3}\frac{dx}{|x|^2\langle x\rangle^2}<\infty.
$$

This single [seminorm](../../../../../seminorm.md) bound proves a [tempered distribution](../../../../../tempered-distribution.md). No principal-value extension is needed at the origin.

First calculate the isotropic transform. For $f_\varepsilon(x)=e^{-\varepsilon|x|}/|x|^2$ and $k=|\xi|>0$, spherical integration and the supplied sine-integral identity give

$$
\widehat f_\varepsilon(\xi)=\frac{4\pi}{k}\int_0^\infty e^{-\varepsilon r}\frac{\sin(kr)}rdr=\frac{4\pi}{k}\arctan\frac k\varepsilon.
$$

The original functions converge in $\mathcal S'$ to $|x|^{-2}$ by [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) against tests. The transforms are bounded by $2\pi^2/|\xi|$, which is locally integrable in three dimensions and integrable against [Schwartz functions](../../../../../schwartz-function.md) at infinity. Hence

$$
\boxed{\mathcal F(|x|^{-2})(\xi)=\frac{2\pi^2}{|\xi|}\quad\text{as a regular tempered distribution}.}
$$

Let $y=G^{1/2}x$. The Jacobian is $(\det G)^{-1/2}$ and the dual vector is $G^{-1/2}\xi$. The [Fourier transform of a reciprocal positive quadratic form](../../../../../fourier-transform-of-a-reciprocal-positive-quadratic-form.md) is consequently

$$
\boxed{\widehat{(1/g)}(\xi)=\frac{2\pi^2}{\sqrt{\det G}\sqrt{\xi^TG^{-1}\xi}}.}
$$

The frequency-origin value is understood distributionally; there is no additional delta term.

For the complex extension use a symmetric [matrix](../../../../../matrix.md) $A=G+iB$ with real symmetric $B$ and positive real part $G$. Symmetry is natural for a [quadratic form](../../../../../quadratic-form.md); a skew-symmetric part contributes nothing. The bound $|x^TAx|\geq x^TGx$ again gives a regular tempered reciprocal. Both sides of the prospective formula depend holomorphically on the [matrix](../../../../../matrix.md) while its real part is positive: compact parameter sets give a common $|x|^{-2}$ bound for pairing and differentiated integrands. Continue from the real positive [matrices](../../../../../matrix.md) along $A_z=G+izB$. In a complex neighborhood of $z=0$, imaginary $z$ gives real positive [matrices](../../../../../matrix.md), so the one-variable identity theorem supplies the equality; connected continuation along $0\leq z\leq1$ reaches $A$.

The [analytic determinant square root for accretive symmetric matrices](../../../../../analytic-determinant-square-root-for-accretive-symmetric-matrices.md) must follow that continuation, rather than an arbitrary scalar principal root of $\det A$. Explicitly, put $C=G^{-1/2}BG^{-1/2}$ and let its real [eigenvalues](../../../../../eigenvalue.md) be $b_j$. Then

$$
d(A)=\sqrt{\det G}\prod_{j=1}^3\sqrt{1+ib_j},
$$

where each factor has positive real part. This is the [determinant](../../../../../determinant.md) square root normalized positively on real positive [matrices](../../../../../matrix.md). Also

$$
\operatorname{Re}(\xi^TA^{-1}\xi)=\xi^TG^{-1/2}(1+C^2)^{-1}G^{-1/2}\xi>0\qquad(\xi\ne0).
$$

Thus the quadratic-form square root has the unambiguous branch with positive real part. The [accretive complex quadratic reciprocal Fourier transform](../../../../../accretive-complex-quadratic-reciprocal-fourier-transform.md) is

$$
\boxed{\mathcal F\!\left(\frac1{x^TAx}\right)(\xi)=\frac{2\pi^2}{d(A)\sqrt{\xi^TA^{-1}\xi}}.}
$$

Uniform local integrability of the right side justifies its [analytic continuation](../../../../../analytic-continuation.md) as a [tempered distribution](../../../../../tempered-distribution.md), not merely pointwise away from the origin.

For the particular form,

$$
A=\begin{pmatrix}1&i&0\\i&1&0\\0&0&2\end{pmatrix},\qquad\det A=4,\qquad d(A)=2,\qquad A^{-1}=\frac12\begin{pmatrix}1&-i&0\\-i&1&0\\0&0&1\end{pmatrix}.
$$

Substitution gives the required normalized expression

$$
\boxed{\mathcal F\!\left(\frac1{x_1^2+x_2^2+2x_3^2+2ix_1x_2}\right)(\xi)=\frac{\sqrt2\pi^2}{\sqrt{\xi_1^2+\xi_2^2+\xi_3^2-2i\xi_1\xi_2}}.}
$$

For every nonzero real $\xi$, the radicand has positive real part, so the specified square root exists uniquely. Both sides are regular [tempered distributions](../../../../../tempered-distribution.md), despite their locally integrable singularities at zero.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
