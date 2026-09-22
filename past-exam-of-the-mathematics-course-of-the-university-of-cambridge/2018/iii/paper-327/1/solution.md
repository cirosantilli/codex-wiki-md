<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat f(\xi)=\int e^{-ix\cdot\xi}f(x)\,dx$ and $D_j=-i\partial_{x_j}$. Thus $D_j$ has [Fourier symbol](../../../../../fourier-symbol-of-a-difference-operator.md) $\xi_j$. This fixes the factors of $i$ in the formula for a differentiated [Dirac delta distribution](../../../../../dirac-delta-function.md) below.

With the [Japanese bracket](../../../../../japanese-bracket.md) $\langle\theta\rangle=(1+|\theta|^2)^{1/2}$, the [symbol class](../../../../../symbol-class.md) $\operatorname{Sym}(X,\mathbb R^k;N)=S^N_{1,0}(X\times\mathbb R^k)$ consists of [smooth functions](../../../../../smooth-function.md) $a$ such that, for every [compact set](../../../../../compact-space.md) $K\subset X$ and all [multi-indices](../../../../../multi-index-notation.md) $\alpha,\beta$,

$$
\boxed{|\partial_x^\alpha\partial_\theta^\beta a(x,\theta)|
\leq C_{K,\alpha,\beta}\langle\theta\rangle^{N-|\beta|}\quad(x\in K).}
$$

Here $N$ is one fixed finite real order; the constants may depend on $K$. Differentiation in $x$ preserves the [symbol class](../../../../../symbol-class.md) order, whereas differentiation in $\theta$ lowers it.

A [phase function](../../../../../phase-function.md) is real-valued and smooth on $X\times(\mathbb R^k\setminus\{0\})$, is a [positively homogeneous function](../../../../../positively-homogeneous-function-degree-one.md) of degree one in $\theta$, and has nonzero total differential:

$$
\Phi(x,t\theta)=t\Phi(x,\theta)\quad(t>0),\qquad
(\nabla_x\Phi,\nabla_\theta\Phi)\ne0\quad(\theta\ne0).
$$

The nonvanishing condition concerns both sets of variables, not just $\nabla_\theta\Phi$. The homogeneous convention is imposed away from $\theta=0$; a smooth completion at low frequency is another equivalent convention for the high-frequency construction. Low-frequency changes contribute a [smooth function](../../../../../smooth-function.md) of $x$.

Choose a [cutoff function](../../../../../cutoff-function.md) $\rho(\theta)$ equal to one near zero. The low-frequency part with [oscillatory integral amplitude](../../../../../amplitude-of-an-oscillatory-integral.md) $\rho a$ is an ordinary convergent integral and defines a [smooth function](../../../../../smooth-function.md): all $x$ derivatives of $\Phi$ are $O_K(|\theta|)$ near zero, so differentiation under this integral preserves integrability. For the remaining part define, when $\theta\ne0$,

$$
G=|\nabla_x\Phi|^2+|\theta|^2|\nabla_\theta\Phi|^2,
\qquad
L=\frac1{iG}\left(\sum_j\partial_{x_j}\Phi\,\partial_{x_j}
+|\theta|^2\sum_\ell\partial_{\theta_\ell}\Phi\,\partial_{\theta_\ell}\right).
$$

Then $Le^{i\Phi}=e^{i\Phi}$. On $K\times\{\theta:|\theta|=1\}$, compactness and the [phase function](../../../../../phase-function.md) condition give a positive lower bound for $G$. Homogeneity consequently gives $G\geq c_K|\theta|^2$. The coefficient of each $x$ derivative in $L$ has [symbol class](../../../../../symbol-class.md) order $-1$, and the coefficient of each $\theta$ derivative has order zero.

If $L=\sum b_j\partial_{x_j}+\sum c_\ell\partial_{\theta_\ell}$, its [formal transpose](../../../../../formal-transpose-of-a-differential-operator.md) is

$$
L^t f=-\sum_j\partial_{x_j}(b_jf)-\sum_\ell\partial_{\theta_\ell}(c_\ell f).
$$

This is the bilinear transpose for [integration by parts](../../../../../integration-by-parts.md), without [complex conjugation](../../../../../complex-conjugation.md). It lowers the [symbol class](../../../../../symbol-class.md) order by one. For a [test function](../../../../../test-function.md) $\varphi$ supported in $K$, choose a nonnegative integer $r>N+k$ and set

$$
\begin{aligned}
\langle I_\Phi(a),\varphi\rangle={}&\int_X\int_{\mathbb R^k}e^{i\Phi}\rho a\varphi\,d\theta\,dx\\
&+\int_X\int_{\mathbb R^k}e^{i\Phi}(L^t)^r\bigl((1-\rho)a\varphi\bigr)\,d\theta\,dx.
\end{aligned}
$$

Both integrals are absolutely convergent, because the last [oscillatory integral amplitude](../../../../../amplitude-of-an-oscillatory-integral.md) has order $N-r<-k$ and [compact support](../../../../../compact-support.md) in $x$.

To verify that this defines the intended [oscillatory integral](../../../../../oscillatory-integral.md), take any $\chi\in C_c^\infty(\mathbb R^k)$ equal to one near zero and insert $\chi(\varepsilon\theta)$ in the original integral. Repeated [integration by parts](../../../../../integration-by-parts.md) gives the preceding expression with $(L^t)^r$ applied also to this [cutoff function](../../../../../cutoff-function.md). Its derivatives satisfy uniform [symbol class](../../../../../symbol-class.md) bounds: on the annulus where they are nonzero, $\varepsilon^{|\beta|}\leq C\langle\theta\rangle^{-|\beta|}$. The transformed integrands are bounded by an integrable multiple of $\langle\theta\rangle^{N-r}$. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) therefore proves

$$
\boxed{\langle I_\Phi(a),\varphi\rangle
=\lim_{\varepsilon\downarrow0}\int_X\int_{\mathbb R^k}
e^{i\Phi(x,\theta)}a(x,\theta)\varphi(x)\chi(\varepsilon\theta)\,d\theta\,dx.}
$$

It also proves independence of the [cutoff function](../../../../../cutoff-function.md), the chosen $r$, and the integration-by-parts representation.

At most $r$ derivatives fall on $\varphi$, so the same estimates give

$$
\boxed{|\langle I_\Phi(a),\varphi\rangle|
\leq C_K\max_{|\alpha|\leq r}\|\partial^\alpha\varphi\|_\infty,
\qquad I_\Phi(a)\in\mathcal D'(X).}
$$

This proves linearity and continuity on the [space of test functions](../../../../../space-of-test-functions.md). It also proves the [finite order of an oscillatory integral distribution](../../../../../finite-order-of-an-oscillatory-integral-distribution.md): the derivative bound uses the same $r$ for every $K$, although $C_K$ changes.

For $x_0\in X$, take $k=n$, $\Phi=(x-x_0)\cdot\theta$, and $a=(2\pi)^{-n}\theta^\alpha$. This [phase function](../../../../../phase-function.md) is valid because $\nabla_x\Phi=\theta\ne0$ for nonzero $\theta$, and the [oscillatory integral amplitude](../../../../../amplitude-of-an-oscillatory-integral.md) is in [symbol class](../../../../../symbol-class.md) $S^{|\alpha|}_{1,0}$. The required identity is

$$
\boxed{D^\alpha\delta_{x_0}=(2\pi)^{-n}\int_{\mathbb R^n}
e^{i(x-x_0)\cdot\theta}\theta^\alpha\,d\theta.}
$$

Indeed, extending a [test function](../../../../../test-function.md) by zero outside $X$ and integrating in $x$ first gives the absolutely convergent expression

$$
(2\pi)^{-n}\int e^{-ix_0\cdot\theta}\theta^\alpha\widehat\varphi(-\theta)\,d\theta
=(2\pi)^{-n}\int e^{ix_0\cdot\xi}(-\xi)^\alpha\widehat\varphi(\xi)\,d\xi
=i^{|\alpha|}\partial^\alpha\varphi(x_0).
$$

Here [Fourier inversion](../../../../../fourier-inversion-theorem.md) applies because $\varphi$ is a [Schwartz function](../../../../../schwartz-function.md). By the definition of a [distributional derivative](../../../../../distributional-derivative.md), the last expression is precisely $\langle D^\alpha\delta_{x_0},\varphi\rangle$. If $D^\alpha$ is instead used for plain $\partial^\alpha$, the [oscillatory integral amplitude](../../../../../amplitude-of-an-oscillatory-integral.md) in the boxed formula is $(2\pi)^{-n}(i\theta)^\alpha$, and the pairing is $(-1)^{|\alpha|}\partial^\alpha\varphi(x_0)$.

**Not every [distribution](../../../../../distribution-mathematical-analysis.md) is one [oscillatory integral](../../../../../oscillatory-integral.md) of the stated class.** On $X=\mathbb R$, consider the locally finite [distribution of unbounded order](../../../../../distribution-of-unbounded-order.md)

$$
T=\sum_{j=1}^\infty D^j\delta_j.
$$

Only finitely many differentiated [Dirac delta distributions](../../../../../dirac-delta-function.md) contribute to each [test function](../../../../../test-function.md), so $T$ is a [distribution](../../../../../distribution-mathematical-analysis.md). Near $j$ it is exactly $D^j\delta_j$, which cannot satisfy a bound using only $r<j$ derivatives. Explicitly choose $\eta\in C_c^\infty((-1/4,1/4))$ with $\eta^{(j)}(0)\ne0$ and use

$$
\varphi_\varepsilon(x)=\varepsilon^r\eta((x-j)/\varepsilon).
$$

The derivatives through order $r$ remain bounded for $0<\varepsilon\leq1$, whereas

$$
|\langle T,\varphi_\varepsilon\rangle|
=\varepsilon^{r-j}|\eta^{(j)}(0)|\longrightarrow\infty.
$$

Any single [oscillatory integral](../../../../../oscillatory-integral.md) with finite $k$ and a fixed finite [symbol class](../../../../../symbol-class.md) order $N$ has the uniform order bound just proved, so it cannot equal $T$. The same construction works on any nonempty [open set](../../../../../open-set.md) in positive dimension by choosing points that leave every [compact set](../../../../../compact-space.md) and taking locally finite differentiated [Dirac delta distributions](../../../../../dirac-delta-function.md) there. This obstruction concerns a single fixed-order [oscillatory integral](../../../../../oscillatory-integral.md), rather than local representations or an infinite sum of them.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 327](../../paper-327-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
