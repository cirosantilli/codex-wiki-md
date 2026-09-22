# Paper 327

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_327.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_327.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat f(\xi)=\int e^{-ix\cdot\xi}f(x)\,dx$ and $D_j=-i\partial_{x_j}$. Thus $D_j$ has [Fourier symbol](../../../finite-difference.md#fourier-symbol-of-a-difference-operator) $\xi_j$. This fixes the factors of $i$ in the formula for a differentiated [Dirac delta distribution](../../../distribution-theory.md#dirac-delta-function) below.

With the [Japanese bracket](../../../analysis.md#japanese-bracket) $\langle\theta\rangle=(1+|\theta|^2)^{1/2}$, the [symbol class](../../../distribution-theory.md#symbol-class) $\operatorname{Sym}(X,\mathbb R^k;N)=S^N_{1,0}(X\times\mathbb R^k)$ consists of [smooth functions](../../../analysis.md#smooth-function) $a$ such that, for every [compact set](../../../topology.md#compact-space) $K\subset X$ and all [multi-indices](../../../distribution-theory.md#multi-index-notation) $\alpha,\beta$,

$$
\boxed{|\partial_x^\alpha\partial_\theta^\beta a(x,\theta)|
\leq C_{K,\alpha,\beta}\langle\theta\rangle^{N-|\beta|}\quad(x\in K).}
$$

Here $N$ is one fixed finite real order; the constants may depend on $K$. Differentiation in $x$ preserves the [symbol class](../../../distribution-theory.md#symbol-class) order, whereas differentiation in $\theta$ lowers it.

A [phase function](../../../distribution-theory.md#phase-function) is real-valued and smooth on $X\times(\mathbb R^k\setminus\{0\})$, is a [positively homogeneous function](../../../real-analysis.md#positively-homogeneous-function-degree-one) of degree one in $\theta$, and has nonzero total differential:

$$
\Phi(x,t\theta)=t\Phi(x,\theta)\quad(t>0),\qquad
(\nabla_x\Phi,\nabla_\theta\Phi)\ne0\quad(\theta\ne0).
$$

The nonvanishing condition concerns both sets of variables, not just $\nabla_\theta\Phi$. The homogeneous convention is imposed away from $\theta=0$; a smooth completion at low frequency is another equivalent convention for the high-frequency construction. Low-frequency changes contribute a [smooth function](../../../analysis.md#smooth-function) of $x$.

Choose a [cutoff function](../../../distribution-theory.md#cutoff-function) $\rho(\theta)$ equal to one near zero. The low-frequency part with [oscillatory integral amplitude](../../../distribution-theory.md#amplitude-of-an-oscillatory-integral) $\rho a$ is an ordinary convergent integral and defines a [smooth function](../../../analysis.md#smooth-function): all $x$ derivatives of $\Phi$ are $O_K(|\theta|)$ near zero, so differentiation under this integral preserves integrability. For the remaining part define, when $\theta\ne0$,

$$
G=|\nabla_x\Phi|^2+|\theta|^2|\nabla_\theta\Phi|^2,
\qquad
L=\frac1{iG}\left(\sum_j\partial_{x_j}\Phi\,\partial_{x_j}
+|\theta|^2\sum_\ell\partial_{\theta_\ell}\Phi\,\partial_{\theta_\ell}\right).
$$

Then $Le^{i\Phi}=e^{i\Phi}$. On $K\times\{\theta:|\theta|=1\}$, compactness and the [phase function](../../../distribution-theory.md#phase-function) condition give a positive lower bound for $G$. Homogeneity consequently gives $G\geq c_K|\theta|^2$. The coefficient of each $x$ derivative in $L$ has [symbol class](../../../distribution-theory.md#symbol-class) order $-1$, and the coefficient of each $\theta$ derivative has order zero.

If $L=\sum b_j\partial_{x_j}+\sum c_\ell\partial_{\theta_\ell}$, its [formal transpose](../../../analysis.md#formal-transpose-of-a-differential-operator) is

$$
L^t f=-\sum_j\partial_{x_j}(b_jf)-\sum_\ell\partial_{\theta_\ell}(c_\ell f).
$$

This is the bilinear transpose for [integration by parts](../../../calculus.md#integration-by-parts), without [complex conjugation](../../../complex-analysis.md#complex-conjugation). It lowers the [symbol class](../../../distribution-theory.md#symbol-class) order by one. For a [test function](../../../distribution-theory.md#test-function) $\varphi$ supported in $K$, choose a nonnegative integer $r>N+k$ and set

$$
\begin{aligned}
\langle I_\Phi(a),\varphi\rangle={}&\int_X\int_{\mathbb R^k}e^{i\Phi}\rho a\varphi\,d\theta\,dx\\
&+\int_X\int_{\mathbb R^k}e^{i\Phi}(L^t)^r\bigl((1-\rho)a\varphi\bigr)\,d\theta\,dx.
\end{aligned}
$$

Both integrals are absolutely convergent, because the last [oscillatory integral amplitude](../../../distribution-theory.md#amplitude-of-an-oscillatory-integral) has order $N-r<-k$ and [compact support](../../../function.md#compact-support) in $x$.

To verify that this defines the intended [oscillatory integral](../../../distribution-theory.md#oscillatory-integral), take any $\chi\in C_c^\infty(\mathbb R^k)$ equal to one near zero and insert $\chi(\varepsilon\theta)$ in the original integral. Repeated [integration by parts](../../../calculus.md#integration-by-parts) gives the preceding expression with $(L^t)^r$ applied also to this [cutoff function](../../../distribution-theory.md#cutoff-function). Its derivatives satisfy uniform [symbol class](../../../distribution-theory.md#symbol-class) bounds: on the annulus where they are nonzero, $\varepsilon^{|\beta|}\leq C\langle\theta\rangle^{-|\beta|}$. The transformed integrands are bounded by an integrable multiple of $\langle\theta\rangle^{N-r}$. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) therefore proves

$$
\boxed{\langle I_\Phi(a),\varphi\rangle
=\lim_{\varepsilon\downarrow0}\int_X\int_{\mathbb R^k}
e^{i\Phi(x,\theta)}a(x,\theta)\varphi(x)\chi(\varepsilon\theta)\,d\theta\,dx.}
$$

It also proves independence of the [cutoff function](../../../distribution-theory.md#cutoff-function), the chosen $r$, and the integration-by-parts representation.

At most $r$ derivatives fall on $\varphi$, so the same estimates give

$$
\boxed{|\langle I_\Phi(a),\varphi\rangle|
\leq C_K\max_{|\alpha|\leq r}\|\partial^\alpha\varphi\|_\infty,
\qquad I_\Phi(a)\in\mathcal D'(X).}
$$

This proves linearity and continuity on the [space of test functions](../../../distribution-theory.md#space-of-test-functions). It also proves the [finite order of an oscillatory integral distribution](../../../distribution-theory.md#finite-order-of-an-oscillatory-integral-distribution): the derivative bound uses the same $r$ for every $K$, although $C_K$ changes.

For $x_0\in X$, take $k=n$, $\Phi=(x-x_0)\cdot\theta$, and $a=(2\pi)^{-n}\theta^\alpha$. This [phase function](../../../distribution-theory.md#phase-function) is valid because $\nabla_x\Phi=\theta\ne0$ for nonzero $\theta$, and the [oscillatory integral amplitude](../../../distribution-theory.md#amplitude-of-an-oscillatory-integral) is in [symbol class](../../../distribution-theory.md#symbol-class) $S^{|\alpha|}_{1,0}$. The required identity is

$$
\boxed{D^\alpha\delta_{x_0}=(2\pi)^{-n}\int_{\mathbb R^n}
e^{i(x-x_0)\cdot\theta}\theta^\alpha\,d\theta.}
$$

Indeed, extending a [test function](../../../distribution-theory.md#test-function) by zero outside $X$ and integrating in $x$ first gives the absolutely convergent expression

$$
(2\pi)^{-n}\int e^{-ix_0\cdot\theta}\theta^\alpha\widehat\varphi(-\theta)\,d\theta
=(2\pi)^{-n}\int e^{ix_0\cdot\xi}(-\xi)^\alpha\widehat\varphi(\xi)\,d\xi
=i^{|\alpha|}\partial^\alpha\varphi(x_0).
$$

Here [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) applies because $\varphi$ is a [Schwartz function](../../../fourier-analysis.md#schwartz-function). By the definition of a [distributional derivative](../../../distribution-theory.md#distributional-derivative), the last expression is precisely $\langle D^\alpha\delta_{x_0},\varphi\rangle$. If $D^\alpha$ is instead used for plain $\partial^\alpha$, the [oscillatory integral amplitude](../../../distribution-theory.md#amplitude-of-an-oscillatory-integral) in the boxed formula is $(2\pi)^{-n}(i\theta)^\alpha$, and the pairing is $(-1)^{|\alpha|}\partial^\alpha\varphi(x_0)$.

**Not every [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) is one [oscillatory integral](../../../distribution-theory.md#oscillatory-integral) of the stated class.** On $X=\mathbb R$, consider the locally finite [distribution of unbounded order](../../../distribution-theory.md#distribution-of-unbounded-order)

$$
T=\sum_{j=1}^\infty D^j\delta_j.
$$

Only finitely many differentiated [Dirac delta distributions](../../../distribution-theory.md#dirac-delta-function) contribute to each [test function](../../../distribution-theory.md#test-function), so $T$ is a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis). Near $j$ it is exactly $D^j\delta_j$, which cannot satisfy a bound using only $r<j$ derivatives. Explicitly choose $\eta\in C_c^\infty((-1/4,1/4))$ with $\eta^{(j)}(0)\ne0$ and use

$$
\varphi_\varepsilon(x)=\varepsilon^r\eta((x-j)/\varepsilon).
$$

The derivatives through order $r$ remain bounded for $0<\varepsilon\leq1$, whereas

$$
|\langle T,\varphi_\varepsilon\rangle|
=\varepsilon^{r-j}|\eta^{(j)}(0)|\longrightarrow\infty.
$$

Any single [oscillatory integral](../../../distribution-theory.md#oscillatory-integral) with finite $k$ and a fixed finite [symbol class](../../../distribution-theory.md#symbol-class) order $N$ has the uniform order bound just proved, so it cannot equal $T$. The same construction works on any nonempty [open set](../../../topology.md#open-set) in positive dimension by choosing points that leave every [compact set](../../../topology.md#compact-space) and taking locally finite differentiated [Dirac delta distributions](../../../distribution-theory.md#dirac-delta-function) there. This obstruction concerns a single fixed-order [oscillatory integral](../../../distribution-theory.md#oscillatory-integral), rather than local representations or an infinite sum of them.

## 2

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [space of test functions](../../../distribution-theory.md#space-of-test-functions) is $\mathcal D(\mathbb R)=C_c^\infty(\mathbb R)$. A sequence $\varphi_j$ converges to $\varphi$ when all functions eventually have [compact support](../../../function.md#compact-support) in one [compact set](../../../topology.md#compact-space) $K$ and every derivative converges uniformly:

$$
\|\varphi_j^{(q)}-\varphi^{(q)}\|_\infty\longrightarrow0
\quad\text{for each integer }q\geq0.
$$

A [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) is a continuous linear functional on this [space of test functions](../../../distribution-theory.md#space-of-test-functions). Equivalently, for each [compact set](../../../topology.md#compact-space) $K$, there are $C_K$ and a finite integer $m_K$ such that

$$
|\langle u,\varphi\rangle|\leq C_K\max_{0\leq q\leq m_K}\|\varphi^{(q)}\|_\infty
\quad\text{whenever }\operatorname{supp}\varphi\subseteq K.
$$

The integer $m_K$ is permitted to depend on $K$. The usual [weak convergence of distributions](../../../distribution-theory.md#weak-convergence-of-distributions) is

$$
\boxed{u_j\longrightarrow u\text{ in }\mathcal D'(\mathbb R)
\quad\Longleftrightarrow\quad
\langle u_j,\varphi\rangle\longrightarrow\langle u,\varphi\rangle
\text{ for every }\varphi\in\mathcal D(\mathbb R).}
$$

Thus the convergence convention on the [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) space is its weak dual topology.

For the [principal-value reciprocal distribution](../../../distribution-theory.md#principal-value-reciprocal-distribution), the symmetric truncations can be written

$$
\left\langle\operatorname{pv}\frac1x,\varphi\right\rangle
=\lim_{\varepsilon\downarrow0}\int_{|x|>\varepsilon}\frac{\varphi(x)}x\,dx
=\int_0^\infty\frac{\varphi(x)-\varphi(-x)}x\,dx.
$$

The numerator is $O(x)$ near zero by the [mean value theorem](../../../calculus.md#mean-value-theorem), and the integrand vanishes for large $x$ because $\varphi$ has [compact support](../../../function.md#compact-support). For $\operatorname{supp}\varphi\subset[-R,R]$,

$$
\left|\left\langle\operatorname{pv}\frac1x,\varphi\right\rangle\right|
\leq2R\|\varphi'\|_\infty.
$$

Consequently the [Cauchy principal value](../../../complex-analysis.md#cauchy-principal-value) defines a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) of [order of a distribution](../../../distribution-theory.md#order-of-a-distribution) at most one.

The function $\log|x|$ has [local integrability](../../../distribution-theory.md#locally-integrable-function), since $\int_0^1|\log x|\,dx<\infty$, and therefore defines a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis). For its [distributional derivative](../../../distribution-theory.md#distributional-derivative), remove $(-\varepsilon,\varepsilon)$ and use [integration by parts](../../../calculus.md#integration-by-parts) on both remaining intervals:

$$
-\int_{|x|>\varepsilon}\log|x|\,\varphi'(x)\,dx
=\int_{|x|>\varepsilon}\frac{\varphi(x)}x\,dx
+\log\varepsilon\,[\varphi(\varepsilon)-\varphi(-\varepsilon)].
$$

The boundary term is $O(\varepsilon|\log\varepsilon|)$ and tends to zero. The omitted integral of $\log|x|\varphi'$ tends to zero by [local integrability](../../../distribution-theory.md#locally-integrable-function). Hence the [distributional derivative of the logarithmic modulus](../../../distribution-theory.md#distributional-derivative-of-the-logarithmic-modulus) satisfies

$$
\boxed{\frac{d}{dx}\log|x|=\operatorname{pv}\frac1x\quad\text{in }\mathcal D'(\mathbb R).}
$$

Symmetric truncation is essential to this normalization of the [principal-value reciprocal distribution](../../../distribution-theory.md#principal-value-reciprocal-distribution).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $T_q\varphi(x)=\sum_{k=0}^q\varphi^{(k)}(0)x^k/k!$ denote the [Taylor polynomial](../../../calculus.md#taylor-polynomial) at zero. On $0<|x|<1$, the integrand defining the [Hadamard finite-part reciprocal-power distribution](../../../distribution-theory.md#hadamard-finite-part-reciprocal-power-distribution) is

$$
x^{-m}\bigl(\varphi(x)-T_{m-2}\varphi(x)\bigr)
=\frac{\varphi^{(m-1)}(0)}{(m-1)!}\frac1x
+x^{-m}\bigl(\varphi(x)-T_{m-1}\varphi(x)\bigr).
$$

The first term is odd, so it cancels under symmetric truncation. The [Taylor remainder](../../../calculus.md#taylor-remainder) in the second term has absolute value at most $|x|^m\|\varphi^{(m)}\|_\infty/m!$. The integral near zero therefore has a finite limit. For $|x|\geq1$, the original terms are integrable: $x^{-m}\varphi$ has [compact support](../../../function.md#compact-support), and each subtracted power has exponent $k-m\leq-2$.

This proves existence and linearity. It also gives the global estimate

$$
\begin{aligned}
|\langle\Lambda_m,\varphi\rangle|\leq{}&\frac2{m!}\|\varphi^{(m)}\|_\infty
+\frac2{m-1}\|\varphi\|_\infty\\
&+\sum_{k=0}^{m-2}\frac2{k!(m-k-1)}|\varphi^{(k)}(0)|.
\end{aligned}
$$

Thus

$$
\boxed{\Lambda_m\in\mathcal D'(\mathbb R),\qquad
\operatorname{ord}\Lambda_m\leq m.}
$$

In particular the [order of a distribution](../../../distribution-theory.md#order-of-a-distribution) is bounded by one integer on all [compact sets](../../../topology.md#compact-space), not merely separately on each of them.

For the recurrence, write the truncated [Hadamard finite-part integral](../../../distribution-theory.md#hadamard-finite-part-integral) as

$$
A_m(\varepsilon,\varphi)=\int_{|x|>\varepsilon}x^{-m}\varphi(x)\,dx
-C_m(\varepsilon,\varphi),
$$

where parity evaluates all subtraction integrals explicitly:

$$
C_m(\varepsilon,\varphi)=
2\sum_{\substack{0\leq k\leq m-2\\m-k\text{ even}}}
\frac{\varphi^{(k)}(0)}{k!(m-k-1)}\varepsilon^{k-m+1}.
$$

Set $C_1=0$ and $\Lambda_1=\operatorname{pv}(1/x)$. On the two truncated intervals, [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\int_{|x|>\varepsilon}x^{-m}\varphi'(x)\,dx
=m\int_{|x|>\varepsilon}x^{-m-1}\varphi(x)\,dx
+\varepsilon^{-m}\bigl[(-1)^m\varphi(-\varepsilon)-\varphi(\varepsilon)\bigr].
$$

There are no boundary contributions at infinity. The coefficients of the subtraction terms satisfy

$$
mC_{m+1}(\varepsilon,\varphi)-C_m(\varepsilon,\varphi')
=2\sum_{\substack{0\leq k\leq m-1\\m-k\text{ odd}}}
\frac{\varphi^{(k)}(0)}{k!}\varepsilon^{k-m}.
$$

This is exactly the negative of the boundary term's [Taylor polynomial](../../../calculus.md#taylor-polynomial) through degree $m$; the degree-$m$ term itself vanishes by parity. Hence

$$
\begin{aligned}
&A_m(\varepsilon,\varphi')-mA_{m+1}(\varepsilon,\varphi)\\
&\quad=\varepsilon^{-m}\left[
(-1)^m\bigl(\varphi(-\varepsilon)-T_m\varphi(-\varepsilon)\bigr)
-\bigl(\varphi(\varepsilon)-T_m\varphi(\varepsilon)\bigr)\right]
=O(\varepsilon).
\end{aligned}
$$

Taking the limit proves the full [distributional identity](../../../distribution-theory.md#distributional-identity)

$$
\boxed{\langle\Lambda_m,\varphi'\rangle=m\langle\Lambda_{m+1},\varphi\rangle,
\qquad \Lambda_m'=-m\Lambda_{m+1}.}
$$

The same calculation includes $m=1$. Starting with the [distributional derivative of the logarithmic modulus](../../../distribution-theory.md#distributional-derivative-of-the-logarithmic-modulus) from part (i), induction yields

$$
\boxed{\Lambda_m=\frac{(-1)^{m-1}}{(m-1)!}\left(\frac d{dx}\right)^m\log|x|,
\qquad c_m=\frac{(-1)^{m-1}}{(m-1)!}.}
$$

This identity holds on all of $\mathbb R$ as a [distributional identity](../../../distribution-theory.md#distributional-identity). It is stronger than matching the ordinary derivatives away from zero, which would leave possible differentiated [Dirac delta distributions](../../../distribution-theory.md#dirac-delta-function) at zero undetermined.

## 3

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Take $D_j=-i\partial_{x_j}$ and the [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat f(\lambda)=\int e^{-ix\cdot\lambda}f(x)\,dx$. Write the scalar [polynomial](../../../polynomial.md) as $P=P_N+P_{N-1}+\cdots+P_0$, with $P_j$ homogeneous of degree $j$. The [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) of the constant-coefficient [linear partial differential operator](../../../partial-differential-equation.md#linear-partial-differential-operator) $P(D)$ is $P_N$. It is an [elliptic differential operator](../../../distribution-theory.md#elliptic-differential-operator) exactly when

$$
\boxed{P_N(\lambda)\ne0\quad\text{for every real }\lambda\ne0.}
$$

Complex coefficients are allowed, but the frequency $\lambda$ is real.

By compactness of the unit [sphere](../../../geometry-and-topology.md#sphere), $c=\min_{|\omega|=1}|P_N(\omega)|>0$. Homogeneity gives $|P_N(\lambda)|\geq c|\lambda|^N$, whereas the lower-degree terms are bounded by $C|\lambda|^{N-1}$ for $|\lambda|\geq1$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) then gives the [high-frequency lower bound for an elliptic polynomial](../../../distribution-theory.md#high-frequency-lower-bound-for-an-elliptic-polynomial):

$$
|P(\lambda)|\geq c|\lambda|^N-C|\lambda|^{N-1}
\geq\frac c2|\lambda|^N\geq c'\langle\lambda\rangle^N
$$

for sufficiently large $|\lambda|$. Thus

$$
\boxed{|P(\lambda)|\gtrsim\langle\lambda\rangle^N\quad(|\lambda|\geq R).}
$$

The [Japanese bracket](../../../analysis.md#japanese-bracket) is $\langle\lambda\rangle=(1+|\lambda|^2)^{1/2}$. If $N=0$, a nonzero constant $P$ satisfies the same assertion directly.

For real $s$, the [Sobolev space](../../../sobolev-space.md) is the [tempered distribution](../../../fourier-analysis.md#tempered-distribution) space

$$
H^s(\mathbb R^n)=\left\{u\in\mathcal S'(\mathbb R^n):
\widehat u\text{ is a function and }
\int_{\mathbb R^n}\langle\lambda\rangle^{2s}|\widehat u(\lambda)|^2\,d\lambda<\infty\right\}.
$$

One may include $(2\pi)^{-n}$ in the squared norm for this [Fourier transform](../../../analysis.md#fourier-transform) normalization; it does not change the space. The [Local Sobolev space](../../../sobolev-space.md#local-sobolev-space) is

$$
H^s_{\mathrm{loc}}(X)=\{u\in\mathcal D'(X):\chi u\in H^s(\mathbb R^n)
\text{ for every }\chi\in C_c^\infty(X)\},
$$

where [multiplication of a distribution by a smooth function](../../../distribution-theory.md#multiplication-of-a-distribution-by-a-smooth-function) is followed by extension by zero.

If $u$ is a [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution), choose a [cutoff function](../../../distribution-theory.md#cutoff-function) $\chi$ equal to one near its [compact support](../../../function.md#compact-support). The finite [order of a distribution](../../../distribution-theory.md#order-of-a-distribution) gives an integer $M$ and a bound

$$
|\langle u,\psi\rangle|\leq C\max_{|\alpha|\leq M}
\sup_{x\in K}|\partial^\alpha\psi(x)|
$$

for a fixed [compact set](../../../topology.md#compact-space) $K$. This also makes $u$ a [tempered distribution](../../../fourier-analysis.md#tempered-distribution). Its [Fourier transform of a compactly supported distribution](../../../distribution-theory.md#fourier-transform-of-a-compactly-supported-distribution) is the [smooth function](../../../analysis.md#smooth-function)

$$
\widehat u(\lambda)=\langle u,\chi(x)e^{-ix\cdot\lambda}\rangle,
\qquad |\widehat u(\lambda)|\leq C'\langle\lambda\rangle^M.
$$

The [Leibniz rule](../../../calculus.md#leibniz-rule) gives the last estimate, and parameter differentiation under the finite-order pairing proves smoothness of this [Fourier transform](../../../analysis.md#fourier-transform). Therefore the [negative Sobolev regularity of a compactly supported distribution](../../../distribution-theory.md#negative-sobolev-regularity-of-a-compactly-supported-distribution) is

$$
\boxed{u\in H^s(\mathbb R^n)\quad\text{for every }s<-M-\frac n2.}
$$

Indeed $\langle\lambda\rangle^{2(s+M)}$ is integrable precisely when $2(s+M)<-n$. This proves the claimed existence of a sufficiently negative [Sobolev space](../../../sobolev-space.md) index.

We use three elementary [Sobolev space](../../../sobolev-space.md) facts: differentiation of order $q$ maps $H^t$ continuously into $H^{t-q}$; $H^a\subseteq H^b$ for $a\geq b$; and [Sobolev multiplication by a smooth cutoff](../../../sobolev-space.md#sobolev-multiplication-by-a-smooth-cutoff) is bounded on $H^t$ for every real $t$. The first two follow directly from the frequency weights. For the third, [multiplication of a distribution by a smooth function](../../../distribution-theory.md#multiplication-of-a-distribution-by-a-smooth-function) becomes convolution with the rapidly decaying $\widehat\chi$, and

$$
\langle\lambda\rangle^t\leq C_t\langle\lambda-\eta\rangle^{|t|}\langle\eta\rangle^t
$$

together with [Young's convolution inequality](../../../fourier-analysis.md#young-s-convolution-inequality) gives the bound. These facts apply after localization as well.

The [high-frequency lower bound for an elliptic polynomial](../../../distribution-theory.md#high-frequency-lower-bound-for-an-elliptic-polynomial) gives a useful global implication. If $w\in H^r(\mathbb R^n)$ and $P(D)w\in H^t(\mathbb R^n)$, split its [Fourier transform](../../../analysis.md#fourier-transform) into $|\lambda|\leq R$ and $|\lambda|>R$. The low-frequency part is controlled by $\|w\|_{H^r}$, while the high-frequency part is controlled by $\|P(D)w\|_{H^t}$. Thus, for arbitrary real $r,t$,

$$
\boxed{\|w\|_{H^{t+N}}\leq C_{r,t}\left(\|P(D)w\|_{H^t}+\|w\|_{H^r}\right).}
$$

The conclusion that $w\in H^{t+N}$ is obtained directly by integrating these frequency bounds; it is not an assumption made to state the estimate.

For the [cutoff bootstrap for local elliptic regularity](../../../distribution-theory.md#cutoff-bootstrap-for-local-elliptic-regularity), fix $U\Subset X$. A [cutoff function](../../../distribution-theory.md#cutoff-function) equal to one near $\overline U$ makes $u$ a [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution) after multiplication, so the preceding negative-index argument gives $u\in H^r_{\mathrm{loc}}(U)$ for some finite $r$. Suppose inductively that $u\in H^q_{\mathrm{loc}}(U)$. For any [test function](../../../distribution-theory.md#test-function) $\chi\in C_c^\infty(U)$,

$$
P(D)(\chi u)=\chi P(D)u+[P(D),\chi]u.
$$

The [Leibniz rule](../../../calculus.md#leibniz-rule) shows that this [commutator](../../../lie-algebra.md#commutator) has order at most $N-1$, with [smooth functions](../../../analysis.md#smooth-function) as coefficients, all with [compact support](../../../function.md#compact-support):

$$
[P(D),\chi]=\sum_{|\alpha|\leq N}p_\alpha
\sum_{0<\beta\leq\alpha}\binom\alpha\beta
(D^\beta\chi)D^{\alpha-\beta}.
$$

A second [cutoff function](../../../distribution-theory.md#cutoff-function) equal to one near $\operatorname{supp}\chi$ lets us apply the stated [Sobolev space](../../../sobolev-space.md) bounds to every term. Hence $[P(D),\chi]u\in H^{q-N+1}(\mathbb R^n)$, while $\chi P(D)u\in H^s(\mathbb R^n)$. For $N\geq1$, the global estimate yields

$$
\chi u\in H^{\min(s,q-N+1)+N}
=H^{\min(s+N,q+1)}.
$$

This holds for every such $\chi$, so it improves the [Local Sobolev space](../../../sobolev-space.md#local-sobolev-space) index by one until $s+N$ is reached. A finite number of iterations starting at $r$ proves

$$
\boxed{P(D)u\in H^s_{\mathrm{loc}}(X)\quad\Longrightarrow\quad
u\in H^{s+N}_{\mathrm{loc}}(X).}
$$

Since $U\Subset X$ was arbitrary, the conclusion holds throughout $X$. For $N=0$, division by the nonzero constant $P$ proves it immediately. This is the asserted [elliptic regularity](../../../distribution-theory.md#elliptic-regularity), proved without assuming an initial nonnegative [Sobolev space](../../../sobolev-space.md) index.

A first-order example on $\mathbb R^2$ is the [first-order Cauchy-Riemann operator](../../../analysis.md#first-order-cauchy-riemann-operator)

$$
\boxed{P(D)=D_1+iD_2=-2i\,\partial_{\bar z},\qquad
P_1(\lambda)=\lambda_1+i\lambda_2,\qquad |P_1(\lambda)|=|\lambda|.}
$$

It is an [elliptic differential operator](../../../distribution-theory.md#elliptic-differential-operator) with complex coefficients. In one real variable, $D=-i\,d/dx$ is already a first-order [elliptic differential operator](../../../distribution-theory.md#elliptic-differential-operator).

**There is no scalar [elliptic differential operator](../../../distribution-theory.md#elliptic-differential-operator) of odd order in three variables.** If its order $N$ were odd, its [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) would satisfy $P_N(-\omega)=-P_N(\omega)$ on $S^2$. Regard the [continuous map](../../../topology.md#continuous-map)

$$
f:S^2\longrightarrow\mathbb R^2,\qquad
f(\omega)=(\operatorname{Re}P_N(\omega),\operatorname{Im}P_N(\omega)).
$$

The [Borsuk-Ulam theorem](../../../algebraic-topology.md#borsuk-ulam-theorem) gives $f(\omega)=f(-\omega)$ for some $\omega$. Oddness then gives $f(\omega)=0$, contradicting ellipticity. This is the [odd-order obstruction for scalar elliptic operators in at least three dimensions](../../../distribution-theory.md#odd-order-obstruction-for-scalar-elliptic-operators-in-at-least-three-dimensions); restricting to a three-dimensional subspace proves the higher-dimensional case too. For real coefficients alone, the same obstruction follows from the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) along a path between antipodal points.

The scalar qualification matters. An [elliptic system of differential equations](../../../distribution-theory.md#elliptic-system-of-differential-equations) can be first order in three variables: with the [Pauli matrices](../../../algebra.md#pauli-matrices), the matrix symbol $A(\lambda)=\sum_{j=1}^3\sigma_j\lambda_j$ satisfies $A(\lambda)^2=|\lambda|^2\mathbf1$ and is invertible for $\lambda\ne0$. This does not contradict the scalar [polynomial](../../../polynomial.md) obstruction.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
