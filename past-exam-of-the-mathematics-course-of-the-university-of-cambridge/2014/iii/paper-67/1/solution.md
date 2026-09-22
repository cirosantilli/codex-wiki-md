<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use complex-linear [distribution](../../../../../distribution-mathematical-analysis.md) pairings, without conjugation. Write $\mathcal D=C_c^\infty(\mathbb R^n)$ for the [space of test functions](../../../../../space-of-test-functions.md). The [smoothing convolution with a test function](../../../../../smoothing-convolution-with-a-test-function.md) is

$$
\boxed{(u*\varphi)(x)=\langle u_y,\varphi(x-y)\rangle.}
$$

On a compact set of $x$ values, all the translated [test functions](../../../../../test-function.md) have support in one compact set. Continuity of the [distribution](../../../../../distribution-mathematical-analysis.md) therefore permits differentiation in $x$, giving $\partial_x^\alpha(u*\varphi)(x)=\langle u,\partial^\alpha\varphi(x-\cdot)\rangle$ for every [multi-index](../../../../../multi-index-notation.md). In particular this [convolution](../../../../../convolution.md) is a [smooth function](../../../../../smooth-function.md), even if $u$ is not tempered.

For the first associativity identity, integration against $\psi$ and the [distribution](../../../../../distribution-mathematical-analysis.md) pairing can be interchanged: the integrand has a common [compact support](../../../../../compact-support.md) in $y$, depends smoothly on the integration variable, and satisfies the finite-order continuity estimate there. Consequently

$$
\begin{aligned}
((u*\varphi)*\psi)(x)
&=\int\psi(z)\langle u_y,\varphi(x-z-y)\rangle\,dz\\
&=\left\langle u_y,\int\varphi((x-y)-z)\psi(z)\,dz\right\rangle\\
&=\boxed{u*(\varphi*\psi)(x).}
\end{aligned}
$$

The common-support argument matters: a general [distribution](../../../../../distribution-mathematical-analysis.md) cannot be paired with arbitrary noncompact functions.

For [convolution of distributions with a compactly supported factor](../../../../../convolution-of-distributions-with-a-compactly-supported-factor.md), first take $v$ with [compact support](../../../../../compact-support.md) $K$ and define

$$
\boxed{\langle w,\chi\rangle
=\left\langle u_x,\left\langle v_y,\chi(x+y)\right\rangle\right\rangle,
\qquad\chi\in\mathcal D.}
$$

The inner pairing is interpreted using a [cutoff function](../../../../../cutoff-function.md) equal to one near $K$. It is smooth in $x$ and has support in $\operatorname{supp}\chi-K$. To see continuity, restrict $\chi$ to a fixed [compact support](../../../../../compact-support.md) $A$. The [order of a distribution](../../../../../order-of-a-distribution.md) estimate for $v$ controls derivatives of the inner function by finitely many derivatives of $\chi$, and its support lies in the fixed compact set $A-K$. Applying the corresponding estimate for $u$ gives

$$
|\langle w,\chi\rangle|\le C_A\max_{|\alpha|\le m_A}\sup|\partial^\alpha\chi|.
$$

Thus $w$ is a [distribution](../../../../../distribution-mathematical-analysis.md), not merely a formal iterated pairing.

Choose an additional [cutoff function](../../../../../cutoff-function.md) in $x$ equal to one on a neighborhood of $A-K$. The resulting joint kernel is compactly supported in both variables, so the [tensor product of distributions](../../../../../tensor-product-of-distributions.md) permits reversing the pairings. One justification is to approximate that smooth compact kernel, in all the required derivative seminorms, by finite sums of products of one-variable kernels; the two orders agree on such products and their continuity estimates pass to the limit. Reversing $x,y$ consequently gives **$u*v=v*u$**. If $u$ rather than $v$ has [compact support](../../../../../compact-support.md), use the same construction with the roles reversed; pairing $u$ against a [smooth function](../../../../../smooth-function.md) is then legitimate.

Evaluating the resulting [smoothing convolution with a test function](../../../../../smoothing-convolution-with-a-test-function.md) gives

$$
(w*\varphi)(x)=\langle u_y,\langle v_z,\varphi(x-y-z)\rangle\rangle
=\boxed{u*(v*\varphi)(x).}
$$

If $v$ has [compact support](../../../../../compact-support.md), $v*\varphi$ is itself a [test function](../../../../../test-function.md); if $u$ has [compact support](../../../../../compact-support.md), its action on the smooth inner [convolution](../../../../../convolution.md) uses a cutoff. This explains the meaning of the formula in either case. It also proves **uniqueness**: $(w*\varphi)(0)=\langle w,\varphi(-\cdot)\rangle$, and reflection runs through all [test functions](../../../../../test-function.md). When both factors have [compact support](../../../../../compact-support.md), the same definition gives $\operatorname{supp}(u*v)\subset\operatorname{supp}u+\operatorname{supp}v$, their [Minkowski sum](../../../../../minkowski-addition.md).

The [Schwartz space](../../../../../schwartz-space.md) consists of [smooth functions](../../../../../smooth-function.md) for which every seminorm $\sup_x|x^\alpha\partial^\beta\phi(x)|$ is finite. A [tempered distribution](../../../../../tempered-distribution.md) is a [continuous linear functional](../../../../../continuous-linear-functional.md) on this space. Fix the angular-frequency [Fourier transform](../../../../../fourier-transform.md) convention

$$
\widehat\phi(\lambda)=\int e^{-i\lambda\cdot x}\phi(x)\,dx,\qquad
\langle\widehat u,\phi\rangle=\langle u,\widehat\phi\rangle,
\qquad \mathcal F^{-1}g(x)=(2\pi)^{-n}\int e^{i\lambda\cdot x}g(\lambda)\,d\lambda.
$$

The [Fourier transform isomorphism of the Schwartz space](../../../../../fourier-transform-isomorphism-of-the-schwartz-space.md) makes the dual definition continuous. For a [compactly supported distribution](../../../../../compactly-supported-distribution.md), a fixed [cutoff function](../../../../../cutoff-function.md) $\chi=1$ near its support extends the action to [smooth functions](../../../../../smooth-function.md) by $\langle u,g\rangle=\langle u,\chi g\rangle$. A finite-order estimate controls this by finitely many [Schwartz space](../../../../../schwartz-space.md) seminorms, so **both compactly supported factors are tempered**.

Their [Fourier transform of a compactly supported distribution](../../../../../fourier-transform-of-a-compactly-supported-distribution.md) is the [smooth function](../../../../../smooth-function.md) $\widehat u(\lambda)=\langle u,e^{-i\lambda\cdot x}\rangle$. Applying the compact-support [convolution](../../../../../convolution.md) definition to the exponential gives

$$
\begin{aligned}
\widehat{u*v}(\lambda)
&=\langle u_x\otimes v_y,e^{-i\lambda\cdot(x+y)}\rangle\\
&=\langle u_x,e^{-i\lambda\cdot x}\rangle
\langle v_y,e^{-i\lambda\cdot y}\rangle
=\boxed{\widehat u(\lambda)\widehat v(\lambda).}
\end{aligned}
$$

The [convolution theorem](../../../../../convolution-theorem.md) has no extra factor with this normalization.

For the [spherical surface measure convolution](../../../../../spherical-surface-measure-convolution.md), put $k=|\lambda|$. Rotate the polar axis to the direction of $\lambda$; rotational invariance of surface area gives

$$
\widehat u_a(\lambda)=2\pi a^2\int_{-1}^1e^{-iak s}\,ds
=\boxed{\frac{4\pi a\sin(ak)}k.}
$$

At $k=0$ the removable value is **$4\pi a^2$**, the total sphere area. Hence $\widehat{u_a*u_b}(\lambda)=16\pi^2ab\sin(ak)\sin(bk)/k^2$.

For $r=|x|>0$, angular integration in [Fourier inversion](../../../../../fourier-inversion-theorem.md) now gives

$$
(u_a*u_b)(x)=\frac{8ab}{r}\int_0^\infty
\frac{\sin(ak)\sin(bk)\sin(rk)}k\,dk.
$$

This conditional integral can be made rigorous by first inserting $e^{-\varepsilon k}$ and then taking $\varepsilon\downarrow0$ in [tempered distributions](../../../../../tempered-distribution.md). The supplied sine identity gives an integral of $\pi/4$ when $|a-b|<r<a+b$, and zero off that interval. Thus

$$
\boxed{u_a*u_b=\frac{2\pi ab}{|x|}\,\mathbf1_{\{|a-b|<|x|<a+b\}}}
$$

as a [regular distribution](../../../../../regular-distribution.md). To justify the limiting density as well as the signs, expand the product of sines into four sine terms and use $\int_0^\infty e^{-\varepsilon k}\sin(sk)\,dk/k=\arctan(s/\varepsilon)$. The four arctangents are uniformly bounded; the regularized inverse is bounded by a constant times $1/r$, which is a [locally integrable function](../../../../../locally-integrable-function.md) in three dimensions. [Dominated convergence theorem](../../../../../dominated-convergence-theorem.md) therefore identifies the distributional limit with the displayed density.

Changing the two endpoint sphere values does not change the [regular distribution](../../../../../regular-distribution.md); this includes the source's closed-interval representative. At a jump, symmetric Fourier inversion instead takes the half-value. If $a=b$, the $1/r$ singularity at the origin remains locally integrable and is not a point mass. As a normalization check,

$$
\int_{\mathbb R^3}\frac{2\pi ab}{|x|}\mathbf1_{\{|a-b|<|x|<a+b\}}\,dx
=4\pi^2ab\big((a+b)^2-(a-b)^2\big)
=16\pi^2a^2b^2,
$$

exactly the product of the original sphere areas.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
