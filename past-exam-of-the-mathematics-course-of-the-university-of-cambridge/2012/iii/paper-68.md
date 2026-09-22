# Paper 68

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_68.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_68.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use $D_j=-i\partial_{x_j}$ and $\langle\xi\rangle=(1+|\xi|^2)^{1/2}$, so the [Fourier transform](../../../analysis.md#fourier-transform) of $P(D)u$ is $P(\xi)\widehat u(\xi)$. Write $P_N$ for the homogeneous degree-$N$ part. An [elliptic differential operator](../../../distribution-theory.md#elliptic-differential-operator) has $P_N(\xi)\ne0$ for every real $\xi\ne0$. By [continuity](../../../calculus.md#continuous-function) on the [unit sphere](../../../topology.md#unit-sphere), $m=\min_{|\omega|=1}|P_N(\omega)|>0$. The lower-degree terms are bounded by $C|\xi|^{N-1}$ for $|\xi|\geq1$, whence

$$
|P(\xi)|\geq m|\xi|^N-C|\xi|^{N-1}\geq\frac m2|\xi|^N\geq c\langle\xi\rangle^N
$$

for sufficiently large $|\xi|$. This proves the [high-frequency lower bound for an elliptic polynomial](../../../distribution-theory.md#high-frequency-lower-bound-for-an-elliptic-polynomial). Degree zero just means a nonzero constant and has no [derivative](../../../calculus.md#derivative) gain.

With the Fourier convention in Question 3, the [Sobolev space](../../../sobolev-space.md) is

$$
\boxed{H^s(\mathbb R^n)=\{u\in\mathcal S':\langle\xi\rangle^s\widehat u\in L^2\},\qquad\|u\|_{H^s}^2=(2\pi)^{-n}\int\langle\xi\rangle^{2s}|\widehat u(\xi)|^2d\xi.}
$$

The condition includes that the weighted transform is represented by an $L^2$ function. For open $X$, the [Local Sobolev space](../../../sobolev-space.md#local-sobolev-space) consists of $u\in\mathcal D'(X)$ for which $\chi u$, extended by zero, belongs to $H^s(\mathbb R^n)$ for every $\chi\in C_c^\infty(X)$. We use the elementary [Sobolev multiplication by a smooth cutoff](../../../sobolev-space.md#sobolev-multiplication-by-a-smooth-cutoff) fact for every real $s$. It follows from Fourier [convolution](../../../fourier-analysis.md#convolution) with the rapidly decreasing $\widehat\chi$, the weighted inequality $\langle\xi\rangle^s\lesssim\langle\xi-\eta\rangle^{|s|}\langle\eta\rangle^s$, and the $L^1*L^2\to L^2$ [convolution](../../../fourier-analysis.md#convolution) bound.

For a [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution), [continuity](../../../calculus.md#continuous-function) on [test functions](../../../distribution-theory.md#test-function) supported in a fixed compact neighborhood gives finite order: for some integer $M$,

$$
|\langle u,\varphi\rangle|\leq C\max_{|\alpha|\leq M}\sup_K|\partial^\alpha\varphi|.
$$

Insert a compact smooth [cutoff function](../../../distribution-theory.md#cutoff-function) equal to one near the support, times $e^{-ix\cdot\xi}$. The resulting [Fourier transform](../../../analysis.md#fourier-transform) is smooth and satisfies $|\widehat u(\xi)|\leq C'\langle\xi\rangle^M$. The [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) is also tempered by this same finite-order bound. Thus

$$
\boxed{u\in H^t(\mathbb R^n)\quad\text{whenever }t<-M-n/2.}
$$

Indeed the square of the weighted bound is integrable exactly when $2(t+M)<-n$. This is [negative Sobolev regularity of a compactly supported distribution](../../../distribution-theory.md#negative-sobolev-regularity-of-a-compactly-supported-distribution).

We next prove local regularity by a [high-frequency reciprocal parametrix kernel](../../../distribution-theory.md#high-frequency-reciprocal-parametrix-kernel), including its off-diagonal smoothing property. Choose $\psi\in C_c^\infty(\mathbb R^n)$ equal to one on a ball containing all real zeros of $P$, and put $b(\xi)=(1-\psi(\xi))/P(\xi)$, defining it smoothly as zero in the inner ball. Differentiation of the reciprocal and the elliptic lower bound give

$$
|\partial_\xi^\alpha b(\xi)|\leq C_\alpha\langle\xi\rangle^{-N-|\alpha|}.
$$

The [Fourier multiplier](../../../analysis.md#fourier-multiplier) $E=b(D)$ maps $H^s$ to $H^{s+N}$ by its zeroth-order bound, and

$$
EP(D)=P(D)E=1-R,\qquad R=\psi(D).
$$

The kernel $K=\mathcal F^{-1}b$ is smooth away from the origin: for $x\ne0$, repeatedly integrate by parts using $e^{ix\cdot\xi}=(i|x|^2)^{-1}x\cdot\partial_\xi e^{ix\cdot\xi}$. After sufficiently many integrations, the differentiated symbol is integrable. For any desired $x$ [derivative](../../../calculus.md#derivative), repeat the argument with the additional [polynomial](../../../polynomial.md) $\xi^\beta$. A large-radius [cutoff function](../../../distribution-theory.md#cutoff-function) justifies each step and its removal uniformly on compact sets away from zero. Thus [convolution](../../../fourier-analysis.md#convolution) by $K$ carries a [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution) to a smooth function at points separated from its support. Also $R$ carries a [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution) to a [Schwartz function](../../../fourier-analysis.md#schwartz-function), because $\psi\widehat u$ is smooth with compact support.

For a target compact set in $X$, choose $\chi\in C_c^\infty(X)$ equal to one on a neighborhood of it. Then $\chi u$ and $[P(D),\chi]u$ have compact support, and the commutator is supported where [derivatives](../../../calculus.md#derivative) of $\chi$ occur, away from the target. The [parametrix](../../../distribution-theory.md#parametrix) identity gives

$$
\chi u=E[\chi P(D)u]+E[[P(D),\chi]u]+R(\chi u).
$$

The first term is in $H^{s+N}$ since $\chi P(D)u\in H^s$. The other two terms are smooth near the target by the proved kernel property. Since the target was arbitrary,

$$
\boxed{P(D)u\in H^s_{\mathrm{loc}}(X)\Longrightarrow u\in H^{s+N}_{\mathrm{loc}}(X).}
$$

This proof does not discard the [cutoff function](../../../distribution-theory.md#cutoff-function) commutator; it places its support away from the set where regularity is sought.

For the final [polynomial](../../../polynomial.md), select a multi-index $\alpha_0$ with $|\alpha_0|=N$ and $\partial^{\alpha_0}Q$ a nonzero constant. The derivative-ratio hypothesis immediately gives $|Q(\xi)|\geq c|\xi|^{\delta N}$ at large frequency. In particular $Q$ has no real zero there. For $N>0$, its degree bound also forces $\delta\leq1$. Differentiating $1/Q$ gives products of ratios $\partial^\beta Q/Q$, whose total [derivative](../../../calculus.md#derivative) order is $|\alpha|$. Hence the corresponding high-frequency reciprocal satisfies

$$
|\partial_\xi^\alpha b_Q(\xi)|\leq C_\alpha\langle\xi\rangle^{-\delta N-\delta|\alpha|}.
$$

Its multiplier maps $H^s$ to $H^{s+\delta N}$. Its kernel is still smooth off zero: each frequency [integration by parts](../../../calculus.md#integration-by-parts) now lowers the order by $\delta$, so more iterations may be needed, but $\delta>0$ supplies arbitrarily much decay. The same separated-support commutator identity applies without a change. The [derivative-ratio Sobolev gain for a polynomial operator](../../../distribution-theory.md#derivative-ratio-sobolev-gain-for-a-polynomial-operator) is therefore

$$
\boxed{Q(D)u\in H^s_{\mathrm{loc}}(X)\Longrightarrow u\in H^{s+\delta N}_{\mathrm{loc}}(X).}
$$

Simply estimating the commutator by its differential order would lose this sharper gain; the off-diagonal kernel argument uses the full derivative-ratio hypothesis.

## 2

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [symbol class](../../../distribution-theory.md#symbol-class) $\mathrm{Sym}(X,\mathbb R^k;N)$ consists of smooth amplitudes with estimates

$$
\boxed{|\partial_x^\alpha\partial_\theta^\beta a(x,\theta)|\leq C_{K,\alpha,\beta}\langle\theta\rangle^{N-|\beta|},\qquad x\in K\Subset X.}
$$

There is no loss of symbol order under an $x$ [derivative](../../../calculus.md#derivative). A [phase function](../../../distribution-theory.md#phase-function) is real and smooth for $\theta\ne0$, positively homogeneous of degree one in $\theta$, with its full differential $(d_x\Phi,d_\theta\Phi)$ nowhere zero there, at least on the amplitude's conic support. Homogeneous phases need not be smooth at $\theta=0$; that bounded-frequency region is handled separately or the amplitude is cut off near it.

Choose $\rho\in C_c^\infty(\mathbb R^k)$ equal to one near zero. The [oscillatory integral](../../../distribution-theory.md#oscillatory-integral) is defined by regularization in [distributions](../../../distribution-theory.md#distribution-mathematical-analysis):

$$
\boxed{\langle I_\Phi(a),f\rangle=\lim_{\varepsilon\downarrow0}\int_X\int e^{i\Phi(x,\theta)}a(x,\theta)\rho(\varepsilon\theta)f(x)\,d\theta\,dx,\qquad f\in C_c^\infty(X).}
$$

This is an ordinary integral when decay makes it absolutely convergent. For general order, the definition is independent of the regularizer. To see the mechanism, at large $|\theta|$ set

$$
A=|d_x\Phi|^2+|\theta|^2|d_\theta\Phi|^2,\qquad L=\frac{d_x\Phi\cdot\partial_x+|\theta|^2d_\theta\Phi\cdot\partial_\theta}{iA}.
$$

Homogeneity and the nonvanishing full differential give $A\gtrsim|\theta|^2$ on compact $x$ sets, and $Le^{i\Phi}=e^{i\Phi}$. Its $x$-derivative coefficients have order $-1$ and its $\theta$-derivative coefficients order zero, so each formal transpose $L^t$ lowers the amplitude order by one. Iterating more than $N+k$ times makes the test-function pairing integrable, and the same estimates control regularizer [derivatives](../../../calculus.md#derivative). This justifies the [cutoff function](../../../distribution-theory.md#cutoff-function) limit and its independence. A fixed bounded-frequency integral is smooth in $x$.

The [singular support](../../../distribution-theory.md#singular-support) of a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) is the complement of the largest [open set](../../../topology.md#open-set) on which it is represented by a smooth function. For the support-sensitive bound one must use [conic support of an oscillatory amplitude](../../../distribution-theory.md#conic-support-of-an-oscillatory-amplitude): a closed set of limiting high-frequency directions, locally in the base variable. One sufficient precise choice is

$$
C_a=\bigcap_{R>0}\overline{\{(x,\theta/|\theta|):(x,\theta)\in\operatorname{supp}_{X\times\mathbb R^k}a,\ |\theta|\geq R\}}\subset X\times S^{k-1},
$$

with closure taken in this product. If $x_0$ is outside the projection of $C_a\cap\{d_\theta\Phi=0\}$, compactness of the [unit sphere](../../../topology.md#unit-sphere) gives a neighborhood of $x_0$ and a positive uniform lower bound on $|d_\theta\Phi|$ wherever the large-frequency amplitude is supported. On that region use

$$
L_\theta=\frac{d_\theta\Phi\cdot\partial_\theta}{i|d_\theta\Phi|^2},\qquad L_\theta e^{i\Phi}=e^{i\Phi}.
$$

Its coefficients have order zero and its transpose lowers order by one. To prove $C^j$ regularity, first differentiate $j$ times in $x$, raising the amplitude order by at most $j$, and then integrate by parts more than $N+j+k$ times. The resulting integrals and their [derivatives](../../../calculus.md#derivative) converge uniformly on compact neighborhoods. Since $j$ is arbitrary, the [stationary-direction bound for singular support](../../../distribution-theory.md#stationary-direction-bound-for-singular-support) follows:

$$
\boxed{\operatorname{sing\,supp}I_\Phi(a)\subset\pi_X\bigl(C_a\cap\{d_\theta\Phi=0\}\bigr).}
$$

This is the standard conic interpretation of the support restriction in the question; directions at infinity, rather than finite-frequency stationary points, determine possible singularities.

**If $\operatorname{supp}a(x,\cdot)$ literally means the support of the restricted function, the printed inclusion can fail.** There is a [slice-support obstruction for oscillatory singularities](../../../distribution-theory.md#slice-support-obstruction-for-oscillatory-singularities). In one dimension, take $\Phi=x\theta$ and $a=x\eta(\theta)/|\theta|$, where $\eta$ is smooth and even, zero for $|\theta|\leq1$, and one for $|\theta|\geq2$. This is a symbol of order $-1$, and the full phase differential is nonzero for $\theta\ne0$. Its regularized integral near $x=0$ is

$$
I(x)=2x\int_0^\infty\eta(\theta)\frac{\cos(x\theta)}\theta\,d\theta=-2x\log|x|+\text{a smooth function}.
$$

Indeed substitute $u=|x|\theta$ in the tail, split at $u=1$, and write $\cos u=1+(\cos u-1)$ below one. The first term gives $-\log|x|$, while the remainder has an even convergent power series in $x$ plus a constant; the bounded-frequency correction is smooth. Thus $0$ is in the [singular support](../../../distribution-theory.md#singular-support), but $a(0,\cdot)=0$ has empty slice support. The joint closed conic support retains this limiting base point and makes the proved theorem valid. No nonstationarity conclusion is inferred just from the amplitude vanishing at one base point.

For the [wave equation](../../../wave-equation.md), Fourier transformation in $x$ reduces the initial-value problem to $\partial_t^2\widehat E+c^2|\xi|^2\widehat E=0$, with $\widehat E(\xi,0)=0$ and $\partial_t\widehat E(\xi,0)=1$. For $c>0$ its solution is

$$
\boxed{\widehat E(\xi,t)=\frac{\sin(ct|\xi|)}{c|\xi|},}
$$

with value $t$ at zero. Choose $\chi\in C_c^\infty(\mathbb R^n)$ equal to one near zero. The [low-frequency decomposition of the wave propagator](../../../wave-equation.md#low-frequency-decomposition-of-the-wave-propagator) is

$$
E(x,t)=E_{\mathrm{low}}(x,t)+I_{\Phi_+}(a_+)(x,t)+I_{\Phi_-}(a_-)(x,t),
$$

where

$$
E_{\mathrm{low}}=(2\pi)^{-n}\int e^{ix\cdot\xi}\chi(\xi)\frac{\sin(ct|\xi|)}{c|\xi|}\,d\xi,\quad\Phi_\pm=x\cdot\xi\pm ct|\xi|,\quad a_\pm=\pm\frac{(2\pi)^{-n}(1-\chi(\xi))}{2ic|\xi|}.
$$

The low-frequency term is an ordinary smooth function: the sine quotient extends smoothly in $\xi$ at zero and all [derivatives](../../../calculus.md#derivative) are integrable on the fixed compact frequency set. The high-frequency amplitudes belong to $\mathrm{Sym}(\mathbb R^{n+1},\mathbb R^n;-1)$, vanish near zero, and the phases have nonzero full differential since $d_x\Phi_\pm=\xi\ne0$. Their stationary-direction equations are $x\pm ct\xi/|\xi|=0$. Such a direction can occur only if $|x|=c|t|$. The smooth low-frequency term contributes no [singular support](../../../distribution-theory.md#singular-support), so

$$
\boxed{\operatorname{sing\,supp}E\subset\{(x,t):|x|=c|t|\}.}
$$

This is a statement about [singular support](../../../distribution-theory.md#singular-support): some dimensions have a smooth nonzero tail inside the cone, so it does not claim that the [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) is concentrated only on the cone.

## 3

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [Schwartz function](../../../fourier-analysis.md#schwartz-function) is a smooth function for which every [seminorm](../../../topological-vector-space.md#seminorm)

$$
p_{\alpha\beta}(\varphi)=\sup_{x\in\mathbb R^n}|x^\alpha\partial^\beta\varphi(x)|
$$

is finite. These [seminorms](../../../topological-vector-space.md#seminorm) define the Fréchet topology of the [Schwartz space](../../../fourier-analysis.md#schwartz-space) $\mathcal S(\mathbb R^n)$. The [tempered distributions](../../../fourier-analysis.md#tempered-distribution) form its continuous linear dual $\mathcal S'$. We use bilinear [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) pairing, with no complex conjugation on the [test function](../../../distribution-theory.md#test-function).

Differentiation under the Fourier integral and [integration by parts](../../../calculus.md#integration-by-parts) give

$$
\partial_\xi^\beta\widehat\varphi=\mathcal F[(-ix)^\beta\varphi],\qquad\xi^\alpha\widehat f=\mathcal F[D^\alpha f],\quad D=-i\partial.
$$

Therefore each [Schwartz seminorm](../../../fourier-analysis.md#schwartz-seminorm) of $\widehat\varphi$ is bounded by a finite sum of $L^1$ norms of polynomially weighted [derivatives](../../../calculus.md#derivative) of $\varphi$. Insert the integrable weight $\langle x\rangle^{-n-1}$ to bound those norms by finitely many [Schwartz seminorms](../../../fourier-analysis.md#schwartz-seminorm). This proves that $\mathcal F:\mathcal S\to\mathcal S$ is continuous.

To justify inversion without a merely formal exchange of integrals, insert $e^{-\varepsilon|\xi|^2/2}$ in the inverse integral. The Gaussian Fourier integral gives

$$
(2\pi)^{-n}\int e^{ix\cdot\xi}e^{-\varepsilon|\xi|^2/2}\widehat\varphi(\xi)d\xi=(\varphi*g_\varepsilon)(x),\qquad g_\varepsilon(x)=(2\pi\varepsilon)^{-n/2}e^{-|x|^2/(2\varepsilon)}.
$$

The normalized Gaussian is an approximate identity, so the right side tends to $\varphi(x)$; the left side converges by [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) since $\widehat\varphi$ is integrable. It follows that

$$
\boxed{\varphi(x)=(2\pi)^{-n}\int e^{ix\cdot\xi}\widehat\varphi(\xi)d\xi,\qquad\mathcal F^2\varphi=(2\pi)^n\varphi(-\cdot).}
$$

Reflection is continuous in [Schwartz seminorms](../../../fourier-analysis.md#schwartz-seminorm), so $\mathcal F^{-1}=(2\pi)^{-n}\mathcal R\mathcal F$ is continuous as well. This proves the [Fourier transform isomorphism of the Schwartz space](../../../analysis.md#fourier-transform-isomorphism-of-the-schwartz-space).

Define the [distributional Fourier transform](../../../fourier-analysis.md#fourier-transform-of-a-tempered-distribution) by

$$
\boxed{\langle\widehat u,\varphi\rangle=\langle u,\widehat\varphi\rangle.}
$$

It agrees with the ordinary integral transform whenever Fubini applies. Transposing the Schwartz inverse gives an inverse on $\mathcal S'$, and the same squared-transform identity holds. For the usual strong dual topology, a [seminorm](../../../topological-vector-space.md#seminorm) is $p_B(u)=\sup_{\varphi\in B}|\langle u,\varphi\rangle|$ for a bounded set $B\subset\mathcal S$. Since a continuous linear Schwartz map takes bounded sets to bounded sets, $p_B(\widehat u)=p_{\mathcal F B}(u)$ proves [continuity](../../../calculus.md#continuous-function), and similarly for the inverse. [Continuity](../../../calculus.md#continuous-function) also holds in the weak dual topology. Thus the transform is a continuous isomorphism on [tempered distributions](../../../fourier-analysis.md#tempered-distribution), with the stated normalization.

For a real symmetric [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) $G$, there is $c>0$ with $g(x)=x^TGx\geq c|x|^2$. The reciprocal is locally integrable in dimension three: the radial factor near zero is $r^2r^{-2}dr$. At infinity, rapid decay of a Schwartz [test function](../../../distribution-theory.md#test-function) makes it integrable. More quantitatively,

$$
\left|\int\frac{\varphi(x)}{g(x)}dx\right|\leq C\sup_x\langle x\rangle^2|\varphi(x)|\int_{\mathbb R^3}\frac{dx}{|x|^2\langle x\rangle^2}<\infty.
$$

This single [seminorm](../../../topological-vector-space.md#seminorm) bound proves a [tempered distribution](../../../fourier-analysis.md#tempered-distribution). No principal-value extension is needed at the origin.

First calculate the isotropic transform. For $f_\varepsilon(x)=e^{-\varepsilon|x|}/|x|^2$ and $k=|\xi|>0$, spherical integration and the supplied sine-integral identity give

$$
\widehat f_\varepsilon(\xi)=\frac{4\pi}{k}\int_0^\infty e^{-\varepsilon r}\frac{\sin(kr)}rdr=\frac{4\pi}{k}\arctan\frac k\varepsilon.
$$

The original functions converge in $\mathcal S'$ to $|x|^{-2}$ by [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) against tests. The transforms are bounded by $2\pi^2/|\xi|$, which is locally integrable in three dimensions and integrable against [Schwartz functions](../../../fourier-analysis.md#schwartz-function) at infinity. Hence

$$
\boxed{\mathcal F(|x|^{-2})(\xi)=\frac{2\pi^2}{|\xi|}\quad\text{as a regular tempered distribution}.}
$$

Let $y=G^{1/2}x$. The Jacobian is $(\det G)^{-1/2}$ and the dual vector is $G^{-1/2}\xi$. The [Fourier transform of a reciprocal positive quadratic form](../../../distribution-theory.md#fourier-transform-of-a-reciprocal-positive-quadratic-form) is consequently

$$
\boxed{\widehat{(1/g)}(\xi)=\frac{2\pi^2}{\sqrt{\det G}\sqrt{\xi^TG^{-1}\xi}}.}
$$

The frequency-origin value is understood distributionally; there is no additional delta term.

For the complex extension use a symmetric [matrix](../../../vector-space.md#matrix) $A=G+iB$ with real symmetric $B$ and positive real part $G$. Symmetry is natural for a [quadratic form](../../../linear-algebra.md#quadratic-form); a skew-symmetric part contributes nothing. The bound $|x^TAx|\geq x^TGx$ again gives a regular tempered reciprocal. Both sides of the prospective formula depend holomorphically on the [matrix](../../../vector-space.md#matrix) while its real part is positive: compact parameter sets give a common $|x|^{-2}$ bound for pairing and differentiated integrands. Continue from the real positive [matrices](../../../vector-space.md#matrix) along $A_z=G+izB$. In a complex neighborhood of $z=0$, imaginary $z$ gives real positive [matrices](../../../vector-space.md#matrix), so the one-variable identity theorem supplies the equality; connected continuation along $0\leq z\leq1$ reaches $A$.

The [analytic determinant square root for accretive symmetric matrices](../../../vector-space.md#analytic-determinant-square-root-for-accretive-symmetric-matrices) must follow that continuation, rather than an arbitrary scalar principal root of $\det A$. Explicitly, put $C=G^{-1/2}BG^{-1/2}$ and let its real [eigenvalues](../../../linear-operator-theory.md#eigenvalue) be $b_j$. Then

$$
d(A)=\sqrt{\det G}\prod_{j=1}^3\sqrt{1+ib_j},
$$

where each factor has positive real part. This is the [determinant](../../../linear-algebra.md#determinant) square root normalized positively on real positive [matrices](../../../vector-space.md#matrix). Also

$$
\operatorname{Re}(\xi^TA^{-1}\xi)=\xi^TG^{-1/2}(1+C^2)^{-1}G^{-1/2}\xi>0\qquad(\xi\ne0).
$$

Thus the quadratic-form square root has the unambiguous branch with positive real part. The [accretive complex quadratic reciprocal Fourier transform](../../../distribution-theory.md#accretive-complex-quadratic-reciprocal-fourier-transform) is

$$
\boxed{\mathcal F\!\left(\frac1{x^TAx}\right)(\xi)=\frac{2\pi^2}{d(A)\sqrt{\xi^TA^{-1}\xi}}.}
$$

Uniform local integrability of the right side justifies its [analytic continuation](../../../complex-analysis.md#analytic-continuation) as a [tempered distribution](../../../fourier-analysis.md#tempered-distribution), not merely pointwise away from the origin.

For the particular form,

$$
A=\begin{pmatrix}1&i&0\\i&1&0\\0&0&2\end{pmatrix},\qquad\det A=4,\qquad d(A)=2,\qquad A^{-1}=\frac12\begin{pmatrix}1&-i&0\\-i&1&0\\0&0&1\end{pmatrix}.
$$

Substitution gives the required normalized expression

$$
\boxed{\mathcal F\!\left(\frac1{x_1^2+x_2^2+2x_3^2+2ix_1x_2}\right)(\xi)=\frac{\sqrt2\pi^2}{\sqrt{\xi_1^2+\xi_2^2+\xi_3^2-2i\xi_1\xi_2}}.}
$$

For every nonzero real $\xi$, the radicand has positive real part, so the specified square root exists uniquely. Both sides are regular [tempered distributions](../../../fourier-analysis.md#tempered-distribution), despite their locally integrable singularities at zero.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
