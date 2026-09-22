# Paper 71

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_71.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_71.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)

## 1

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use complex-linear [distributions](../../../distribution-theory.md#distribution-mathematical-analysis), so the pairing contains no complex conjugation. The [space of smooth functions](../../../distribution-theory.md#space-of-smooth-functions) is $\mathcal E(X)=C^\infty(X)$, with [seminorms](../../../topological-vector-space.md#seminorm)

$$
p_{K,r}(f)=\max_{|\alpha|\leq r}\sup_{x\in K}|\partial^\alpha f(x)|,\qquad K\Subset X.
$$

Thus $f_j\to f$ means uniform convergence of every [derivative](../../../calculus.md#derivative) on every [compact subset](../../../topology.md#compact-space) of $X$. A cofinal [compact exhaustion](../../../topology.md#compact-exhaustion) with $K_j\subset\operatorname{int}K_{j+1}$ makes $p_j=p_{K_j,j}$ an increasing defining family. Such an exhaustion exists for every [open set](../../../topology.md#open-set); for example, use bounded sets staying a positive distance from its complement and enlarge them slightly. This is a [Fréchet space](../../../topological-vector-space.md#frechet-space).

The [compactly supported distribution space](../../../distribution-theory.md#compactly-supported-distribution-space) is the [continuous dual space](../../../continuous-dual-space.md) $\mathcal E'(X)$. We use its [weak-star topology](../../../weak-topology.md#weak-star-topology): $u_j\to u$ precisely when $\langle u_j,f\rangle\to\langle u,f\rangle$ for every $f\in\mathcal E(X)$. A stronger standard choice is the [strong dual topology](../../../continuous-dual-space.md#strong-dual-topology), which requires uniform convergence on bounded subsets of $\mathcal E(X)$; specifying the weak convention avoids conflating these definitions.

A continuous linear functional necessarily takes null sequences to zero. Conversely, suppose a linear functional $u$ fails to be continuous. For each $j$, it is unbounded on $\{f:p_j(f)\leq1\}$; otherwise scaling would give a continuity estimate. We can therefore choose $f_j$ with

$$
p_j(f_j)\leq\frac1j,\qquad |u(f_j)|\geq1.
$$

For each fixed $l$, $p_l(f_j)\leq p_j(f_j)\to0$ once $j\geq l$. This contradicts the assumed null-sequence property. Hence **sequential continuity characterizes the continuous dual**:

$$
\boxed{u\in\mathcal E'(X)\iff f_j\to0\text{ in }\mathcal E(X)\Longrightarrow u(f_j)\to0.}
$$

This is the [sequential continuity criterion in a metrizable vector space](../../../topological-vector-space.md#sequential-continuity-criterion-in-a-metrizable-vector-space) applied to a linear functional.

Continuity also yields one compact $K\Subset X$, an integer $m$ and a constant $C$ such that $|u(f)|\leq Cp_{K,m}(f)$. Thus $u$ has [compact support](../../../function.md#compact-support) in $K$ and finite [order of a distribution](../../../distribution-theory.md#order-of-a-distribution). Conversely, a [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution) extends to $\mathcal E(X)$ by $u(f)=u(\eta f)$, where a [cutoff function](../../../distribution-theory.md#cutoff-function) $\eta$ equals one near its [support of a distribution](../../../distribution-theory.md#support-of-a-distribution). The local finite-order estimate makes this extension continuous and independent of $\eta$. This identifies the dual definition with compactly supported [distributions](../../../distribution-theory.md#distribution-mathematical-analysis).

Here is an explicit [compact continuous-derivative representation of a distribution](../../../distribution-theory.md#compact-continuous-derivative-representation-of-a-distribution). Extend $u$ by zero to $\mathbb R^n$ using a [cutoff function](../../../distribution-theory.md#cutoff-function) inside $X$, retaining finite order $m$. Put $r=m+2$ and

$$
E(x)=\prod_{j=1}^n\frac{(x_j)_+^{r-1}}{(r-1)!},\qquad\gamma=(r,\ldots,r).
$$

This locally $C^m$ function satisfies $\partial^\gamma E=\delta_0$. Indeed, each one-dimensional factor has $r$th [distributional derivative](../../../distribution-theory.md#distributional-derivative) equal to the [Dirac delta distribution](../../../distribution-theory.md#dirac-delta-function). The [convolution](../../../fourier-analysis.md#convolution) $F=u*E$ is continuous: the finite-order estimate extends $u$ to $C^m$ functions near its [compact support](../../../function.md#compact-support), and translated $E$ varies continuously in their $C^m$ norms. Equivalently, mollify $E$ and use the estimate to obtain local uniform convergence of the convolved functions. Distributional differentiation gives $\partial^\gamma F=u$.

Choose $\chi\in C_c^\infty(X)$ equal to one near $\operatorname{supp}u$. Since $\chi u=u$, repeated [Leibniz rule](../../../calculus.md#leibniz-rule) gives

$$
u=\chi\partial^\gamma F=\sum_{\beta\leq\gamma}(-1)^{|\beta|}\binom\gamma\beta\partial^{\gamma-\beta}\big((\partial^\beta\chi)F\big).
$$

Every coefficient function on the right is continuous and compactly supported in $X$. Thus **the required representation is finite**:

$$
\boxed{u=\sum_\alpha\partial^\alpha f_\alpha,\qquad f_\alpha\in C_c(X).}
$$

The equality first holds on [test functions](../../../distribution-theory.md#test-function) and then on all [smooth functions](../../../analysis.md#smooth-function) after inserting a common cutoff, so it holds in $\mathcal E'(X)$.

**A general [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) need not admit one finite such sum**, even if [compact support](../../../function.md#compact-support) is not required of the [continuous functions](../../../calculus.md#continuous-function). On $X=\mathbb R$, consider

$$
v=\sum_{j=1}^\infty\delta_j^{(j)}.
$$

The sum is locally finite, so it defines a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis). If it were a finite sum $\sum_{l=0}^M\partial^l g_l$ with all $g_l$ continuous, then on every fixed compact set its action would be bounded by test [derivatives](../../../calculus.md#derivative) through order $M$. Near an integer $j>M$, however, it is exactly $\delta_j^{(j)}$, whose order is $j$. To see the contradiction directly, choose a [test function](../../../distribution-theory.md#test-function) $\psi$ with $\psi^{(j)}(0)\ne0$ and put $\psi_\varepsilon(x)=\varepsilon^j\psi((x-j)/\varepsilon)$. All [derivative](../../../calculus.md#derivative) norms through order $M$ tend to zero, while $\langle\delta_j^{(j)},\psi_\varepsilon\rangle=(-1)^j\psi^{(j)}(0)$. This is a [distribution of unbounded order](../../../distribution-theory.md#distribution-of-unbounded-order). In dimensions $n>1$, the same example uses point masses at $(j,0,\ldots,0)$ and [derivatives](../../../calculus.md#derivative) in the first coordinate.

## 2

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

We place the definitions and the unheaded preliminary requests here before addressing the first labelled property. The [Schwartz space](../../../fourier-analysis.md#schwartz-space) consists of [smooth functions](../../../analysis.md#smooth-function) with finite [seminorms](../../../topological-vector-space.md#seminorm)

$$
q_{\alpha,\beta}(f)=\sup_{x\in\mathbb R^n}|x^\alpha\partial^\beta f(x)|
$$

for every pair of [multi-indices](../../../distribution-theory.md#multi-index-notation). Convergence means convergence in each [seminorm](../../../topological-vector-space.md#seminorm). The [tempered distribution](../../../fourier-analysis.md#tempered-distribution) space $\mathcal S'(\mathbb R^n)$ is its [continuous dual space](../../../continuous-dual-space.md), with weak convergence tested against every [Schwartz function](../../../fourier-analysis.md#schwartz-function). A continuous functional satisfies a bound by finitely many of these [seminorms](../../../topological-vector-space.md#seminorm), equivalently by one sufficiently large weighted [derivative](../../../calculus.md#derivative) [seminorm](../../../topological-vector-space.md#seminorm).

Use the [Fourier transform](../../../analysis.md#fourier-transform) convention

$$
\widehat f(\xi)=\int e^{-ix\cdot\xi}f(x)\,dx,\qquad f(x)=\frac1{(2\pi)^n}\int e^{ix\cdot\xi}\widehat f(\xi)\,d\xi.
$$

Differentiation under the integral and [integration by parts](../../../calculus.md#integration-by-parts) express $\xi^\alpha\partial_\xi^\beta\widehat f$ as a constant of modulus one times the [Fourier transform](../../../analysis.md#fourier-transform) of $\partial_x^\alpha(x^\beta f)$. Its supremum is bounded by the $L^1$ norm of that function. For $s>n$, this norm is at most a constant times finitely many Schwartz [seminorms](../../../topological-vector-space.md#seminorm), using the integrable weight $(1+|x|)^{-s}$. Thus $\mathcal F:\mathcal S\to\mathcal S$ is continuous.

For completeness, [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) follows by inserting $e^{-\varepsilon|\xi|^2}$ in the inverse integral and using [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem). The result is [convolution](../../../fourier-analysis.md#convolution) with the [Gaussian approximate identity](../../../diffusion-equation.md#gaussian-approximate-identity)

$$
(4\pi\varepsilon)^{-n/2}e^{-|x|^2/(4\varepsilon)}.
$$

It tends to $f$, while integrability of $\widehat f$ allows the damping factor to be removed by [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem). Consequently $\mathcal F^2f=(2\pi)^nf(-\cdot)$. Reflection preserves every Schwartz [seminorm](../../../topological-vector-space.md#seminorm), so the inverse transform is continuous as well. This proves **the [Fourier transform isomorphism of the Schwartz space](../../../analysis.md#fourier-transform-isomorphism-of-the-schwartz-space)**.

Define the [Fourier transform of a tempered distribution](../../../fourier-analysis.md#fourier-transform-of-a-tempered-distribution) by transposition,

$$
\langle\widehat u,\psi\rangle=\langle u,\widehat\psi\rangle.
$$

The Schwartz-space continuity just proved makes this a [tempered distribution](../../../fourier-analysis.md#tempered-distribution). Its inverse is $(2\pi)^{-n}\mathcal R\mathcal F$, where $\langle\mathcal Ru,\psi\rangle=\langle u,\psi(-\cdot)\rangle$. These maps are continuous for weak convergence, since each pairing is a pairing with a fixed transformed test. They are also continuous for the [strong dual topology](../../../continuous-dual-space.md#strong-dual-topology), because the Schwartz-space maps take bounded sets to bounded sets.

The [convolution of a tempered distribution with a Schwartz function](../../../fourier-analysis.md#convolution-of-a-tempered-distribution-with-a-schwartz-function) is

$$
(u*\varphi)(x)=\langle u_y,\varphi(x-y)\rangle.
$$

Smooth dependence of translated Schwartz functions gives $\partial^\alpha(u*\varphi)(x)=\langle u,\partial^\alpha\varphi(x-\cdot)\rangle$. The finite-[seminorm](../../../topological-vector-space.md#seminorm) estimate and $1+|y|\leq(1+|x|)(1+|x-y|)$ show that each [derivative](../../../calculus.md#derivative) has at most [polynomial growth](../../../analysis.md#polynomial-growth). In particular, $u*\varphi$ is a [smooth function](../../../analysis.md#smooth-function) defining a [tempered distribution](../../../fourier-analysis.md#tempered-distribution). It need not itself be a [Schwartz function](../../../fourier-analysis.md#schwartz-function); for example $1*\varphi=\int\varphi$.

Writing $\check\varphi(y)=\varphi(-y)$, its distributional pairing is $\langle u*\varphi,\psi\rangle=\langle u,\check\varphi*\psi\rangle$. The inner [convolution](../../../fourier-analysis.md#convolution) is a [Schwartz function](../../../fourier-analysis.md#schwartz-function), and this identity follows by integration in the Schwartz topology, justified by the weighted [seminorm](../../../topological-vector-space.md#seminorm) estimates. A direct [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) calculation gives $\check\varphi*\widehat\psi=\mathcal F(\widehat\varphi\psi)$. Hence

$$
\langle\widehat{u*\varphi},\psi\rangle=\langle u,\mathcal F(\widehat\varphi\psi)\rangle=\langle\widehat u,\widehat\varphi\psi\rangle,
\qquad\boxed{\widehat{u*\varphi}=\widehat u\,\widehat\varphi.}
$$

Multiplication is well defined because multiplication by $\widehat\varphi$ acts continuously on $\mathcal S$.

Now write the [Hilbert transform](../../../analysis.md#hilbert-transform) as [convolution](../../../fourier-analysis.md#convolution) with $K=\pi^{-1}\operatorname{pv}(1/x)$, the [principal-value reciprocal distribution](../../../distribution-theory.md#principal-value-reciprocal-distribution). The given [Heaviside function](../../../analysis.md#heaviside-step-function) transform, together with $\mathcal F^2H=2\pi H(-\cdot)$, yields

$$
\pi-i\mathcal F\big(\operatorname{pv}(1/x)\big)=2\pi H(-\xi),\qquad\widehat K(\xi)=-i\operatorname{sgn}\xi.
$$

The value of the sign function at zero is irrelevant to its regular [distribution](../../../distribution-theory.md#distribution-mathematical-analysis). Thus the [Hilbert-transform Fourier multiplier](../../../analysis.md#hilbert-transform-fourier-multiplier) is

$$
\widehat{\mathcal H\varphi}(\xi)=-i\operatorname{sgn}(\xi)\widehat\varphi(\xi).
$$

Applying [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem), whose normalization here is $\|f\|_2^2=(2\pi)^{-1}\|\widehat f\|_2^2$, proves **the isometry**:

$$
\boxed{\|\mathcal H\varphi\|_{L^2}=\|\varphi\|_{L^2}.}
$$

The principal-value integral agrees with this [convolution](../../../fourier-analysis.md#convolution): near its singular point subtract $\varphi(x)$, and use odd cancellation; at infinity the Schwartz decay gives convergence. The [Hilbert transform](../../../analysis.md#hilbert-transform) has domain $\mathcal S$, but generally does not take values in $\mathcal S$, as the tail in part (c) demonstrates.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Hilbert-transform Fourier multiplier](../../../analysis.md#hilbert-transform-fourier-multiplier) is bounded, and $\xi^r\widehat\varphi(\xi)$ is integrable for every nonnegative integer $r$. Therefore its inverse [Fourier transform](../../../analysis.md#fourier-transform) can be differentiated under the integral arbitrarily many times:

$$
\partial_x^r\mathcal H\varphi(x)=\frac1{2\pi}\int e^{ix\xi}(i\xi)^r[-i\operatorname{sgn}(\xi)]\widehat\varphi(\xi)\,d\xi.
$$

These [derivatives](../../../calculus.md#derivative) are continuous by [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem). Since $\widehat{\varphi^{(r)}}=(i\xi)^r\widehat\varphi$, **the Hilbert transform is smooth and commutes with differentiation**:

$$
\boxed{\mathcal H\varphi\in C^\infty(\mathbb R),\qquad (\mathcal H\varphi)'=\mathcal H(\varphi').}
$$

The Fourier proof avoids differentiating a singular kernel without preserving its [Cauchy principal value](../../../complex-analysis.md#cauchy-principal-value) prescription.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $f=\widehat\varphi$, a [Schwartz function](../../../fourier-analysis.md#schwartz-function). Splitting the inverse [Fourier transform](../../../analysis.md#fourier-transform) at the jump in the [Hilbert-transform Fourier multiplier](../../../analysis.md#hilbert-transform-fourier-multiplier) gives

$$
\mathcal H\varphi(x)=-\frac i{2\pi}\left[\int_0^\infty e^{ix\xi}f(\xi)\,d\xi-\int_{-\infty}^0e^{ix\xi}f(\xi)\,d\xi\right].
$$

For $x\ne0$, [integration by parts](../../../calculus.md#integration-by-parts) on each half-line shows

$$
\mathcal H\varphi(x)=\frac{f(0)}{\pi x}+\frac1{2\pi x}\left[\int_0^\infty e^{ix\xi}f'(\xi)\,d\xi-\int_{-\infty}^0e^{ix\xi}f'(\xi)\,d\xi\right].
$$

Both restricted [derivatives](../../../calculus.md#derivative) are in $L^1$. The [Riemann-Lebesgue lemma](../../../fourier-analysis.md#riemann-lebesgue-lemma) makes the bracket tend to zero as $|x|\to\infty$. Hence **the two-sided tail is**

$$
\boxed{\mathcal H\varphi(x)=\frac{\widehat\varphi(0)}{\pi x}+o(|x|^{-1}),\qquad |x|\to\infty.}
$$

Here $\widehat\varphi(0)=\int\varphi$. The [large-distance tail of the Hilbert transform](../../../analysis.md#large-distance-tail-of-the-hilbert-transform) thus depends on the zeroth moment of the input. If that moment is nonzero, the $1/x$ tail proves that the output is not a [Schwartz function](../../../fourier-analysis.md#schwartz-function), despite being smooth and square-integrable.

## 3

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

A [phase function](../../../distribution-theory.md#phase-function) is a real $C^\infty$ function on $X\times(\mathbb R^k\setminus\{0\})$, positively homogeneous of degree one in its frequency variable,

$$
\Phi(x,t\theta)=t\Phi(x,\theta)\quad(t>0),
$$

with nonvanishing total differential $d_{x,\theta}\Phi$. Vanishing of its frequency gradient alone is allowed; those critical directions are relevant to singularities.

With $\langle\theta\rangle=(1+|\theta|^2)^{1/2}$, the [symbol class](../../../distribution-theory.md#symbol-class) $\operatorname{Sym}(X;\mathbb R^k;N)=S^N_{1,0}$ consists of [smooth functions](../../../analysis.md#smooth-function) $a$ such that, for every $K\Subset X$ and every pair of [multi-indices](../../../distribution-theory.md#multi-index-notation),

$$
|\partial_x^\alpha\partial_\theta^\beta a(x,\theta)|\leq C_{K,\alpha,\beta}\langle\theta\rangle^{N-|\beta|},\qquad x\in K.
$$

There is no requirement that the constant be uniform in the [derivative](../../../calculus.md#derivative) indices. We use $D=(1/i)\partial$; the factors of $i$ do not affect these estimates.

For $b=D_x^\alpha D_\theta^\beta a$, any further [derivative](../../../calculus.md#derivative) satisfies

$$
|\partial_x^\mu\partial_\theta^\nu b|=|\partial_x^{\mu+\alpha}\partial_\theta^{\nu+\beta}a|\leq C\langle\theta\rangle^{N-|\beta|-|\nu|}.
$$

Thus **frequency [derivatives](../../../calculus.md#derivative) lower symbol order and spatial [derivatives](../../../calculus.md#derivative) preserve it**:

$$
\boxed{D_x^\alpha D_\theta^\beta a\in\operatorname{Sym}(X;\mathbb R^k;N-|\beta|).}
$$

This is the differentiation rule in [symbol calculus](../../../distribution-theory.md#symbol-calculus).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The [Leibniz rule](../../../calculus.md#leibniz-rule) expands each [derivative](../../../calculus.md#derivative) of a product into finitely many terms:

$$
\partial_x^\alpha\partial_\theta^\beta(a_1a_2)=\sum_{\mu\leq\alpha,\nu\leq\beta}\binom\alpha\mu\binom\beta\nu(\partial_x^\mu\partial_\theta^\nu a_1)(\partial_x^{\alpha-\mu}\partial_\theta^{\beta-\nu}a_2).
$$

The [symbol class](../../../distribution-theory.md#symbol-class) estimates bound every summand by a constant times $\langle\theta\rangle^{N_1-|\nu|+N_2-|\beta-\nu|}=\langle\theta\rangle^{N_1+N_2-|\beta|}$. Hence **symbol orders add under multiplication**:

$$
\boxed{a_1a_2\in\operatorname{Sym}(X;\mathbb R^k;N_1+N_2).}
$$

We now address the remaining unheaded requests. To define the [oscillatory integral](../../../distribution-theory.md#oscillatory-integral) as a functional on the [space of test functions](../../../distribution-theory.md#space-of-test-functions), choose $\eta\in C_c^\infty(\mathbb R^k)$ equal to one near zero and set

$$
\langle I_\Phi(a),f\rangle=\lim_{R\to\infty}\iint e^{i\Phi(x,\theta)}a(x,\theta)f(x)\eta(\theta/R)\,d\theta\,dx.
$$

The limit is not an assertion of absolute convergence of the original frequency integral. Split off a bounded-frequency part, which is smooth in $x$. At large frequency define

$$
q=|\nabla_x\Phi|^2+|\theta|^2|\nabla_\theta\Phi|^2,\qquad
L=\frac1{iq}\left(\nabla_x\Phi\cdot\nabla_x+|\theta|^2\nabla_\theta\Phi\cdot\nabla_\theta\right).
$$

Homogeneity and nonvanishing of the total phase differential imply $q\geq c_K|\theta|^2$ on each compact spatial set. Also $Le^{i\Phi}=e^{i\Phi}$. The spatial coefficients of $L$ have symbol order $-1$, and its frequency coefficients have order zero; consequently its [formal transpose of a differential operator](../../../analysis.md#formal-transpose-of-a-differential-operator) $L^t$ lowers symbol order by one. After $r>N+k$ integrations by parts, the high-frequency pairing has an absolutely integrable amplitude $(L^t)^r[(1-\chi(\theta))a(x,\theta)f(x)]$, where $\chi$ is a fixed cutoff near zero. [Derivatives](../../../calculus.md#derivative) of the outer cutoff yield errors bounded by $CR^{N+k-r}$ times finitely many [derivatives](../../../calculus.md#derivative) of $f$, so they tend to zero. This proves [cutoff independence of an oscillatory integral](../../../distribution-theory.md#cutoff-independence-of-an-oscillatory-integral) and defines a linear map into $\mathbb C$. Its distributional continuity is permitted as an assumption, and is also visible from this finite-[derivative](../../../calculus.md#derivative) estimate.

The [singular support](../../../distribution-theory.md#singular-support) of a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) is the complement of the largest open subset on which it equals a smooth [regular distribution](../../../distribution-theory.md#regular-distribution). The [stationary-direction bound for singular support](../../../distribution-theory.md#stationary-direction-bound-for-singular-support) needs [conic support of an oscillatory amplitude](../../../distribution-theory.md#conic-support-of-an-oscillatory-amplitude). Write

$$
C_a=\overline{\{(x,\theta/|\theta|):(x,\theta)\in\operatorname{supp}a,\ \theta\ne0\}}\subset X\times S^{k-1}.
$$

Its radial lift is the closed conic enlargement of the ordinary support. **The generally valid bound is**

$$
\boxed{\operatorname{sing\,supp}I_\Phi(a)\subset\{x:\exists\omega\in S^{k-1},\ (x,\omega)\in C_a,\ \nabla_\theta\Phi(x,\omega)=0\}.}
$$

If the amplitude support is conic, this is exactly the printed bound. It is also the standard interpretation when support in the frequency directions is understood conically.

To prove the bound, take a point outside its right-hand side. Closedness of $C_a$ and compactness of the sphere give a neighborhood $U$ and $c>0$ with $|\nabla_\theta\Phi|\geq c$ on the amplitude's directions over $U$. On a slightly larger directional neighborhood use

$$
L_\theta=\frac{\nabla_\theta\Phi\cdot\nabla_\theta}{i|\nabla_\theta\Phi|^2},\qquad L_\theta e^{i\Phi}=e^{i\Phi}.
$$

The [formal transpose of a differential operator](../../../analysis.md#formal-transpose-of-a-differential-operator) $L_\theta^t$ lowers symbol order by one, using frequency [derivatives](../../../calculus.md#derivative) only. An $x$ [derivative](../../../calculus.md#derivative) of order $l$ of the oscillatory integrand has symbol order at most $N+l$. Choosing more than $N+l+k$ integrations by parts makes that [derivative](../../../calculus.md#derivative) absolutely integrable, uniformly on smaller compact subsets of $U$. This works for every $l$, so $I_\Phi(a)$ is smooth on $U$.

The [ordinary amplitude support can miss a singular-support limit](../../../distribution-theory.md#ordinary-amplitude-support-can-miss-a-singular-support-limit) phenomenon requires a qualification here: **with unrestricted ordinary support the printed inclusion is false.** An explicit counterexample uses $X=\mathbb R^2$, $x=(s,t)$, one frequency variable and $\Phi(s,t,\theta)=s\theta$. Choose $t_j=1/j$, $w_j=1/(10j^2)$ and $\chi\in C_c^\infty((-1/4,1/4))$ with $\chi(0)=1$. Its translates $\chi_j(t)=\chi((t-t_j)/w_j)$ have disjoint supports. Choose an even [smooth function](../../../analysis.md#smooth-function) $\rho$ that is zero for $|\theta|\leq1$ and one for $|\theta|\geq2$, and put

$$
a(s,t,\theta)=\sum_{j\geq1}e^{-j^2}\chi_j(t)\rho(\theta/2^j).
$$

This is a symbol of order zero. All spatial [derivative](../../../calculus.md#derivative) bounds follow from $\sum_j e^{-j^2}w_j^{-l}<\infty$; frequency [derivatives](../../../calculus.md#derivative) have the required decay because the $j$th cutoff [derivative](../../../calculus.md#derivative) is supported where $|\theta|\asymp2^j$. Near every point $(s,0,\theta)$ with finite $\theta$, all large-$j$ terms vanish through the frequency cutoff and all remaining terms vanish in a small $t$ neighborhood. Thus no point $(0,0,\theta)$ lies in its ordinary support.

Nevertheless its oscillatory integral is

$$
I_\Phi(a)=2\pi B(t)\delta_0(s)-G(s,t),\qquad B(t)=\sum_j e^{-j^2}\chi_j(t),
$$

where $G$ is smooth. Indeed, its $j$th term is the ordinary Fourier integral of $1-\rho(\theta/2^j)$ times $e^{-j^2}\chi_j(t)$; [derivatives](../../../calculus.md#derivative) of order $l$ in $s$ and $m$ in $t$ are bounded by a constant times $e^{-j^2}2^{j(l+1)}w_j^{-m}$, a summable sequence. Since $B(t_j)\ne0$, each $(0,t_j)$ is singular. Closedness of [singular support](../../../distribution-theory.md#singular-support) forces $(0,0)$ to be singular too, although the literal ordinary-support right-hand side omits it. The closed conic support includes this limiting point and resolves the defect.

Finally use [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) distributionally. The constant amplitude gives $(2\pi)^{-n}\int e^{ix\cdot\theta}d\theta=\delta_0$, and differentiation of the exponential supplies a factor $i\theta$. Thus **the polynomial-amplitude integral is a delta [derivative](../../../calculus.md#derivative)**:

$$
\boxed{\frac1{(2\pi)^n}\int\theta^\alpha e^{ix\cdot\theta}\,d\theta=i^{-|\alpha|}\partial^\alpha\delta_0=D^\alpha\delta_0.}
$$

Its action on a [test function](../../../distribution-theory.md#test-function) $f$ is $i^{|\alpha|}\partial^\alpha f(0)$, confirming both the sign and the normalization. This is the [delta derivatives from polynomial oscillatory amplitudes](../../../distribution-theory.md#delta-derivatives-from-polynomial-oscillatory-amplitudes) identity.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
