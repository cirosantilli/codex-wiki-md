# Paper 340

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_340.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_340.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 340](paper-340.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat f(\xi)=\int_{\mathbb R}f(x)e^{-ix\xi}\,dx$. An [orthonormal](../../../linear-algebra.md#orthonormal-set) [multiresolution analysis](../../../fourier-analysis.md#multiresolution-analysis) is a family of closed [vector subspaces](../../../vector-space.md#vector-subspace) $V_j\subset L^2(\mathbb R)$, indexed by [integers](../../../number-theory.md#integer), with $V_j\subset V_{j+1}$, $\overline{\bigcup_jV_j}=L^2(\mathbb R)$, and $\bigcap_jV_j=\{0\}$. Its dilation condition is $f\in V_j$ if and only if $f(2\mathord\cdot)\in V_{j+1}$. The space $V_0$ is invariant under [integer](../../../number-theory.md#integer) [function translations](../../../function.md#translation-of-a-function) and admits a [scaling function](../../../fourier-analysis.md#scaling-function) $\varphi$ whose [integer](../../../number-theory.md#integer) [function translations](../../../function.md#translation-of-a-function) form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis). Consequently $\varphi_{j,k}=2^{j/2}\varphi(2^j\mathord\cdot-k)$ form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $V_j$.

Since $\varphi\in V_1$, expansion in that [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) gives the [scaling refinement equation](../../../fourier-analysis.md#scaling-refinement-equation)

$$
\varphi(x)=\sqrt2\sum_{k\in\mathbb Z}h_k\varphi(2x-k),\qquad h_k=\langle\varphi,\varphi_{1,k}\rangle.
$$

The [series](../../../real-analysis.md#series-mathematics) converges in the [L2 norm](../../../real-analysis.md#l2-norm). The associated [low-pass filter of a multiresolution analysis](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis) is the periodic [Fourier series](../../../fourier-series.md) symbol

$$
\boxed{m(\xi)=\frac1{\sqrt2}\sum_{k\in\mathbb Z}h_ke^{-ik\xi},\qquad\widehat\varphi(2\xi)=m(\xi)\widehat\varphi(\xi).}
$$

Initially the symbol is defined almost everywhere. [Orthonormal](../../../linear-algebra.md#orthonormal-set) [integer](../../../number-theory.md#integer) [function translations](../../../function.md#translation-of-a-function) give the [quadrature mirror filter](../../../fourier-analysis.md#quadrature-mirror-filter) identity $|m(\xi)|^2+|m(\xi+\pi)|^2=1$ almost everywhere. For a [Lebesgue integrable](../../../measure-theory.md#lebesgue-integrable-function) [scaling function](../../../fourier-analysis.md#scaling-function), its [Fourier transform](../../../analysis.md#fourier-transform) is [continuous](../../../calculus.md#continuous-function) and $|\widehat\varphi(0)|=1$; choosing a constant phase makes $\widehat\varphi(0)=1$ and the [continuous](../../../calculus.md#continuous-function) representative near zero has $m(0)=1$. Different conventions absorb $\sqrt2$ into the refinement coefficients; the displayed convention fixes that ambiguity.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $W_j=V_{j+1}\ominus V_j$ denote the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) of $V_j$ inside $V_{j+1}$. The [Meyer-Mallat theorem](../../../fourier-analysis.md#meyer-mallat-theorem) constructs a [wavelet](../../../fourier-analysis.md#wavelet) whose [integer](../../../number-theory.md#integer) [function translations](../../../function.md#translation-of-a-function) form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $W_0$. Dilation then gives the [orthogonal](../../../linear-algebra.md#orthogonal-vectors) decomposition into [orthogonal complements](../../../hilbert-space.md#orthogonal-complement) $L^2(\mathbb R)=\bigoplus_{j\in\mathbb Z}W_j$, so its translates and dilates form an [orthonormal wavelet](../../../fourier-analysis.md#orthonormal-wavelet) basis.

Using the [MRA low-pass filter](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis), choose the high-pass symbol $n(\xi)=e^{-i\xi}\overline{m(\xi+\pi)}$. The [quadrature mirror filter](../../../fourier-analysis.md#quadrature-mirror-filter) identity makes the two analysis channels [orthonormal](../../../linear-algebra.md#orthonormal-set). The resulting [Fourier transform](../../../analysis.md#fourier-transform) formula is

$$
\boxed{\widehat\psi(2\xi)=e^{-i\xi}\overline{m(\xi+\pi)}\widehat\varphi(\xi).}
$$

Equivalently, with the refinement coefficients from the [scaling refinement equation](../../../fourier-analysis.md#scaling-refinement-equation), put $g_k=(-1)^{k-1}\overline{h_{1-k}}$ and $\psi(x)=\sqrt2\sum_kg_k\varphi(2x-k)$. This index choice gives precisely the displayed high-pass symbol. Changing all $g_k$ by one constant unit phase gives the same [orthonormal wavelet](../../../fourier-analysis.md#orthonormal-wavelet) construction. In particular the often-used $(-1)^k\overline{h_{1-k}}$ convention differs only by a global minus sign. The basis is $\psi_{j,k}(x)=2^{j/2}\psi(2^jx-k)$ for $j,k\in\mathbb Z$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

A [wavelet](../../../fourier-analysis.md#wavelet) with $p$ [vanishing moments](../../../fourier-analysis.md#vanishing-moment) satisfies $x^k\psi\in L^1$ and $\int x^k\psi(x)\,dx=0$ for $0\le k<p$. The [moment differentiation of the Fourier transform](../../../analysis.md#moment-differentiation-of-the-fourier-transform) theorem states that these weighted integrability hypotheses make $\widehat\psi\in C^{p-1}$, with $\widehat\psi^{(k)}(\xi)=\int(-ix)^k\psi(x)e^{-ix\xi}\,dx$. Hence $\widehat\psi^{(k)}(0)=0$. The [MRA projection Fourier identity](../../../fourier-analysis.md#mra-projection-fourier-identity), together with density of the approximation spaces and [continuity](../../../calculus.md#continuous-function) of $\widehat\varphi$ at zero, gives $|\widehat\varphi(0)|=1$. These are the two analytic theorems needed in addition to the [quadrature mirror filter](../../../fourier-analysis.md#quadrature-mirror-filter) construction.

For the ordinary [derivative](../../../calculus.md#derivative) conclusion, assume also that the [MRA low-pass filter](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis) is $C^{p-1}$ near $\pi$ and $\widehat\varphi$ is $C^{p-1}$ near zero. These hypotheses hold, for example, for a compactly supported [scaling function](../../../fourier-analysis.md#scaling-function) with a finite refinement filter. The [wavelet](../../../fourier-analysis.md#wavelet) identity gives

$$
\overline{m(\pi+t)}=\frac{e^{it}\widehat\psi(2t)}{\widehat\varphi(t)}.
$$

The denominator is nonzero near zero. Its reciprocal and the exponential are $C^{p-1}$, so the [product rule](../../../calculus.md#product-rule) and the zero [Taylor polynomial](../../../calculus.md#taylor-polynomial) of $\widehat\psi$ give the [smooth-mask vanishing-moment criterion](../../../fourier-analysis.md#smooth-mask-vanishing-moment-criterion)

$$
\boxed{m^{(k)}(\pi)=0\quad(0\le k<p),\quad\text{under the stated smoothness hypotheses}.}
$$

**The printed integrability hypothesis alone does not guarantee ordinary higher [derivatives](../../../calculus.md#derivative).** It gives only a [continuous](../../../calculus.md#continuous-function) $\widehat\varphi$. Without added smoothness, [Taylor theorem](../../../calculus.md#taylor-theorem) for $\widehat\psi$ still gives $m(\pi+t)=o(|t|^{p-1})$ for the representative defined by the quotient: a [Peano zero](../../../calculus.md#peano-zero). This establishes the value at $\pi$, and for $p\ge2$ the first [derivative](../../../calculus.md#derivative) there, but it does not automatically establish iterated [derivatives](../../../calculus.md#derivative).

Here is a [lacunary scaling-phase regularity counterexample](../../../fourier-analysis.md#lacunary-scaling-phase-regularity-counterexample) for $p\ge3$. Start with a compactly supported [Daubechies wavelet](../../../fourier-analysis.md#daubechies-wavelet) having $p$ [vanishing moments](../../../fourier-analysis.md#vanishing-moment), with [scaling function](../../../fourier-analysis.md#scaling-function) $\varphi_0$ and finite [MRA low-pass filter](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis) $m_0$. Define the periodic phase

$$
\theta(t)=\sum_{n\ge0}2^{-n}\sin(2^nt),\qquad a(t)=e^{i\theta(t)},\qquad\widehat\varphi(t)=a(t)\widehat\varphi_0(t).
$$

The [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) of $\theta$ are absolutely summable. The [Wiener algebra](../../../fourier-series.md#wiener-algebra) is closed under multiplication and the exponential [series](../../../real-analysis.md#series-mathematics), so $a$ and $a^{-1}$ have absolutely summable [Fourier coefficients](../../../fourier-series.md#fourier-coefficient). Thus $\varphi$ is an absolutely summable combination of [integer](../../../number-theory.md#integer) [function translations](../../../function.md#translation-of-a-function) of $\varphi_0$, belongs to $L^1\cap L^2$, and generates the same $V_0$. Unimodularity preserves [orthogonality](../../../linear-algebra.md#orthogonal-vectors) and unit [norm](../../../functional-analysis.md#norm) of its [integer](../../../number-theory.md#integer) [function translations](../../../function.md#translation-of-a-function); the inverse phase preserves their complete span. The same approximation spaces therefore give a [multiresolution analysis](../../../fourier-analysis.md#multiresolution-analysis).

The identity $\theta(2t)=\theta(t)+\theta(t+\pi)$ gives $a(2t)=a(t)a(t+\pi)$, so the [periodic phase change of a scaling function](../../../fourier-analysis.md#periodic-phase-change-of-a-scaling-function) produces $m(t)=a(t+\pi)m_0(t)$. In the high-pass formula the phases cancel:

$$
e^{-it}\overline{m(t+\pi)}\widehat\varphi(t)
=e^{-it}\overline{m_0(t+\pi)}\widehat\varphi_0(t).
$$

The associated [wavelet](../../../fourier-analysis.md#wavelet) is therefore exactly the original one, with unchanged [vanishing moments](../../../fourier-analysis.md#vanishing-moment).

At any dyadic point $t_0=2\pi k/2^j$, the [difference quotient](../../../calculus.md#difference-quotient) of the terms with $j\le n\le\log_2(1/|h|)$ is $1+O((2^nh)^2)$ per term. The sum of these errors and the remaining tail divided by $h$ are bounded; the finitely many earlier terms have finite limits. Hence $(\theta(t_0+h)-\theta(t_0))/h=\log_2(1/|h|)+O(1)$, which has no finite limit. The exponential has the same failure of [differentiability](../../../analysis.md#differentiability). Dyadic points are [dense](../../../topology.md#dense-set), and $m_0(\pi+t)$ is nonzero for sufficiently small $t\ne0$. Thus $m$ is not [differentiable](../../../analysis.md#differentiable-function) on any neighborhood of $\pi$, so an ordinary second [derivative](../../../calculus.md#derivative) at $\pi$, understood as the [derivative](../../../calculus.md#derivative) of a locally defined first [derivative](../../../calculus.md#derivative), need not exist. The [Peano zero](../../../calculus.md#peano-zero) remains valid. This separates the intended smooth-mask theorem from what the literal assumptions establish.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Under the smoothness hypotheses in the [smooth-mask vanishing-moment criterion](../../../fourier-analysis.md#smooth-mask-vanishing-moment-criterion), write any nonzero [integer](../../../number-theory.md#integer) $j$ as $j=2^r\ell$, where $r\ge0$ and $\ell$ is odd, possibly negative. Iterating the [scaling refinement equation](../../../fourier-analysis.md#scaling-refinement-equation) exactly $r+1$ times gives

$$
\widehat\varphi(2\pi j+t)=\left[\prod_{n=1}^{r+1}m\left(\frac{2\pi j+t}{2^n}\right)\right]\widehat\varphi\left(\frac{2\pi j+t}{2^{r+1}}\right).
$$

The last [MRA low-pass filter](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis) factor is $m(\pi\ell+t/2^{r+1})$. Its [derivatives](../../../calculus.md#derivative) of all orders less than $p$ vanish at $t=0$, because $\ell$ is odd and the [MRA low-pass filter](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis) is $2\pi$-periodic. If the remaining factors are $C^{p-1}$ at the displayed arguments, the [product rule](../../../calculus.md#product-rule) forces every [derivative](../../../calculus.md#derivative) of order less than $p$ of the product to vanish. In particular [compact support](../../../function.md#compact-support) and a finite [MRA low-pass filter](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis) supply all these hypotheses. Therefore the [integer-frequency zeros of a scaling function](../../../fourier-analysis.md#integer-frequency-zeros-of-a-scaling-function) are

$$
\boxed{\widehat\varphi^{(k)}(2\pi j)=0\quad(j\ne0,\ 0\le k<p),\quad\text{with the stated regularity}.}
$$

Under only the printed assumptions, the exact same finite refinement argument gives the [Peano zero](../../../calculus.md#peano-zero) $\widehat\varphi(2\pi j+t)=o(|t|^{p-1})$. Indeed, the last [MRA low-pass filter](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis) factor has that estimate, the other [MRA low-pass filter](../../../fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis) factors are bounded by one almost everywhere by the [quadrature mirror filter](../../../fourier-analysis.md#quadrature-mirror-filter) identity, and the last [Fourier transform](../../../analysis.md#fourier-transform) factor is bounded because $\varphi\in L^1$. The estimate initially holds almost everywhere and extends to every $t$ by [continuity](../../../calculus.md#continuous-function) of $\widehat\varphi$. It does not imply arbitrary ordinary higher [derivatives](../../../calculus.md#derivative). In the [lacunary scaling-phase regularity counterexample](../../../fourier-analysis.md#lacunary-scaling-phase-regularity-counterexample), $\widehat\varphi=a\widehat\varphi_0$ is nondifferentiable at [dense](../../../topology.md#dense-set) dyadic points next to the isolated integer-frequency zeros of the [smooth](../../../analysis.md#smooth-function) base transform. Thus the same regularity qualification is necessary here.

## 2

↑ **Parent:** [Paper 340](paper-340.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Fix the ordering of the [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) and write $c_m=\langle f,g_m\rangle$, taking indices from $1$. The [linear N-term approximation](../../../hilbert-space.md#linear-n-term-approximation) retains the first $N$ coefficients:

$$
\boxed{f_N^{\mathrm{lin}}=\sum_{m=1}^Nc_mg_m.}
$$

Its index set is independent of $f$, so the map is an [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) and is [linear](../../../vector-space.md#linearity).

For the [nonlinear N-term approximation](../../../hilbert-space.md#best-n-term-approximation), let $\Lambda_N(f)$ be any set of $N$ indices with greatest $|c_m|$, resolving ties arbitrarily and padding with zero coefficients if necessary. Since $(c_m)\in\ell^2$, such a selection exists. Then

$$
\boxed{f_N^{\mathrm{nonlin}}=\sum_{m\in\Lambda_N(f)}c_mg_m,\qquad\|f-f_N^{\mathrm{nonlin}}\|^2=\sum_{m\notin\Lambda_N(f)}|c_m|^2.}
$$

The [Parseval identity](../../../fourier-analysis.md#parseval-identity) shows that for any fixed index set the displayed coefficients minimize the [Hilbert space](../../../hilbert-space.md) error. Choosing the largest squared magnitudes minimizes the omitted sum over every set of at most $N$ indices. This is the [best N-term approximation](../../../hilbert-space.md#best-n-term-approximation); dependence of the selected indices on $f$ makes the operation nonlinear.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $0<\alpha\le1$, uniform Lipschitz-$\alpha$ means that one constant $M$ satisfies $|f(x)-f(y)|\le M|x-y|^\alpha$ for every $x,y\in[0,1]$. The resulting [Hölder space](../../../sobolev-space.md#holder-space) has [norm](../../../functional-analysis.md#norm)

$$
\|f\|_{C^{0,\alpha}}=\|f\|_\infty+[f]_{C^{0,\alpha}},\qquad[f]_{C^{0,\alpha}}=\sup_{x\ne y}\frac{|f(x)-f(y)|}{|x-y|^\alpha}.
$$

For the subsequent estimates at general $\alpha>0$, use the higher-order [Hölder class](../../../sobolev-space.md#holder-class) convention: write $\alpha=r+\beta$ with $r\ge0$ an [integer](../../../number-theory.md#integer) and $0<\beta\le1$, and require $f\in C^r([0,1])$ with $f^{(r)}$ uniformly Lipschitz-$\beta$. Thus

$$
\boxed{C^\alpha=C^{r,\beta},\qquad\|f\|_{C^\alpha}=\sum_{k=0}^r\|f^{(k)}\|_\infty+[f^{(r)}]_{C^{0,\beta}}.}
$$

At [integer](../../../number-theory.md#integer) $\alpha=k$, this uses $C^{k-1,1}$; the alternative classical $C^k$ convention is stronger on this [compact](../../../topology.md#compact-space) [closed interval](../../../real-analysis.md#closed-real-interval) and also suffices for the estimates.

**For exponents above one, a first-difference inequality alone forces the [function](../../../function.md) to be constant.** Partition $[x,y]$ into $n$ equal pieces and use the [triangle inequality](../../../topological-analysis.md#triangle-inequality): $|f(y)-f(x)|\le M|y-x|^\alpha n^{1-\alpha}\to0$. Consequently a nontrivial higher-order definition is needed for the full range of exponents in the later [wavelet](../../../fourier-analysis.md#wavelet) estimates. Equivalently, higher-order [Hölder class](../../../sobolev-space.md#holder-class) gives a local [Taylor polynomial](../../../calculus.md#taylor-polynomial) with remainder bounded by $C\|f\|_{C^\alpha}|x-x_0|^\alpha$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use localization and cancellation of the assumed [interval-adapted wavelet basis](../../../fourier-analysis.md#interval-adapted-wavelet-basis): at scale $j$, every detail [wavelet](../../../fourier-analysis.md#wavelet) has support diameter at most $B2^{-j}$, [L1 norm](../../../functional-analysis.md#l1-norm) at most $B'2^{-j/2}$, and annihilates [polynomials](../../../polynomial.md) of degree less than $q$. These bounds also apply to the modified [boundary wavelets](../../../fourier-analysis.md#boundary-wavelet); a restriction of an arbitrary whole-line [wavelet](../../../fourier-analysis.md#wavelet) without the cancellation-preserving boundary construction would not suffice. The finitely many coarse [scaling functions](../../../fourier-analysis.md#scaling-function) can be treated separately.

Write $\alpha=r+\beta$ with $0<\beta\le1$ as above. Because $\alpha<q$, we have $r<q$. Choose $x_0$ in the [support of a function](../../../function.md#support) of $\psi_{j,n}$, and let $T_{x_0}$ be the degree-$r$ [Taylor polynomial](../../../calculus.md#taylor-polynomial) of $f$. The [Hölder-Taylor remainder bound](../../../sobolev-space.md#holder-taylor-remainder-bound) gives

$$
|f(x)-T_{x_0}(x)|\le C_\alpha\|f\|_{C^\alpha}|x-x_0|^\alpha.
$$

For $r=0$ this is the [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) bound. For $r\ge1$, the [integral](../../../calculus.md#integral) [Taylor remainder](../../../calculus.md#taylor-remainder) is bounded using $f^{(r)}(t)-f^{(r)}(x_0)$, whose magnitude is at most $[f^{(r)}]_{C^{0,\beta}}|t-x_0|^\beta$.

The [vanishing moments](../../../fourier-analysis.md#vanishing-moment) remove $T_{x_0}$ from the [inner product](../../../linear-algebra.md#inner-product). Applying the remainder estimate and the [L1 norm](../../../functional-analysis.md#l1-norm) bound on the localized support yields the [wavelet coefficient decay for Hölder functions](../../../sobolev-space.md#wavelet-coefficient-decay-for-holder-functions)

$$
|\langle f,\psi_{j,n}\rangle|\le\sup_{\operatorname{supp}\psi_{j,n}}|f-T_{x_0}|\,\|\psi_{j,n}\|_1\le C_\alpha B^\alpha B'\|f\|_{C^\alpha}2^{-j\alpha}2^{-j/2}.
$$

Thus

$$
\boxed{|\langle f,\psi_{j,n}\rangle|\le C2^{-j(\alpha+1/2)}\|f\|_{C^\alpha}.}
$$

Here $C$ depends on the fixed [wavelet](../../../fourier-analysis.md#wavelet) family, the exponent and boundary construction, but not on $f,j,n$. The proof uses the assumed regularity and moments; it does not identify the minimal [Daubechies wavelet](../../../fourier-analysis.md#daubechies-wavelet) order with its [differentiability](../../../analysis.md#differentiability) order, which need not coincide.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $M$ bound the piecewise [Hölder norms](../../../sobolev-space.md#holder-norm), and let $B=\|f\|_\infty$. At scale $j$, classify a [wavelet](../../../fourier-analysis.md#wavelet) as bad when its localized [support of a function](../../../function.md#support) meets a discontinuity, and as good otherwise. [Compact support](../../../function.md#compact-support) and bounded overlap imply at most $C_0K$ bad [wavelets](../../../fourier-analysis.md#wavelet) per scale and at most $C_12^j$ total [wavelets](../../../fourier-analysis.md#wavelet). A good support lies in a single [smooth](../../../analysis.md#smooth-function) piece, so the preceding [wavelet coefficient decay for Hölder functions](../../../sobolev-space.md#wavelet-coefficient-decay-for-holder-functions) gives $|c_{j,n}|\le C M2^{-j(\alpha+1/2)}$. The permitted bounded-function estimate gives $|c_{j,n}|\le C B2^{-j/2}$ for bad coefficients.

Consider a specific [N-term approximation](../../../hilbert-space.md#n-term-approximation): retain all coarse [scaling functions](../../../fourier-analysis.md#scaling-function) and all [wavelets](../../../fourier-analysis.md#wavelet) through scale $J$, and also retain the bad coefficients at scales $J<j\le L$, where $L=\lceil2\alpha J\rceil$. Since $\alpha>1/2$, $L\ge J$ for large $J$. Its term count is bounded by

$$
N_J\le C_2 2^J+C_3K(L-J)+C_4=O(2^J+KJ).
$$

By the [Parseval identity](../../../fourier-analysis.md#parseval-identity), its squared [L2 norm](../../../real-analysis.md#l2-norm) error is the sum of omitted squared coefficients. The good tail satisfies

$$
\sum_{j>J}\sum_{n\ \mathrm{good}}|c_{j,n}|^2\le C M^2\sum_{j>J}2^j2^{-2j(\alpha+1/2)}\le C'M^22^{-2\alpha J},
$$

and the remaining bad tail satisfies

$$
\sum_{j>L}\sum_{n\ \mathrm{bad}}|c_{j,n}|^2\le C K B^2\sum_{j>L}2^{-j}\le C'KB^22^{-L}\le C'KB^22^{-2\alpha J}.
$$

Choose $J=\lfloor\log_2(N/(2C_2'))\rfloor$ with a fixed sufficiently large $C_2'$; then the $O(KJ)$ extra terms fit the remaining budget for all sufficiently large $N$, while $2^J$ is comparable to $N$. Padding to $N$ terms does not increase the error. The [best N-term approximation](../../../hilbert-space.md#best-n-term-approximation) is at least as accurate as this constructed selection, so

$$
\boxed{\epsilon_n(N,f)=\|f-f_N^{\mathrm{nonlin}}\|_2^2=O(N^{-2\alpha}).}
$$

The constant may depend on the finite number of jumps, the piecewise [Hölder norms](../../../sobolev-space.md#holder-norm), $B$ and the fixed [wavelet](../../../fourier-analysis.md#wavelet) family. Values exactly at the jumps are immaterial in $L^2$. The improvement comes from retaining only a bounded number of jump-crossing coefficients at each finer scale, as in [best N-term wavelet approximation of piecewise Hölder functions](../../../hilbert-space.md#best-n-term-wavelet-approximation-of-piecewise-holder-functions).

## 3

↑ **Parent:** [Paper 340](paper-340.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The strict [null space property](../../../numerical-analysis.md#nullspace-property) of order $s$ is

$$
\boxed{\|v_S\|_1<\|v_{S^c}\|_1\quad\text{for every }0\ne v\in\ker A\text{ and every }|S|\le s.}
$$

Here $v_S$ agrees with $v$ on $S$ and is zero elsewhere. Suppose a nonzero null [vector](../../../vector-space.md#vector) had at most $2s$ nonzero entries. Split its [support of a vector](../../../numerical-analysis.md#support-of-a-vector) into disjoint sets $S,T$ of size at most $s$. Applying the [null space property](../../../numerical-analysis.md#nullspace-property) to both sets would give $\|v_S\|_1<\|v_T\|_1$ and $\|v_T\|_1<\|v_S\|_1$, a contradiction. Empty parts cause the same contradiction. Thus no such nonzero null [vector](../../../vector-space.md#vector) exists.

For an $s$-sparse $x$, the feasible [vector](../../../vector-space.md#vector) $x$ has $\|x\|_0\le s$, where the zero-subscript quantity counts nonzero entries and is not a [norm](../../../functional-analysis.md#norm). Any feasible competitor $z$ with $\|z\|_0\le\|x\|_0$ also has at most $s$ nonzero entries. The difference $z-x\in\ker A$ has at most $2s$ nonzero entries, so $z=x$. Competitors with larger support have strictly larger objective. Therefore **every s-sparse [vector](../../../vector-space.md#vector) is the unique sparsest feasible [vector](../../../vector-space.md#vector)**. This is [sparse injectivity](../../../numerical-analysis.md#sparse-injectivity); for $s=0$ the only sparse [vector](../../../vector-space.md#vector) is zero and the conclusion is immediate.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

It is equivalent to minimize $\|z\|_q$ or its $q$th power $F_q(z)=\sum_i|z_i|^q$, because taking the $q$th root is strictly increasing. For $q<1$, this is an [Lq quasi-norm](../../../real-analysis.md#lq-quasi-norm), while $q=1$ gives the [L1 norm](../../../functional-analysis.md#l1-norm).

Assume the [Lq null space property](../../../numerical-analysis.md#lq-null-space-property) of order $s$. Let $x$ have [support of a vector](../../../numerical-analysis.md#support-of-a-vector) $S$ with $|S|\le s$, and let $z=x+v$ be any distinct feasible [vector](../../../vector-space.md#vector). Then $0\ne v\in\ker A$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) for complex magnitudes and the subadditivity $(a+b)^q\le a^q+b^q$ give

$$
|x_i|^q\le(|x_i+v_i|+|v_i|)^q\le|x_i+v_i|^q+|v_i|^q.
$$

For $q=1$ the same inequality follows directly from the [triangle inequality](../../../topological-analysis.md#triangle-inequality). Since $x=0$ off $S$,

$$
F_q(x+v)\ge F_q(x)-\sum_{i\in S}|v_i|^q+\sum_{i\notin S}|v_i|^q>F_q(x).
$$

Thus $x$ is the unique minimizer.

Conversely, suppose every $s$-sparse [vector](../../../vector-space.md#vector) is the unique minimizer for its measurements. Fix $0\ne v\in\ker A$ and any $S$ with $|S|\le s$. The [vectors](../../../vector-space.md#vector) $x=-v_S$ and $z=v_{S^c}$ are distinct and satisfy $Az=Ax$, since $Av=0$. Uniqueness for this $x$ therefore implies $F_q(x)<F_q(z)$, exactly the required strict inequality. Hence

$$
\boxed{\text{uniform unique }s\text{-sparse }\ell^q\text{ recovery}\ \Longleftrightarrow\ \sum_{i\in S}|v_i|^q<\sum_{i\notin S}|v_i|^q\quad(0\ne v\in\ker A,\ |S|\le s).}
$$

The quantifier is uniform over the entire sparse class. Recovery of one particular signed [vector](../../../vector-space.md#vector) alone would not imply this [null space property](../../../numerical-analysis.md#nullspace-property).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the [Lq null space property](../../../numerical-analysis.md#lq-null-space-property) established above. Fix $0\ne v\in\ker A$ and order its magnitudes $a_1\ge\cdots\ge a_N\ge0$. For a fixed exponent, the sum over the largest $s$ entries is the greatest sum over any [support of a vector](../../../numerical-analysis.md#support-of-a-vector) of size at most $s$, so it suffices to verify the property for this ordered support.

If $s\ge1$, put $t=a_s$. We have $t>0$: otherwise $v$ would have fewer than $s$ nonzero entries, and applying the [Lq null space property](../../../numerical-analysis.md#lq-null-space-property) to its support would assert a positive number is less than zero. For $0<p<q$, the exponent $p-q$ is negative. Thus

$$
\sum_{i=1}^sa_i^p\le t^{p-q}\sum_{i=1}^sa_i^q<t^{p-q}\sum_{i>s}a_i^q\le\sum_{i>s}a_i^p.
$$

The first inequality uses $a_i\ge t$ on the top part; the last uses $0<a_i\le t$ in the tail. Zero tail entries contribute zero without invoking a negative power of zero. Every other set of size at most $s$ has no larger top sum and no smaller complementary sum, so it too satisfies the strict $p$ inequality. The preceding equivalence proves

$$
\boxed{\text{uniform }s\text{-sparse recovery at }q\ \Longrightarrow\ \text{uniform }s\text{-sparse recovery at every }0<p<q.}
$$

This is [monotonicity of uniform sparse recovery in the exponent](../../../numerical-analysis.md#monotonicity-of-uniform-sparse-recovery-in-the-exponent). If $\ker A=\{0\}$ the feasible [vector](../../../vector-space.md#vector) is unique regardless of the objective; if $s=0$, only the zero [vector](../../../vector-space.md#vector) is relevant. These cases need no threshold argument.

## 4

↑ **Parent:** [Paper 340](paper-340.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For real $u\in L^1(\Omega)$, its [total variation seminorm on a domain](../../../inverse-problem.md#total-variation-seminorm-on-a-domain) is

$$
\boxed{|Du|(\Omega)=\sup\left\{\int_\Omega u\,\operatorname{div}\xi\,dx:\xi\in C_c^1(\Omega;\mathbb R^2),\ |\xi(x)|_2\le1\right\}.}
$$

The [vector fields](../../../calculus.md#vector-field) have [compact support](../../../function.md#compact-support) inside $\Omega$, so no boundary term is charged. Taking both $\xi$ and $-\xi$ makes this equivalent to a supremum of absolute pairings. When finite, the [distributional derivative](../../../distribution-theory.md#distributional-derivative) $Du$ is a finite vector-valued [Radon measure](../../../measure-theory.md#radon-measure), and the displayed supremum is its [total variation norm of a measure](../../../measure-theory.md#total-variation-norm-of-a-measure). For a [smooth](../../../analysis.md#smooth-function) [function](../../../function.md) it equals $\int_\Omega|\nabla u|_2\,dx$.

The [function of bounded variation on a domain](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain) belongs to the [Banach space](../../../banach-space.md)

$$
\boxed{BV(\Omega)=\{u\in L^1(\Omega):|Du|(\Omega)<\infty\},\qquad\|u\|_{BV}=\|u\|_{L^1}+|Du|(\Omega).}
$$

The [L1 norm](../../../functional-analysis.md#l1-norm) is needed because variation alone vanishes on constant [functions](../../../function.md) and is only a [seminorm](../../../topological-vector-space.md#seminorm). No smoothness of $u$ is part of this definition.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Take the [indicator function](../../../measure-theory.md#indicator-function) $u(x_1,x_2)=\chi_{\{x_1>1/2\}}$ inside $(0,1)^2$. For a compactly supported test [vector field](../../../calculus.md#vector-field), integration in $x_1$ and then $x_2$ gives

$$
\int_\Omega u\,\operatorname{div}\xi\,dx=-\int_0^1\xi_1(1/2,x_2)\,dx_2.
$$

The vertical [derivative](../../../calculus.md#derivative) term integrates to zero. The absolute pairing is at most one, and test [vector fields](../../../calculus.md#vector-field) with $\xi_1=-1$ along all but arbitrarily short endpoint pieces approach one. Thus $|Du|(\Omega)=1$. More explicitly, the [distributional derivative](../../../distribution-theory.md#distributional-derivative) is $Du=e_1\mathcal H^1\!\restriction\{(1/2,x_2):0<x_2<1\}$, where $\mathcal H^1$ is [Hausdorff measure](../../../measure-theory.md#hausdorff-measure) along the segment. Also $\|u\|_1=1/2$.

A [Sobolev space](../../../sobolev-space.md) [function](../../../function.md) in $W^{1,1}(\Omega)$ has each weak [derivative](../../../calculus.md#derivative) represented by an $L^1$ density with respect to planar [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). The nonzero segment measure here is singular with respect to that measure, so this requirement fails. Equivalently, the [Sobolev fundamental theorem of calculus on lines](../../../sobolev-space.md#sobolev-fundamental-theorem-of-calculus-on-lines) would require an absolutely [continuous](../../../calculus.md#continuous-function) representative on almost every horizontal slice, whereas each slice has a jump. Therefore

$$
\boxed{u\in BV(\Omega)\setminus W^{1,1}(\Omega),\qquad\|u\|_{BV}=\tfrac32.}
$$

This is the [bounded-variation step outside W11](../../../inverse-problem.md#bounded-variation-step-outside-w11) example.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Work in the real [Hilbert space](../../../hilbert-space.md) $L^2(\mathbb R^2)$, with $g\in L^2$ and $\alpha>0$. The penalty $J$ is a [proper convex function](../../../real-analysis.md#proper-convex-function): it is finite at zero, and the [bounded-variation space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain) domain is [convex](../../../real-analysis.md#convex-function). Its [subdifferential](../../../convex-optimization.md#subdifferential) at a finite-penalty $u$ consists of $q\in L^2$ satisfying $J(v)\ge J(u)+\langle q,v-u\rangle$ for every $v\in L^2$.

If $q=(g-u)/\alpha\in\partial J(u)$, expand the quadratic term and use the [subgradient inequality](../../../real-analysis.md#subgradient-inequality):

$$
\alpha J(v)+\tfrac12\|v-g\|_2^2-\alpha J(u)-\tfrac12\|u-g\|_2^2\ge\alpha\langle q,v-u\rangle+\langle u-g,v-u\rangle+\tfrac12\|v-u\|_2^2=\tfrac12\|v-u\|_2^2.
$$

Thus $u$ is the unique minimizer.

Conversely, let $u$ be a minimizer. Its penalty is finite since comparison with zero gives a finite objective. For any $v$ with $J(v)<\infty$, set $w_t=u+t(v-u)$, where $0<t\le1$. [Convexity](../../../real-analysis.md#convex-function) gives $J(w_t)-J(u)\le t(J(v)-J(u))$. Minimality and quadratic expansion then imply

$$
0\le\alpha\bigl(J(v)-J(u)\bigr)+\langle u-g,v-u\rangle+\tfrac t2\|v-u\|_2^2.
$$

Letting $t\downarrow0$ yields $J(v)\ge J(u)+\langle(g-u)/\alpha,v-u\rangle$. The inequality is automatic if $J(v)=\infty$. Hence

$$
\boxed{u\text{ minimizes }\alpha J+\tfrac12\|\mathord\cdot-g\|_2^2\ \Longleftrightarrow\ \frac{g-u}{\alpha}\in\partial J(u).}
$$

This also follows from the [subdifferential sum rule](../../../convex-optimization.md#subdifferential-sum-rule), since the quadratic term is everywhere [continuous](../../../calculus.md#continuous-function) and [differentiable](../../../analysis.md#differentiable-function), and the [subgradient optimality condition](../../../real-analysis.md#subgradient-optimality-condition). The direct proof above needs no unproved existence theorem.

**On the entire plane, the printed global BV domain is not closed in the L2 geometry.** The usual $BV(\mathbb R^2)$ definition includes an $L^1$ condition. For $1<a\le2$, $f(x)=(1+|x|)^{-a}$ belongs to $L^2$, has finite distributional variation $2\pi a\int_0^\infty r(1+r)^{-a-1}\,dr$, and fails to belong to $L^1$. The truncated $f_T=f\chi_{B(0,T)}$ lies in $BV\cap L^2$ and tends to $f$ in $L^2$. Its variation is the interior variation plus $2\pi T(1+T)^{-a}$, and tends to a finite limit. Thus $J(f_T)$ stays bounded but the literal $J(f)=\infty$, establishing [failure of L2 closure of the global BV domain](../../../inverse-problem.md#failure-of-l2-closure-of-the-global-bv-domain). One must not infer universal minimizer existence from an inapplicable closed-penalty [proximal operator](../../../convex-optimization.md#proximal-operator) theorem. The standard closed extension uses the [homogeneous bounded-variation space](../../../inverse-problem.md#homogeneous-bounded-variation-space), allowing finite distributional variation without global $L^1$. The optimality equivalence just proved is valid for the literal penalty whenever a minimizer exists; the next datum has an explicit certified minimizer in its domain.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let $B=B(0,R)$, with $R>0$. Its [indicator function](../../../measure-theory.md#indicator-function) has [L2 norm](../../../real-analysis.md#l2-norm) squared $\pi R^2$ and [total variation seminorm on a domain](../../../inverse-problem.md#total-variation-seminorm-on-a-domain) $2\pi R$. On the family $u=c\chi_B$, the objective is $2\pi\alpha R|c|+\tfrac12\pi R^2(c-1)^2$, whose minimizer is $c=(1-2\alpha/R)_+$. To prove global optimality, a [total variation calibration](../../../inverse-problem.md#total-variation-calibration) is needed.

Define the bounded radial [vector field](../../../calculus.md#vector-field)

$$
z(x)=\begin{cases}x/R,&|x|\le R,\\Rx/|x|^2,&|x|>R.\end{cases}
$$

It satisfies $|z|\le1$ and has a [continuous](../../../calculus.md#continuous-function) normal component across $\partial B$. Its [distributional divergence](../../../calculus.md#distributional-divergence) therefore has no boundary measure, and direct differentiation yields $q=\operatorname{div}z=(2/R)\chi_B\in L^2$. Although $z$ is not compactly supported, multiply it by a [smooth](../../../analysis.md#smooth-function) radial cutoff equal to one through radius $T$ and zero beyond $2T$. The extra divergence has magnitude $O(R/T^2)$ on an annulus of area $O(T^2)$, hence [L2 norm](../../../real-analysis.md#l2-norm) $O(R/T)$. Smoothing the [continuous](../../../calculus.md#continuous-function) piecewise field gives compactly supported [smooth](../../../analysis.md#smooth-function) admissible test [vector fields](../../../calculus.md#vector-field) with divergences tending to $q$ in $L^2$, preserving the bound $|z|\le1$. The dual definition therefore gives $\langle q,v\rangle\le J(v)$ for every finite-penalty $v$, and trivially for all other $v$.

Moreover $\langle q,\chi_B\rangle=(2/R)\pi R^2=2\pi R=J(\chi_B)$. By the [subgradient](../../../real-analysis.md#subgradient) characterization of an [absolutely one-homogeneous functional](../../../convex-optimization.md#absolutely-one-homogeneous-functional), $q\in\partial J(c\chi_B)$ for every $c>0$, and $q\in\partial J(0)$. If $0<\alpha<R/2$, choose $c=1-2\alpha/R$; then $(g-c\chi_B)/\alpha=q$. If $\alpha\ge R/2$, choose $u=0$; then $g/\alpha=(R/(2\alpha))q$ belongs to $\partial J(0)$, since multiplying the dual bound by a number in $[0,1]$ preserves it. The previous optimality criterion proves

$$
\boxed{u(x)=\left(1-\frac{2\alpha}{R}\right)_+\chi_{B(0,R)}(x).}
$$

The quadratic fidelity is [strictly convex](../../../real-analysis.md#strictly-convex-function), so this minimizer is unique, including the threshold $\alpha=R/2$. The disk retains its radius on the positive branch and disappears on the zero branch; this is [total variation denoising of a disk](../../../inverse-problem.md#total-variation-denoising-of-a-disk).

## 5

↑ **Parent:** [Paper 340](paper-340.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Write $D=\nabla$ and use the real pixelwise [inner products](../../../linear-algebra.md#inner-product). Let $D^*$ be the [adjoint operator](../../../hilbert-space.md#adjoint-operator), defined by $\langle Du,p\rangle=\langle u,D^*p\rangle$. For each nontrivial grid direction its one-dimensional formula is

$$
(D_x^{+*}p^1)_{i,j}=\begin{cases}-p^1_{1,j},&i=1,\\p^1_{i-1,j}-p^1_{i,j},&1<i<N,\\p^1_{N-1,j},&i=N,\end{cases}
$$

with the analogous formula in $j$ for $D_y^{+*}p^2$. Their sum is $D^*p$; unused components $p^1_{N,j}$ and $p^2_{i,N}$ do not contribute. For $N=1$, $D=D^*=0$. If discrete divergence is defined, its sign convention is $\operatorname{div}=-D^*$, as in the [adjoint of a discrete forward gradient](../../../finite-difference.md#adjoint-of-a-discrete-forward-gradient).

Define the [compact](../../../topology.md#compact-space) [convex set](../../../mathematical-optimization.md#convex-set) $P_\lambda=\{p\in X^2:|p_{i,j}|_2\le\lambda\}$ and its image $C=D^*P_\lambda$. The image is [compact](../../../topology.md#compact-space) and [convex](../../../real-analysis.md#convex-function), hence closed, and contains zero. The finite-dimensional Euclidean duality formula $\lambda|a|_2=\max_{|p|_2\le\lambda}a\cdot p$, applied independently at every pixel, gives

$$
\lambda\|Du\|_{2,1}=\max_{p\in P_\lambda}\langle Du,p\rangle=\max_{w\in C}\langle u,w\rangle=\sigma_C(u).
$$

Thus the penalty is the [support function](../../../mathematical-optimization.md#support-function) $\sigma_C$. Its [convex conjugate](../../../convex-optimization.md#convex-conjugate) is the [indicator functional of a constraint set](../../../inverse-problem.md#indicator-functional-of-a-constraint-set) $\iota_C$, equal to zero on $C$ and infinity elsewhere. For $w\in C$, the conjugate supremum is zero; for $w\notin C$, the separation theorem supplies a direction $u$ with $\langle u,w\rangle>\sigma_C(u)$, and scaling that direction makes the supremum infinite.

The [proximal operator](../../../convex-optimization.md#proximal-operator) is $\operatorname{prox}_{\sigma_C}(g)=\arg\min_u\{\sigma_C(u)+\tfrac12\|u-g\|_2^2\}$. It exists uniquely because the objective is [continuous](../../../calculus.md#continuous-function), coercive and [strictly convex](../../../real-analysis.md#strictly-convex-function). The [Moreau decomposition](../../../convex-optimization.md#moreau-decomposition) for a proper closed [convex function](../../../real-analysis.md#convex-function) gives $\operatorname{prox}_{\sigma_C}(g)+\operatorname{prox}_{\iota_C}(g)=g$. The second term is the [Euclidean projection onto a convex set](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set), so the [projection residual for discrete total variation](../../../inverse-problem.md#projection-residual-for-discrete-total-variation) is

$$
\boxed{u=g-P_Cg,\qquad C=D^*\{p:|p_{i,j}|_2\le\lambda\}.}
$$

Alternatively, the [variational characterization of convex projection](../../../mathematical-optimization.md#variational-characterization-of-convex-projection) says $w=P_Cg$ exactly when $\langle g-w,z-w\rangle\le0$ for every $z\in C$. Hence $w$ attains the [support function](../../../mathematical-optimization.md#support-function) at $u=g-w$, giving $w\in\partial\sigma_C(u)$ and the same optimality condition. This supplies a direct verification of the [Moreau decomposition](../../../convex-optimization.md#moreau-decomposition) step in this instance.

**The printed wording needs “the residual after a projection”, rather than “the projection itself”.** In general this denoising map is not a projection onto any fixed closed [convex set](../../../mathematical-optimization.md#convex-set). A [metric projection onto a closed convex set](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) is idempotent, while denoising a sufficiently large jump twice shrinks it twice. Concretely, for $N=2$ and data with rows $(0,0)$ and $(6\lambda,6\lambda)$, the minimizer has rows $(\lambda,\lambda)$ and $(5\lambda,5\lambda)$. Reapplying the map gives rows $(2\lambda,2\lambda)$ and $(4\lambda,4\lambda)$, so it is not idempotent. These formulas have a global certificate: take $p^1_{1,j}=\lambda$, all other dual entries zero, giving $D^*p$ with rows $(-\lambda,-\lambda)$ and $(\lambda,\lambda)$; it saturates every positive row difference and yields the primal optimality condition. The qualification is therefore not merely a consequence of a restricted two-level ansatz.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Computing $P_Cg$ is equivalent to minimizing $F(p)=\tfrac12\|g-D^*p\|_2^2$ over $P_\lambda$, since $D^*p$ ranges over precisely $C$. Differentiating with the [adjoint operator](../../../hilbert-space.md#adjoint-operator) gives $\nabla F(p)=D(D^*p-g)$, whose [Lipschitz constant](../../../real-analysis.md#lipschitz-constant) is $L=\|DD^*\|=\|D\|^2$. Starting with any $p^0\in P_\lambda$, for example zero, the [projected-gradient dual total variation algorithm](../../../inverse-problem.md#projected-gradient-dual-total-variation-algorithm) is

$$
\boxed{r^k=p^k+\tau D(g-D^*p^k),\qquad p^{k+1}_{i,j}=\frac{r^k_{i,j}}{\max(1,|r^k_{i,j}|_2/\lambda)},\qquad u^k=g-D^*p^k.}
$$

The block formula is the [Euclidean projection onto a convex set](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) $P_\lambda$, since it clips each two-dimensional block to a Euclidean ball of radius $\lambda$. Both components must be clipped together for the isotropic [block mixed norm](../../../functional-analysis.md#block-mixed-norm).

For the unscaled forward differences, $\|D_x^+u\|_2^2\le4\|u\|_2^2$ and likewise in the other direction, so $L\le8$. More exactly, for $N>1$ the one-dimensional path difference has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $4\sin^2(k\pi/(2N))$, $0\le k<N$, and the square-grid operator sums two such spectra. Thus $L=8\cos^2(\pi/(2N))$. Finite-dimensional [projected gradient descent](../../../convex-optimization.md#projected-gradient-descent) for a [convex](../../../real-analysis.md#convex-function) objective with an $L$-Lipschitz [gradient](../../../calculus.md#gradient) converges from every feasible starting point to a dual minimizer for fixed $0<\tau<2/L$. The theorem assumes a nonempty closed [convex set](../../../mathematical-optimization.md#convex-set), a [convex](../../../real-analysis.md#convex-function) [differentiable](../../../analysis.md#differentiable-function) objective with globally Lipschitz [gradient](../../../calculus.md#gradient), and a nonempty minimizer set. All hold here: $P_\lambda$ is [compact](../../../topology.md#compact-space) and [convex](../../../real-analysis.md#convex-function), and $F$ is a [continuous](../../../calculus.md#continuous-function) [convex](../../../real-analysis.md#convex-function) quadratic. Finite-dimensional convergence is of the full [sequence](../../../real-analysis.md#sequence), rather than only its objective values.

Consequently **any fixed step with $0<\tau<1/4$ is safe on this grid**; the more conservative $0<\tau\le1/8$ is also safe. The dual minimizer need not be unique because $D^*$ has a [null space](../../../linear-algebra.md#kernel-of-a-linear-map), but $D^*p^k\to P_Cg$ and $u^k\to u$ uniquely. For $N=1$, the [gradient](../../../calculus.md#gradient) penalty vanishes and $u=g$, so no positive-$L$ step restriction is needed.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

**[Absolute values](../../../real-analysis.md#absolute-value) are missing in the printed formula.** For signed real blocks, the intended [block mixed norm](../../../functional-analysis.md#block-mixed-norm) must be

$$
\|v\|_{q,1}=\sum_{i,j}\left(\sum_{r=1}^d|v^r_{i,j}|^q\right)^{1/q},\qquad q\ge1.
$$

Without them, at $q=1$ a block $(-1,1)$ has value zero although it is nonzero, and a negative [scalar](../../../vector-space.md#scalar) has negative value. For nonintegral $q$, a negative component may not even have a real power. The literal expression therefore is not a [norm](../../../functional-analysis.md#norm) and does not define the claimed general [convex](../../../real-analysis.md#convex-function) problem. Even [integer](../../../number-theory.md#integer) exponents do not fix all other $q$ in the stated range.

With the corrected [norm](../../../functional-analysis.md#norm), let $q'$ be the [Holder conjugate exponent](../../../functional-analysis.md#conjugate-exponents): $q'=q/(q-1)$ for $q>1$ and $q'=\infty$ for $q=1$. Blockwise [Holder inequality](../../../functional-analysis.md#holder-inequality), with equality from a norming block, gives

$$
\lambda\|Au\|_{q,1}=\sup_{p\in P_{\lambda,q'}}\langle Au,p\rangle,\qquad P_{\lambda,q'}=\{p\in X^d:\|p_{i,j}\|_{q'}\le\lambda\text{ for all }i,j\}.
$$

The [duality of block mixed norms](../../../functional-analysis.md#duality-of-block-mixed-norms) identifies the closed [compact](../../../topology.md#compact-space) [convex set](../../../mathematical-optimization.md#convex-set) and the projection residual from the [Moreau decomposition](../../../convex-optimization.md#moreau-decomposition)

$$
\boxed{C= A^*P_{\lambda,q'},\qquad u=g-P_Cg.}
$$

For $q=2$, the dual blocks are [Euclidean balls](../../../functional-analysis.md#euclidean-ball); for $q=1$, they are cubes given by componentwise bounds $|p^r_{i,j}|\le\lambda$. No injectivity or surjectivity of $A$ is required: [compactness](../../../topology.md#compact-space) of the block product makes its [linear](../../../vector-space.md#linearity) image [compact](../../../topology.md#compact-space), and the [strictly convex](../../../real-analysis.md#strictly-convex-function) fidelity still gives a unique primal minimizer. For general $q'$, the Euclidean projection onto a dual block ball is not generally obtained by radial scaling, so the special clipping formula from the isotropic case should not be reused without further analysis.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
