# Paper 67

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_67.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_67.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use complex-linear [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) pairings, without conjugation. Write $\mathcal D=C_c^\infty(\mathbb R^n)$ for the [space of test functions](../../../distribution-theory.md#space-of-test-functions). The [smoothing convolution with a test function](../../../fourier-analysis.md#smoothing-convolution-with-a-test-function) is

$$
\boxed{(u*\varphi)(x)=\langle u_y,\varphi(x-y)\rangle.}
$$

On a compact set of $x$ values, all the translated [test functions](../../../distribution-theory.md#test-function) have support in one compact set. Continuity of the [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) therefore permits differentiation in $x$, giving $\partial_x^\alpha(u*\varphi)(x)=\langle u,\partial^\alpha\varphi(x-\cdot)\rangle$ for every [multi-index](../../../distribution-theory.md#multi-index-notation). In particular this [convolution](../../../fourier-analysis.md#convolution) is a [smooth function](../../../analysis.md#smooth-function), even if $u$ is not tempered.

For the first associativity identity, integration against $\psi$ and the [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) pairing can be interchanged: the integrand has a common [compact support](../../../function.md#compact-support) in $y$, depends smoothly on the integration variable, and satisfies the finite-order continuity estimate there. Consequently

$$
\begin{aligned}
((u*\varphi)*\psi)(x)
&=\int\psi(z)\langle u_y,\varphi(x-z-y)\rangle\,dz\\
&=\left\langle u_y,\int\varphi((x-y)-z)\psi(z)\,dz\right\rangle\\
&=\boxed{u*(\varphi*\psi)(x).}
\end{aligned}
$$

The common-support argument matters: a general [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) cannot be paired with arbitrary noncompact functions.

For [convolution of distributions with a compactly supported factor](../../../fourier-analysis.md#convolution-of-distributions-with-a-compactly-supported-factor), first take $v$ with [compact support](../../../function.md#compact-support) $K$ and define

$$
\boxed{\langle w,\chi\rangle
=\left\langle u_x,\left\langle v_y,\chi(x+y)\right\rangle\right\rangle,
\qquad\chi\in\mathcal D.}
$$

The inner pairing is interpreted using a [cutoff function](../../../distribution-theory.md#cutoff-function) equal to one near $K$. It is smooth in $x$ and has support in $\operatorname{supp}\chi-K$. To see continuity, restrict $\chi$ to a fixed [compact support](../../../function.md#compact-support) $A$. The [order of a distribution](../../../distribution-theory.md#order-of-a-distribution) estimate for $v$ controls derivatives of the inner function by finitely many derivatives of $\chi$, and its support lies in the fixed compact set $A-K$. Applying the corresponding estimate for $u$ gives

$$
|\langle w,\chi\rangle|\le C_A\max_{|\alpha|\le m_A}\sup|\partial^\alpha\chi|.
$$

Thus $w$ is a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis), not merely a formal iterated pairing.

Choose an additional [cutoff function](../../../distribution-theory.md#cutoff-function) in $x$ equal to one on a neighborhood of $A-K$. The resulting joint kernel is compactly supported in both variables, so the [tensor product of distributions](../../../distribution-theory.md#tensor-product-of-distributions) permits reversing the pairings. One justification is to approximate that smooth compact kernel, in all the required derivative seminorms, by finite sums of products of one-variable kernels; the two orders agree on such products and their continuity estimates pass to the limit. Reversing $x,y$ consequently gives **$u*v=v*u$**. If $u$ rather than $v$ has [compact support](../../../function.md#compact-support), use the same construction with the roles reversed; pairing $u$ against a [smooth function](../../../analysis.md#smooth-function) is then legitimate.

Evaluating the resulting [smoothing convolution with a test function](../../../fourier-analysis.md#smoothing-convolution-with-a-test-function) gives

$$
(w*\varphi)(x)=\langle u_y,\langle v_z,\varphi(x-y-z)\rangle\rangle
=\boxed{u*(v*\varphi)(x).}
$$

If $v$ has [compact support](../../../function.md#compact-support), $v*\varphi$ is itself a [test function](../../../distribution-theory.md#test-function); if $u$ has [compact support](../../../function.md#compact-support), its action on the smooth inner [convolution](../../../fourier-analysis.md#convolution) uses a cutoff. This explains the meaning of the formula in either case. It also proves **uniqueness**: $(w*\varphi)(0)=\langle w,\varphi(-\cdot)\rangle$, and reflection runs through all [test functions](../../../distribution-theory.md#test-function). When both factors have [compact support](../../../function.md#compact-support), the same definition gives $\operatorname{supp}(u*v)\subset\operatorname{supp}u+\operatorname{supp}v$, their [Minkowski sum](../../../geometry-and-topology.md#minkowski-addition).

The [Schwartz space](../../../fourier-analysis.md#schwartz-space) consists of [smooth functions](../../../analysis.md#smooth-function) for which every seminorm $\sup_x|x^\alpha\partial^\beta\phi(x)|$ is finite. A [tempered distribution](../../../fourier-analysis.md#tempered-distribution) is a [continuous linear functional](../../../topological-vector-space.md#continuous-linear-functional) on this space. Fix the angular-frequency [Fourier transform](../../../analysis.md#fourier-transform) convention

$$
\widehat\phi(\lambda)=\int e^{-i\lambda\cdot x}\phi(x)\,dx,\qquad
\langle\widehat u,\phi\rangle=\langle u,\widehat\phi\rangle,
\qquad \mathcal F^{-1}g(x)=(2\pi)^{-n}\int e^{i\lambda\cdot x}g(\lambda)\,d\lambda.
$$

The [Fourier transform isomorphism of the Schwartz space](../../../analysis.md#fourier-transform-isomorphism-of-the-schwartz-space) makes the dual definition continuous. For a [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution), a fixed [cutoff function](../../../distribution-theory.md#cutoff-function) $\chi=1$ near its support extends the action to [smooth functions](../../../analysis.md#smooth-function) by $\langle u,g\rangle=\langle u,\chi g\rangle$. A finite-order estimate controls this by finitely many [Schwartz space](../../../fourier-analysis.md#schwartz-space) seminorms, so **both compactly supported factors are tempered**.

Their [Fourier transform of a compactly supported distribution](../../../distribution-theory.md#fourier-transform-of-a-compactly-supported-distribution) is the [smooth function](../../../analysis.md#smooth-function) $\widehat u(\lambda)=\langle u,e^{-i\lambda\cdot x}\rangle$. Applying the compact-support [convolution](../../../fourier-analysis.md#convolution) definition to the exponential gives

$$
\begin{aligned}
\widehat{u*v}(\lambda)
&=\langle u_x\otimes v_y,e^{-i\lambda\cdot(x+y)}\rangle\\
&=\langle u_x,e^{-i\lambda\cdot x}\rangle
\langle v_y,e^{-i\lambda\cdot y}\rangle
=\boxed{\widehat u(\lambda)\widehat v(\lambda).}
\end{aligned}
$$

The [convolution theorem](../../../fourier-analysis.md#convolution-theorem) has no extra factor with this normalization.

For the [spherical surface measure convolution](../../../distribution-theory.md#spherical-surface-measure-convolution), put $k=|\lambda|$. Rotate the polar axis to the direction of $\lambda$; rotational invariance of surface area gives

$$
\widehat u_a(\lambda)=2\pi a^2\int_{-1}^1e^{-iak s}\,ds
=\boxed{\frac{4\pi a\sin(ak)}k.}
$$

At $k=0$ the removable value is **$4\pi a^2$**, the total sphere area. Hence $\widehat{u_a*u_b}(\lambda)=16\pi^2ab\sin(ak)\sin(bk)/k^2$.

For $r=|x|>0$, angular integration in [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) now gives

$$
(u_a*u_b)(x)=\frac{8ab}{r}\int_0^\infty
\frac{\sin(ak)\sin(bk)\sin(rk)}k\,dk.
$$

This conditional integral can be made rigorous by first inserting $e^{-\varepsilon k}$ and then taking $\varepsilon\downarrow0$ in [tempered distributions](../../../fourier-analysis.md#tempered-distribution). The supplied sine identity gives an integral of $\pi/4$ when $|a-b|<r<a+b$, and zero off that interval. Thus

$$
\boxed{u_a*u_b=\frac{2\pi ab}{|x|}\,\mathbf1_{\{|a-b|<|x|<a+b\}}}
$$

as a [regular distribution](../../../distribution-theory.md#regular-distribution). To justify the limiting density as well as the signs, expand the product of sines into four sine terms and use $\int_0^\infty e^{-\varepsilon k}\sin(sk)\,dk/k=\arctan(s/\varepsilon)$. The four arctangents are uniformly bounded; the regularized inverse is bounded by a constant times $1/r$, which is a [locally integrable function](../../../distribution-theory.md#locally-integrable-function) in three dimensions. [Dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) therefore identifies the distributional limit with the displayed density.

Changing the two endpoint sphere values does not change the [regular distribution](../../../distribution-theory.md#regular-distribution); this includes the source's closed-interval representative. At a jump, symmetric Fourier inversion instead takes the half-value. If $a=b$, the $1/r$ singularity at the origin remains locally integrable and is not a point mass. As a normalization check,

$$
\int_{\mathbb R^3}\frac{2\pi ab}{|x|}\mathbf1_{\{|a-b|<|x|<a+b\}}\,dx
=4\pi^2ab\big((a+b)^2-(a-b)^2\big)
=16\pi^2a^2b^2,
$$

exactly the product of the original sphere areas.

## 2

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For $u\in\mathcal E'$, choose a [cutoff function](../../../distribution-theory.md#cutoff-function) $\chi=1$ on a neighborhood of its support. Its extension to [smooth functions](../../../analysis.md#smooth-function) makes

$$
F(z)=\langle u_x,\chi(x)e^{-iz\cdot x}\rangle
$$

independent of the choice of cutoff. For real frequency, the definition of the [distributional Fourier transform](../../../fourier-analysis.md#fourier-transform-of-a-tempered-distribution) gives $F(\lambda)=\widehat u(\lambda)$: interchange the pairing with the integral of a [Schwartz function](../../../fourier-analysis.md#schwartz-function), using the finite-order estimate on the cutoff's [compact support](../../../function.md#compact-support). On each compact set of complex frequencies the exponential and all its $x$ derivatives have uniformly convergent power series. Continuity of the [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) allows termwise differentiation, with

$$
\partial_z^\alpha F(z)=\langle u_x,(-ix)^\alpha e^{-iz\cdot x}\rangle.
$$

Consequently **$F$ is entire on $\mathbb C^n$**.

For the precise exponential type, a fixed enlarged support would give an unnecessarily enlarged radius. Instead use the [shrinking-cutoff exponential-type estimate](../../../distribution-theory.md#shrinking-cutoff-exponential-type-estimate). On one fixed compact neighborhood of the closed radius-$\delta$ ball, $u$ has finite [order of a distribution](../../../distribution-theory.md#order-of-a-distribution) $m$. Choose $\chi_\varepsilon=1$ near that ball, supported in the radius-$(\delta+\varepsilon)$ ball, with $|\partial^\alpha\chi_\varepsilon|\le C_\alpha\varepsilon^{-|\alpha|}$ for $0<\varepsilon\le1/2$. The finite-order estimate gives

$$
|F(z)|\le C\varepsilon^{-m}(1+|z|)^m
 e^{(\delta+\varepsilon)|\operatorname{Im}z|}.
$$

Take $\varepsilon=[2(1+|z|)]^{-1}$. Its extra exponential is bounded by $e^{1/2}$, while the derivative cost is [polynomial](../../../polynomial.md). Thus

$$
\boxed{|\widehat u(z)|\le C'(1+|z|)^{2m}e^{\delta|\operatorname{Im}z|}.}
$$

The entire function was defined with a fixed cutoff; only its bound uses a frequency-dependent cutoff, so no holomorphic dependence is lost. This proves the required estimate with some $N\ge0$ without enlarging $\delta$.

For the converse, set $V(z)=e^{iz\cdot y}U(z)$. Its restriction to real frequencies has [polynomial growth](../../../analysis.md#polynomial-growth). Define the inverse [tempered distribution](../../../fourier-analysis.md#tempered-distribution) $v$ by

$$
\langle v,\phi\rangle=(2\pi)^{-n}\int_{\mathbb R^n}V(\xi)\widehat\phi(-\xi)\,d\xi,
\qquad\phi\in\mathcal S.
$$

Rapid decay of the [Schwartz function](../../../fourier-analysis.md#schwartz-function) transform proves convergence and continuity, and [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) gives $\widehat v=V$ on real frequencies.

We prove its support directly by [contour shifting](../../../complex-analysis.md#contour-shifting), rather than assuming the support conclusion of the [Paley–Wiener–Schwartz theorem](../../../distribution-theory.md#paley-wiener-schwartz-theorem). Let $\omega$ be a real unit vector and take a [test function](../../../distribution-theory.md#test-function) $\phi$ supported in $x\cdot\omega\ge\delta+\epsilon$ for some $\epsilon>0$. For every integer $M\ge0$, [integration by parts](../../../calculus.md#integration-by-parts) in the real-frequency Fourier integral gives

$$
\begin{aligned}
\widehat\phi(-\xi-it\omega)
&=\int e^{i\xi\cdot x}e^{-t\omega\cdot x}\phi(x)\,dx,\\
|\widehat\phi(-\xi-it\omega)|
&\le C_M(1+t)^{2M}(1+|\xi|^2)^{-M}
 e^{-t(\delta+\epsilon)},\qquad t\ge0.
\end{aligned}
$$

Indeed, move $(1-\Delta_x)^M$ from the oscillatory exponential to $e^{-t\omega\cdot x}\phi$; its derivatives supply at most $2M$ powers of $t$.

The product $V(z)\widehat\phi(-z)$ is entire. Rotate coordinates so that $\omega$ is the first coordinate vector and apply [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) to a rectangle in that one complex coordinate, integrating the remaining real coordinates afterwards. For fixed $t$, choose $2M>N+n+2$; the displayed decay estimate, uniformly on the intervening imaginary segment, makes the vertical faces vanish as the real rectangle width tends to infinity. The horizontal integrals are absolutely convergent. Hence

$$
\langle v,\phi\rangle=(2\pi)^{-n}\int_{\mathbb R^n}
 V(\xi+it\omega)\widehat\phi(-\xi-it\omega)\,d\xi.
$$

Using $(1+|\xi+it\omega|)^N\le C(1+t)^N(1+|\xi|)^N$ and the growth hypothesis bounds this pairing by

$$
C'(1+t)^{N+2M}e^{-\epsilon t}
\int_{\mathbb R^n}(1+|\xi|)^N(1+|\xi|^2)^{-M}\,d\xi.
$$

It tends to zero as $t\to\infty$, so the pairing vanishes. Every point outside the closed radius-$\delta$ ball lies in such a separating half-space; a finite [partition of unity](../../../differential-geometry.md#partition-of-unity) for the support of a [test function](../../../distribution-theory.md#test-function) outside the ball proves $\operatorname{supp}v\subset\overline B(0,\delta)$.

Translate this [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution) by $y$: define $\langle u,\phi\rangle=\langle v,\phi(\cdot+y)\rangle$. The [Translation property of the Fourier transform](../../../fourier-analysis.md#translation-property-of-the-fourier-transform) gives

$$
\widehat u(\xi)=e^{-i\xi\cdot y}V(\xi)=U(\xi),
\qquad\boxed{\operatorname{supp}u\subset\overline B(y,\delta).}
$$

The compact-support entire extension agrees with $U$ everywhere by the [identity theorem](../../../complex-analysis.md#identity-theorem), applied successively in the complex coordinates. [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) also gives uniqueness. This completes both directions of the ball version of the [Paley–Wiener–Schwartz theorem](../../../distribution-theory.md#paley-wiener-schwartz-theorem).

For the [wave equation](../../../wave-equation.md), take a real constant $c\ne0$. The [Fourier transform method for the wave equation](../../../wave-equation.md#fourier-transform-method-for-the-wave-equation) gives

$$
\partial_t^2\widehat E_t(\xi)+c^2|\xi|^2\widehat E_t(\xi)=0,
\qquad\boxed{\widehat E_t(\xi)=\cos(ct|\xi|)\widehat f(\xi).}
$$

This inverse [tempered distribution](../../../fourier-analysis.md#tempered-distribution) is twice differentiable in $t$: time derivatives introduce [polynomial](../../../polynomial.md) frequency factors, still integrable against every [Schwartz function](../../../fourier-analysis.md#schwartz-function). It has the specified initial displacement and zero initial velocity and satisfies the equation distributionally.

To apply the support theorem, replace the real norm by the [entire wave cosine multiplier](../../../wave-equation.md#entire-wave-cosine-multiplier)

$$
C_t(z)=\sum_{j=0}^\infty\frac{(-1)^j(ct)^{2j}(z\cdot z)^j}{(2j)!}.
$$

This series is entire and equals $\cos(ct\sqrt{z\cdot z})$ regardless of the square-root choice. Write $z=a+ib$ and $q=\sqrt{z\cdot z}$. Since $|z\cdot z|\le|a|^2+|b|^2$,

$$
(\operatorname{Im}q)^2
=\frac{|z\cdot z|-(|a|^2-|b|^2)}2\le|b|^2.
$$

Together with $|\cos w|\le e^{|\operatorname{Im}w|}$, this yields $|C_t(z)|\le e^{|c|t|\operatorname{Im}z|}$. The forward estimate for the translated initial support now gives

$$
|e^{iz\cdot y}C_t(z)\widehat f(z)|
\le C(1+|z|)^N e^{(\delta+|c|t)|\operatorname{Im}z|}.
$$

The converse therefore proves **finite propagation with the stated speed**:

$$
\boxed{\operatorname{supp}E_t\subset\overline B(y,\delta+|c|t),\qquad t>0.}
$$

In particular, $\sqrt{z\cdot z}$ itself need not be entire; it is the even cosine series that provides the required entire extension.

For completeness this construction identifies the distributional Cauchy solution even without initially assuming spatial temperedness. The zero-displacement wave multiplier is $S_\tau(z)=\int_0^\tau C_s(z)\,ds$, entire with bound $|S_\tau(z)|\le\tau e^{|c|\tau|\operatorname{Im}z|}$. Given a compactly supported smooth $\phi$ and final time $T$, the backward solution $w(s)=\mathcal F^{-1}[S_{T-s}\widehat\phi]$ is smooth, has support in one compact ball for $0\le s\le T$ by the same support theorem, and satisfies $w(T)=0$, $w_s(T)=-\phi$. For the difference $h$ of two distributional solutions with zero initial data,

$$
\frac d{ds}\big(\langle h_s,w\rangle-\langle h,w_s\rangle\big)
=c^2\big(\langle\Delta h,w\rangle-\langle h,\Delta w\rangle\big)=0.
$$

All pairings use compactly supported [test functions](../../../distribution-theory.md#test-function). The expression vanishes initially and equals $\langle h(T),\phi\rangle$ finally. Hence $h(T)=0$, establishing uniqueness in the usual time-differentiable distributional solution class.

## 3

↑ **Parent:** [Paper 67](paper-67.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use $D_j=-i\partial_{x_j}$, so the [Fourier transform](../../../analysis.md#fourier-transform) of $D^\alpha u$ is $\lambda^\alpha\widehat u$. Distinguish the full degree-$N$ [polynomial](../../../polynomial.md) $P(\lambda)$ from its homogeneous top-degree part $p_N(\lambda)$, the [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation). The [elliptic differential operator](../../../distribution-theory.md#elliptic-differential-operator) condition is

$$
\boxed{p_N(\lambda)\ne0\quad\text{for every real }\lambda\ne0.}
$$

It does not require the full [polynomial](../../../polynomial.md) to be nonzero at small frequencies. Compactness of the unit sphere gives $c_0=\min_{|\theta|=1}|p_N(\theta)|>0$. Homogeneity and the lower-degree remainder imply

$$
|P(\lambda)|\ge c_0|\lambda|^N-C(1+|\lambda|)^{N-1}.
$$

For sufficiently large $|\lambda|$ the second term is at most half the first, so the [high-frequency lower bound for an elliptic polynomial](../../../distribution-theory.md#high-frequency-lower-bound-for-an-elliptic-polynomial) is

$$
\boxed{|P(\lambda)|\ge c\langle\lambda\rangle^N,}
\qquad\langle\lambda\rangle=(1+|\lambda|^2)^{1/2}.
$$

Here $\langle\lambda\rangle$ is the [Japanese bracket](../../../analysis.md#japanese-bracket). The order-zero case just means a nonzero constant and is immediate.

For real $s$, the [Sobolev space](../../../sobolev-space.md) definition with the current Fourier normalization is

$$
H^s(\mathbb R^n)=\{u\in\mathcal S':\langle\lambda\rangle^s\widehat u\in L^2\},
\qquad\|u\|_{H^s}^2=(2\pi)^{-n}\int\langle\lambda\rangle^{2s}|\widehat u(\lambda)|^2\,d\lambda.
$$

Changing the harmless constant in the norm gives the same space. A [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) on $X$ belongs to the [Local Sobolev space](../../../sobolev-space.md#local-sobolev-space) $H^s_{\rm loc}(X)$ when $\chi u$, extended by zero outside $X$, belongs to $H^s(\mathbb R^n)$ for every [test function](../../../distribution-theory.md#test-function) $\chi\in C_c^\infty(X)$.

A [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution) of finite [order of a distribution](../../../distribution-theory.md#order-of-a-distribution) $m$ has a smooth [Fourier transform](../../../analysis.md#fourier-transform) satisfying $|\widehat u(\lambda)|\le C(1+|\lambda|)^m$, by applying the finite-order estimate to a fixed cutoff times the exponential. Thus its weighted squared transform is bounded by $C\langle\lambda\rangle^{2(s+m)}$. This is integrable precisely in the sufficient range $2(s+m)<-n$, and proves

$$
\boxed{u\in H^s(\mathbb R^n)\quad\text{for every }s<-m-n/2.}
$$

This is the [negative Sobolev regularity of a compactly supported distribution](../../../distribution-theory.md#negative-sobolev-regularity-of-a-compactly-supported-distribution); the strict inequality is important, and is not a claim that this sufficient threshold is optimal for each [distribution](../../../distribution-theory.md#distribution-mathematical-analysis).

To establish [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) without assuming the answer as an a priori smoothness hypothesis, first obtain a global constant-coefficient gain. For a compactly supported [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) $w$ with $P(D)w\in H^q$, the [polynomial](../../../polynomial.md) lower bound at high frequency gives

$$
\int_{|\lambda|\ge R}\langle\lambda\rangle^{2(q+N)}|\widehat w|^2\,d\lambda
\le C\int_{|\lambda|\ge R}\langle\lambda\rangle^{2q}|\widehat{P(D)w}|^2\,d\lambda<\infty.
$$

On $|\lambda|\le R$, the transform of $w$ is smooth and bounded. Therefore **$P(D)w\in H^q$ implies $w\in H^{q+N}$**. Possible low-frequency zeros of $P$ are harmless; we never divide by them.

Two elementary mapping facts supply the variable-coefficient argument. [Distributional derivatives](../../../distribution-theory.md#distributional-derivative) of order $j$ map $H^r$ into $H^{r-j}$. [Sobolev multiplication by a smooth cutoff](../../../sobolev-space.md#sobolev-multiplication-by-a-smooth-cutoff) is bounded on $H^r$ for every real $r$, including negative ones. Indeed, for a compactly supported smooth $a$, the [Peetre weight inequality](../../../analysis.md#peetre-weight-inequality)

$$
\langle\xi\rangle^r\le C_r\langle\eta\rangle^r\langle\xi-\eta\rangle^{|r|}
$$

and $\widehat{aw}=(2\pi)^{-n}\widehat a*\widehat w$ reduce the bound to [Young's convolution inequality](../../../fourier-analysis.md#young-s-convolution-inequality) with the integrable kernel $\langle\zeta\rangle^{|r|}|\widehat a(\zeta)|$. Smooth coefficients only need this property on compact subsets, where they can be multiplied by another cutoff.

Write the lower-order part as $B=\sum_{|\alpha|<N}f_\alpha D^\alpha$, with $N\ge1$, and suppose provisionally that $u\in H^r_{\rm loc}$ on a relatively compact neighborhood. For a [cutoff function](../../../distribution-theory.md#cutoff-function) $\chi$ supported there,

$$
P(D)(\chi u)=\chi Lu-\chi Bu+[P(D),\chi]u.
$$

The bracket is the operator [commutator](../../../lie-algebra.md#commutator). Its order is at most $N-1$: in the product rule, every surviving term has at least one derivative falling on $\chi$. Choose a second [cutoff function](../../../distribution-theory.md#cutoff-function) equal to one near $\operatorname{supp}\chi$ when estimating the products. The derivative and smooth-multiplication bounds then give

$$
\chi Bu,\ [P(D),\chi]u\in H^{r-N+1},\qquad \chi Lu\in H^s.
$$

The global gain just proved applies to the [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution) $\chi u$, and yields

$$
\boxed{u\in H^{\min(s+N,r+1)}_{\rm loc}.}
$$

This is the [cutoff bootstrap for local elliptic regularity](../../../distribution-theory.md#cutoff-bootstrap-for-local-elliptic-regularity); it works for real indices, not just nonnegative integers.

There is always a legitimate starting index. Around any fixed point choose $\chi_0=1$ on a smaller neighborhood. The [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution) $\chi_0u$ has the negative Sobolev regularity proved above, so $u\in H^{r_0}_{\rm loc}$ on that neighborhood for some finite $r_0$. The index need not be uniform over all of $X$. Repeating the one-step gain finitely many times reaches $s+N$, or the target is already reached if $r_0\ge s+N$. Since the point was arbitrary,

$$
\boxed{Lu\in H^s_{\rm loc}(X)\ \Longrightarrow\ u\in H^{s+N}_{\rm loc}(X).}
$$

For $N=0$ the result follows directly by dividing by the nonzero constant.

Finally, if $Lu=0$, its forcing belongs to every [Local Sobolev space](../../../sobolev-space.md#local-sobolev-space). The gain consequently gives every local Sobolev order for $u$. For each integer $j\ge0$, choose an order larger than $j+n/2$ and apply the [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) to a localized solution. It has a $C^j$ representative; the representatives agree because they represent the same [distribution](../../../distribution-theory.md#distribution-mathematical-analysis). Thus **every distributional solution of $Lu=0$ is smooth on $X$**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
