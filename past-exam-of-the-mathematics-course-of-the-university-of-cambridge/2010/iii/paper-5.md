# Paper 5

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper5.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper5.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)

## 1

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the bilinear pairing $T_g(f)=\int_{\mathbb R^n}fg$, so the map $g\mapsto T_g$ is complex linear. With the sesquilinear convention $\int f\overline g$ the representing map would instead be conjugate linear. For [conjugate exponents](../../../functional-analysis.md#conjugate-exponents) $p,q$, [Hölder's inequality](../../../real-analysis.md#holder-s-inequality) gives $|T_g(f)|\leq\|g\|_q\|f\|_p$. If $g\ne0$, take $v=|g|^{q-2}\overline g$, defined as zero where $g=0$. Then

$$
\int vg=\|g\|_q^q,\qquad \|v\|_p=\|g\|_q^{q/p},\qquad q-q/p=1.
$$

Consequently **$\|T_g\|=\|g\|_q$**. This also proves [injectivity](../../../algebra.md#injective-function) of the representation.

For [surjectivity](../../../algebra.md#surjective-function), let $\ell$ be a nonzero element of the [continuous dual space](../../../continuous-dual-space.md) of $L^p$ and choose $f_0$ with $\ell(f_0)=1$. Its kernel $K$ is a [closed linear subspace](../../../vector-space.md#closed-vector-subspace). Use the allowed best-approximation fact to choose $h\in K$ and put $z=f_0-h$. Thus $\ell(z)=1$ and

$$
\Phi(k):=\int |z|^{p-2}\overline z\,k=0\quad(k\in K),\qquad \Phi(z)=\|z\|_p^p>0.
$$

For each $f$, the vector $f-\ell(f)z$ belongs to $K$. Therefore $\Phi(f)=\ell(f)\|z\|_p^p$, giving

$$
\boxed{\ell(f)=\int fg,\qquad g=\frac{|z|^{p-2}\overline z}{\|z\|_p^p}\in L^q,\qquad \|\ell\|=\|g\|_q.}
$$

Membership follows from $(p-1)q=p$; the zero functional is represented by zero. This proves the isometric isomorphism $(L^p(\mathbb R^n))^*\cong L^q(\mathbb R^n)$ without using a representation theorem as a substitute for the proof. It is the [closed-hyperplane proof of Lp duality](../../../continuous-dual-space.md#closed-hyperplane-proof-of-lp-duality).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The relevant [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) says that for $1<p<\infty$ the closed bounded balls of $L^p(\mathbb R^n)$ are compact in the [weak topology](../../../weak-topology.md). In particular, every bounded sequence has a weakly convergent subsequence whose limit has [norm](../../../functional-analysis.md#norm) no larger than the common bound. Applying the preceding [duality of Lp spaces](../../../continuous-dual-space.md#duality-of-lp-spaces) also identifies this as weak-star compactness of $L^p=(L^q)^*$; its weak and weak-star test spaces are both $L^q$.

Here is a direct proof of both compactness and the subsequence assertion. Let $\|f_j\|_p\leq M$ and choose a countable dense set $\{g_m\}$ in the separable [Lp space](../../../measure-theory.md#lp-space) $L^q$. Each scalar sequence $\int f_jg_m$ is bounded. Successive subsequence selection followed by the [diagonal subsequence argument](../../../real-analysis.md#diagonal-subsequence-argument) gives $f_{j_k}$ for which these pairings converge for every $m$. For arbitrary $g\in L^q$,

$$
\left|\int(f_{j_k}-f_{j_l})g\right|\leq2M\|g-g_m\|_q+\left|\int(f_{j_k}-f_{j_l})g_m\right|.
$$

First approximate $g$ by $g_m$ and then take $k,l$ large. This proves convergence of every pairing, and the limit $\Lambda(g)=\lim_k\int f_{j_k}g$ is linear with $|\Lambda(g)|\leq M\|g\|_q$. Apply the already proved [duality of Lp spaces](../../../continuous-dual-space.md#duality-of-lp-spaces) with $q$ in place of $p$: $\Lambda(g)=\int fg$ for an $f\in L^p$ with $\|f\|_p\leq M$. Thus

$$
\boxed{f_{j_k}\rightharpoonup f\text{ in }L^p,\qquad \|f\|_p\leq M.}
$$

To obtain compactness rather than only a sequential statement, on the radius-$M$ ball define

$$
d(f,h)=\sum_{m=1}^{\infty}2^{-m}\frac{|\int(f-h)g_m|}{1+|\int(f-h)g_m|}.
$$

Density and [Hölder's inequality](../../../real-analysis.md#holder-s-inequality) show that this is a [metric space](../../../topological-analysis.md#metric-space) distance and that its topology is exactly the [weak topology](../../../weak-topology.md) on this ball: every remaining test pairing is uniformly approximated there by a dense-set pairing. The subsequence argument proves sequential compactness for this metric. A sequentially compact [metric space](../../../topological-analysis.md#metric-space) is compact: otherwise either an infinite separated sequence contradicts [total boundedness](../../../topological-analysis.md#totally-bounded-space) or a Cauchy sequence without a limit contradicts sequential compactness; completeness and [total boundedness](../../../topological-analysis.md#totally-bounded-space) give compactness by successive finite coverings. This completes the proof. The same argument is the [Sequential Banach-Alaoglu theorem for a separable predual](../../../functional-analysis.md#sequential-banach-alaoglu-theorem-for-a-separable-predual).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The assertion that fails is weak compactness of the $L^1$ unit ball; the abstract [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) for dual balls never fails. Consider the [concentration prevents weak compactness in L1](../../../weak-topology.md#concentration-prevents-weak-compactness-in-l1) example

$$
\boxed{f_j(x)=j^n\mathbf1_{[0,1/j]^n}(x),\qquad f_j\geq0,\qquad \|f_j\|_1=1.}
$$

Suppose a subsequence converged weakly in $L^1$ to $f$. For each $m$, all sufficiently late supports lie inside $B_{1/m}(0)$. Testing against every bounded measurable function supported outside that ball shows that $f=0$ almost everywhere there. Taking the countable union over $m$ proves $f=0$ almost everywhere on $\mathbb R^n$. But testing against the bounded constant function one gives $\int f=\lim_j\int f_j=1$, a contradiction.

The same argument applies to every subnet whose indices tend to infinity, so the sequence has no weak cluster point in the ball and the ball is not weakly compact. It converges against smooth compactly supported tests to a point mass, which is not an $L^1$ density. Thus **boundedness in $L^1$ does not imply the weak compactness proved in part (b)**; concentration is the obstruction.

## 2

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

One potential form of the [Hardy–Littlewood–Sobolev inequality](../../../nonlinear-analysis.md#hardy-littlewood-sobolev-inequality) is: if $0<\alpha<n$, $1<p<n/\alpha$, and $1/r=1/p-\alpha/n$, then

$$
\boxed{\left\|I_\alpha f\right\|_r\leq C_{n,p,\alpha}\|f\|_p,\qquad I_\alpha f(x)=\int_{\mathbb R^n}|x-y|^{\alpha-n}f(y)\,dy.}
$$

A normalization constant for the [Riesz potential](../../../distribution-theory.md#riesz-potential) only changes $C$. Equivalently, for $0<\lambda<n$, $p,s>1$ and $1/p+1/s+\lambda/n=2$,

$$
\boxed{\iint\frac{|f(x)||g(y)|}{|x-y|^\lambda}\,dx\,dy\leq C\|f\|_p\|g\|_s.}
$$

The exponent relation is necessary under dilation. We prove the potential estimate and then derive the bilinear version.

First establish the needed maximal estimate, so it is not an unproved step in the argument. Define the centered [Hardy-Littlewood maximal function](../../../analysis.md#hardy-littlewood-maximal-function) by $Mf(x)=\sup_{t>0}|B_t|^{-1}\int_{B_t(x)}|f|$. For integrable $f$, cover a compact subset of $\{Mf>a\}$ by finitely many balls whose averages exceed $a$. Order these balls by decreasing radius and greedily retain a ball if it is disjoint from those already retained. Every discarded ball intersects a retained ball of at least its radius, so lies in its triple. Hence

$$
|\{Mf>a\}|\leq3^n\sum_i|B_i|\leq\frac{3^n}{a}\sum_i\int_{B_i}|f|\leq\frac{3^n}{a}\|f\|_1.
$$

The passage from compact subsets uses [inner regularity of Lebesgue measure](../../../measure-theory.md#inner-regularity-of-lebesgue-measure); the superlevel set is open because fixed-radius local averages are continuous. For $f\in L^p$, split $f=f\mathbf1_{\{|f|>a/2\}}+f\mathbf1_{\{|f|\leq a/2\}}$. The second summand's maximal function is at most $a/2$, and the first is integrable. Therefore

$$
|\{Mf>a\}|\leq\frac{2\cdot3^n}{a}\int_{|f|>a/2}|f|.
$$

The [layer cake representation](../../../functional-analysis.md#layer-cake-representation) and [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) give

$$
\begin{aligned}\|Mf\|_p^p&=p\int_0^\infty a^{p-1}|\{Mf>a\}|\,da\\
&\leq2\cdot3^np\int|f(x)|\int_0^{2|f(x)|}a^{p-2}\,da\,dx
=\frac{3^np2^p}{p-1}\|f\|_p^p.
\end{aligned}
$$

Thus the [Strong Lp bound for the Hardy-Littlewood maximal function](../../../analysis.md#strong-lp-bound-for-the-hardy-littlewood-maximal-function) is proved for every $p>1$.

For $I_\alpha|f|(x)$, split at radius $R$. Dyadic shells with radii $2^{-j}R$ give

$$
\int_{|x-y|<R}|x-y|^{\alpha-n}|f(y)|\,dy\leq C\sum_{j\geq0}(2^{-j}R)^\alpha Mf(x)\leq CR^\alpha Mf(x).
$$

For the outer part, [Hölder's inequality](../../../real-analysis.md#holder-s-inequality) gives

$$
\int_{|x-y|\geq R}|x-y|^{\alpha-n}|f(y)|\,dy\leq\|f\|_p\left(\int_{|z|\geq R}|z|^{(\alpha-n)p'}dz\right)^{1/p'}=C\|f\|_pR^{\alpha-n/p}.
$$

The last integral is finite exactly because $p<n/\alpha$. Balance the two bounds by $R^{n/p}=\|f\|_p/Mf(x)$ to obtain the [Hedberg inequality](../../../distribution-theory.md#hedberg-inequality)

$$
I_\alpha|f|(x)\leq C\|f\|_p^\theta(Mf(x))^{1-\theta},\qquad\theta=\alpha p/n.
$$

The zero cases follow directly or by a limit; $Mf$ is finite almost everywhere by the maximal estimate. Since $r(1-\theta)=p$, integration and the proved maximal bound yield $\|I_\alpha f\|_r\leq C\|f\|_p$. Taking $\alpha=n-\lambda$ and pairing $I_\alpha|f|$ with $|g|\in L^{r'}$ proves the bilinear form by [Hölder's inequality](../../../real-analysis.md#holder-s-inequality), because $s=r'$. All integrals are justified first for nonnegative truncations and then by monotone convergence and the resulting finite bound. The strong estimate does not include $p=1$ or $p=n/\alpha$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Write $A_q=\langle f\rangle_{w,q}$ and $N_q=\|f\|_{w,q}$. The exponent on the finite-set expression is $-1/q'$ in the PDF; the TeX aid drops its prime. Ignore zero-measure sets, whose integrals vanish. The equivalence is

$$
\boxed{A_q\leq N_q\leq q'A_q,\qquad C_{1,q}=1,\quad C_{2,q}=q'=\frac q{q-1}.}
$$

For the first bound, let $E_a=\{|f|>a\}$ and choose a finite-measure subset $E\subset E_a$. Since $\int_E|f|\geq a|E|$,

$$
N_q\geq |E|^{-1/q'}\int_E|f|\geq a|E|^{1/q}.
$$

Exhaust $E_a$ by its intersections with bounded balls. If its measure is finite these give the desired bound $a|E_a|^{1/q}$ in the limit; if it is infinite they force $N_q=\infty$. Now take the supremum over $a$.

For the other direction it suffices to assume $0<A_q<\infty$; the zero and infinite cases are immediate. For a set $E$ with $0<|E|=m<\infty$, the [layer cake representation](../../../functional-analysis.md#layer-cake-representation) gives

$$
\int_E|f|=\int_0^\infty|E\cap E_t|\,dt\leq\int_0^\infty\min\{m,(A_q/t)^q\}\,dt.
$$

Split at $t_0=A_qm^{-1/q}$. The first contribution is $mt_0$, and the second is $A_q^qt_0^{1-q}/(q-1)$. Their sum is $q'A_qm^{1/q'}$. Multiply by $m^{-1/q'}$ and take the supremum. This proves the equivalence even when the quantities are extended-valued. The integral expression is an actual [norm](../../../functional-analysis.md#norm) on the [weak Lq space](../../../measure-theory.md#weak-lq-space), since the [triangle inequality](../../../topological-analysis.md#triangle-inequality) holds inside every set integral. The distribution-function expression is generally a [quasi-norm](../../../functional-analysis.md#quasi-norm). The factor $q'$ is sharp: $f(x)=x^{-1/q}$ on $(0,\infty)$ has $A_q=1$ and attains $N_q=q'$ on every initial interval. In higher dimensions, multiply this example by the indicator of a unit box in the remaining coordinates.

## 3

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

As usual, the bounded set is assumed Lebesgue measurable and an $L^q$ exponent is positive; the conventional Banach-space assertion concerns $1\leq q<2^*=2n/(n-2)$. No boundary regularity of $\Omega$ is needed. Choose a smooth compactly supported cutoff $\eta$ equal to one on a ball containing $\Omega$. [Weak convergence](../../../weak-topology.md#weak-convergence) and the [Uniform boundedness principle](../../../banach-space.md#uniform-boundedness-principle) give a common $H^1$ bound for $f_j$, hence also for $g_j=\eta f_j$. These functions have a common compact support.

We prove their local $L^2$ compactness directly. Translation and the fundamental theorem along line segments give, by density from smooth functions,

$$
\|g_j(\cdot-h)-g_j\|_2\leq |h|\|\nabla g_j\|_2.
$$

For a compactly supported [mollifier](../../../distribution-theory.md#mollifier) $\rho_\varepsilon$, integration of this estimate gives

$$
\|g_j*\rho_\varepsilon-g_j\|_2\leq C\varepsilon\|\nabla g_j\|_2\leq C'\varepsilon.
$$

At fixed $\varepsilon$, [Hölder's inequality](../../../real-analysis.md#holder-s-inequality) bounds $\|g_j*\rho_\varepsilon\|_\infty$ and $\|\nabla(g_j*\rho_\varepsilon)\|_\infty$ uniformly by the $L^2$ [norm](../../../functional-analysis.md#norm) of the corresponding smoothing kernels. Their supports lie in one fixed compact set, so the [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) makes this smoothed family precompact in $L^2$. The uniform $O(\varepsilon)$ approximation makes the original family totally bounded in $L^2$: choose a finite net for the smoothed family and add the approximation error. Completeness gives relative compactness.

Every strongly convergent subsequence of $g_j$ has limit $\eta f$, since multiplication by $\eta$ preserves weak $L^2$ convergence. Consequently the whole sequence converges strongly: otherwise a subsequence with distance at least a fixed positive number would have a further convergent subsequence and contradict that unique limit. In particular $\|\chi_\Omega(f_j-f)\|_2\to0$.

The critical [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality) supplies a uniform bound in $L^{2^*}$. For clarity, this estimate follows from part 2(a), not from compactness at the critical exponent. For a compactly supported smooth $v$, integrating by parts against the vector field $(x-y)/|x-y|^n$ gives

$$
|v(x)|\leq C_n\int |x-y|^{1-n}|\nabla v(y)|\,dy.
$$

Its distributional divergence is the sphere-area multiple of a point mass; applying the [Hardy–Littlewood–Sobolev inequality](../../../nonlinear-analysis.md#hardy-littlewood-sobolev-inequality) with $\alpha=1,p=2$ yields $\|v\|_{2^*}\leq C\|\nabla v\|_2$. Density extends this to $H^1(\mathbb R^n)$.

For $2<q<2^*$ choose $0<\theta<1$ with $1/q=\theta/2+(1-\theta)/2^*$. [Hölder's inequality](../../../real-analysis.md#holder-s-inequality) gives

$$
\|\chi_\Omega(f_j-f)\|_q\leq\|\chi_\Omega(f_j-f)\|_2^\theta\|\chi_\Omega(f_j-f)\|_{2^*}^{1-\theta}\longrightarrow0.
$$

For $1\leq q<2$, use $\|v\|_{L^q(\Omega)}\leq|\Omega|^{1/q-1/2}\|v\|_{L^2(\Omega)}$. The same integral estimate also works for $0<q<1$ if $L^q$ is understood with its usual quasi-[norm](../../../functional-analysis.md#norm). Thus **$\chi_\Omega f_j\to\chi_\Omega f$ strongly for every positive $q<2^*$**. We have never asserted that multiplying by the possibly nonsmooth indicator preserves $H^1$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a bounded connected domain with the [interior cone property](../../../sobolev-space.md#interior-cone-property), and $1\leq p<n$, the mean-zero form of the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) is

$$
\boxed{\|v-v_\Omega\|_{L^p(\Omega)}\leq C_{\Omega,p}\|\nabla v\|_{L^p(\Omega)},\qquad v_\Omega=\frac1{|\Omega|}\int_\Omega v.}
$$

No zero boundary trace is imposed. Subtracting the mean is essential because nonzero constants have zero [gradient](../../../calculus.md#gradient).

Suppose the estimate failed. Subtract means and normalize to obtain $v_j\in W^{1,p}(\Omega)$ with

$$
\int_\Omega v_j=0,\qquad\|v_j\|_p=1,\qquad\|\nabla v_j\|_p\longrightarrow0.
$$

This sequence is bounded in the [Sobolev space](../../../sobolev-space.md) $W^{1,p}$. The allowed [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem) on cone domains provides a subsequence converging strongly in $L^p(\Omega)$ to $v$. Its mean is zero and its [norm](../../../functional-analysis.md#norm) is one. For any compactly supported smooth [test function](../../../distribution-theory.md#test-function) $\phi$,

$$
\int v\partial_i\phi=\lim_j\int v_j\partial_i\phi=-\lim_j\int(\partial_i v_j)\phi=0.
$$

Thus every [weak derivative](../../../distribution-theory.md#weak-derivative) of $v$ vanishes. To show this implies constancy, mollify on any ball compactly contained in $\Omega$. The resulting smooth function has zero [gradient](../../../calculus.md#gradient) and is constant on the smaller ball. Passing to its $L^p$ limit makes $v$ constant almost everywhere on that ball. Overlapping balls have the same constant, and [connectedness](../../../geometry-and-topology.md#connected-space) connects any two points by a chain of such balls. Hence $v$ is constant almost everywhere throughout $\Omega$. Its zero mean makes it zero, contradicting [norm](../../../functional-analysis.md#norm) one. This proves the stated [Poincaré inequality](../../../sobolev-space.md#poincare-inequality). The frequently used stronger Sobolev-Poincare formulation also follows: with $p^*=np/(n-p)$, the cone-domain [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) gives $\|w\|_{p^*}\leq C_S(\|w\|_p+\|\nabla w\|_p)$. Insert $w=v-v_\Omega$ and the estimate just proved to obtain

$$
\boxed{\|v-v_\Omega\|_{L^{p^*}(\Omega)}\leq C_S(1+C_{\Omega,p})\|\nabla v\|_{L^p(\Omega)}.}
$$

Thus both the same-exponent and critical-exponent mean-zero versions are covered. Connectedness cannot be dropped without subtracting a separate mean on every component. The usual meaning of the stated range is $1\leq p<n$; $W^{1,p}$ with $p<1$ is not part of this Sobolev-space formulation.

## 4

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $\phi$ be a [test function](../../../distribution-theory.md#test-function) supported in $[-R,R]$. Symmetric cancellation gives

$$
\operatorname{PV}\frac1x(\phi)=\int_0^R\frac{\phi(x)-\phi(-x)}x\,dx.
$$

The integrand is bounded by $2\|\phi'\|_\infty$, so the limit exists and

$$
\left|\operatorname{PV}\frac1x(\phi)\right|\leq2R\|\phi'\|_\infty.
$$

This is a continuous linear functional on every fixed-support test space, hence a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis). It also specifies its local order as at most one.

For the boundary value, split the ordinary complex denominator:

$$
\frac1{x+i\varepsilon}=\frac{x}{x^2+\varepsilon^2}-i\frac{\varepsilon}{x^2+\varepsilon^2},\qquad\varepsilon>0.
$$

The real part paired with $\phi$ is

$$
\int_0^R\frac{x[\phi(x)-\phi(-x)]}{x^2+\varepsilon^2}\,dx.
$$

It converges to the principal value by [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem), using the same bound $2\|\phi'\|_\infty$. In the second part set $x=\varepsilon t$:

$$
\int_\mathbb R\frac{\varepsilon\phi(x)}{x^2+\varepsilon^2}\,dx=\int_\mathbb R\frac{\phi(\varepsilon t)}{1+t^2}\,dt\longrightarrow\pi\phi(0).
$$

Here $\|\phi\|_\infty/(1+t^2)$ is an integrable majorant. The correct [Sokhotski–Plemelj formula](../../../complex-analysis.md#sokhotski-plemelj-theorem) is therefore

$$
\boxed{\frac1{x+i0}=\operatorname{PV}\frac1x-i\pi\delta.}
$$

The resulting functional is continuous, with bound $2R\|\phi'\|_\infty+\pi\|\phi\|_\infty$, so it too is a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis).

**The printed PDF has the wrong sign on its delta term.** For a real even nonnegative [test function](../../../distribution-theory.md#test-function) with $\phi(0)>0$, the principal value is zero while the imaginary part of every regularized integral is negative. Its limit is $-\pi\phi(0)$, disproving the printed plus sign directly. A plus sign instead belongs to the boundary value $(x-i0)^{-1}$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For every compactly supported smooth [test function](../../../distribution-theory.md#test-function) $\phi$, integration by parts in the definition of the [weak derivative](../../../distribution-theory.md#weak-derivative) gives

$$
\int f_j\partial_\ell\phi=-\int(\partial_\ell f_j)\phi.
$$

Both $\phi$ and $\partial_\ell\phi$ belong to $L^2(\mathbb R^n)$, so the assumed weak limits imply

$$
\int g\partial_\ell\phi=-\int h_\ell\phi.
$$

This is exactly the distributional characterization of $\partial_\ell g=h_\ell$. Since $g,h_1,\ldots,h_n$ are all in $L^2$, the defining condition of the [H1 space](../../../sobolev-space.md#h1-space) is satisfied. Thus

$$
\boxed{g\in H^1(\mathbb R^n),\qquad\partial_\ell g=h_\ell\quad(1\leq\ell\leq n).}
$$

For complex functions the same argument uses conjugated test functions in the $L^2$ pairing. No prior identification of an $H^1$ weak limit is needed.

## 5

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For a real locally integrable function, the definitions are distributional:

$$
\boxed{\begin{aligned}f\text{ subharmonic}&\iff\int_\Omega f\Delta\phi\geq0\quad(0\leq\phi\in C_c^\infty(\Omega)),\\
f\text{ superharmonic}&\iff\int_\Omega f\Delta\phi\leq0\quad(0\leq\phi\in C_c^\infty(\Omega)),\\
f\text{ harmonic}&\iff\int_\Omega f\Delta\phi=0\quad(\phi\in C_c^\infty(\Omega)).\end{aligned}}
$$

Thus the [Laplacian](../../../calculus.md#laplacian) is respectively a [positive distribution](../../../fourier-analysis.md#positive-distribution), a negative distribution, or zero. A [superharmonic function](../../../partial-differential-equation.md#superharmonic-function) is the negative of a [subharmonic function](../../../partial-differential-equation.md#subharmonic-function); being both is equivalent to being harmonic. For a $C^2$ function these conditions are $\Delta f\geq0$, $\Delta f\leq0$, and $\Delta f=0$ pointwise.

An $L^1_{\mathrm{loc}}$ equivalence class does not itself specify point values. For the maximum principle use the [canonical representative of a subharmonic distribution](../../../partial-differential-equation.md#canonical-representative-of-a-subharmonic-distribution)

$$
\widetilde f(x)=\lim_{r\downarrow0}\frac1{|B_r|}\int_{B_r(x)}f.
$$

These normalized integrals are ball averages. To justify this construction, first mollify $f$: its smooth local regularizations satisfy $\Delta f_\varepsilon\geq0$. For any smooth subharmonic function, the spherical mean $m_x(r)$ obeys

$$
m_x'(r)=\frac1{|\mathbb S^{n-1}|r^{n-1}}\int_{B_r(x)}\Delta f\geq0.
$$

This follows by differentiating the spherical integral and applying the [divergence theorem](../../../calculus.md#divergence-theorem). Its ball mean also increases with radius: its derivative is $n/r$ times the spherical mean minus the ball mean. Local $L^1$ convergence of the regularizations passes the monotonicity of the ball means to $f$. The decreasing-radius limit therefore exists, possibly as minus infinity at an exceptional point, and equals $f$ almost everywhere by the [Lebesgue differentiation theorem](../../../measure-theory.md#lebesgue-differentiation-theorem). It is [upper semicontinuous](../../../calculus.md#upper-semicontinuity) as the local infimum of continuous ball averages and satisfies

$$
\widetilde f(x)\leq\frac1{|B_r|}\int_{B_r(x)}\widetilde f.
$$

For a [superharmonic function](../../../partial-differential-equation.md#superharmonic-function) use the corresponding [lower semicontinuous](../../../calculus.md#lower-semicontinuity) representative and reverse the inequality.

For a distributionally [harmonic function](../../../partial-differential-equation.md#harmonic-function), the smooth regularizations are harmonic and have constant spherical means. A radial [mollifier](../../../distribution-theory.md#mollifier) $\rho_\delta$ of integral one therefore reproduces them by averaging these means. At fixed interior radius $\delta$, pass to the local $L^1$ limit to obtain $f=f*\rho_\delta$ almost everywhere on a smaller region. The right side is smooth and has zero distributional Laplacian, giving the smooth harmonic representative. This proves the relevant [Weyl lemma](../../../partial-differential-equation.md#weyl-lemma). Changing a value at a single point can spoil a pointwise maximum principle, so the representative convention is essential.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The [strong maximum principle for subharmonic functions](../../../partial-differential-equation.md#strong-maximum-principle-for-subharmonic-functions) is: on a connected open domain, the canonical [upper semicontinuous](../../../calculus.md#upper-semicontinuity) representative of a subharmonic function cannot attain a finite global maximum at an interior point unless it is constant. A local maximum instead forces constancy on an appropriate neighbourhood; it alone does not assert constancy on the whole domain unless that value is a global maximum.

Suppose $u\leq M$ on $\Omega$ and $u(x_0)=M$. For every sufficiently small ball centred at $x_0$, the subharmonic mean inequality gives

$$
M=u(x_0)\leq\frac1{|B_r|}\int_{B_r(x_0)}u\leq M.
$$

The nonnegative function $M-u$ has integral zero, so $u=M$ almost everywhere on that ball. Its canonical representative is then $M$ at every point of the ball, by taking still smaller local averages.

The maximum set $E=\{x:u(x)=M\}$ is consequently open by the same argument at each of its points. It is closed relative to $\Omega$, because upper semicontinuity makes its complement $\{u<M\}$ open. It is nonempty, and [connectedness](../../../geometry-and-topology.md#connected-space) gives $E=\Omega$. Therefore **$u\equiv M$**. This proves the principle, including its representative and [connectedness](../../../geometry-and-topology.md#connected-space) hypotheses. Arbitrary representatives do not satisfy it: the function equal to zero almost everywhere but assigned value one at the origin has zero distributional Laplacian and an artificial pointwise maximum.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The local [Harnack inequality for harmonic functions](../../../partial-differential-equation.md#harnack-inequality-for-harmonic-functions) states that if $u\geq0$ is harmonic on a neighbourhood of $\overline{B_{4r}(a)}$, then

$$
\boxed{\sup_{B_r(a)}u\leq3^n\inf_{B_r(a)}u.}
$$

More generally, for any compact $K$ in a connected open domain $\Omega$, there is $C=C(K,\Omega,n)$ such that $\sup_Ku\leq C\inf_Ku$ for every nonnegative harmonic $u$ on $\Omega$. Positivity is essential; the assertion is not for arbitrary sign-changing functions.

First prove the [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions). For a smooth harmonic function the spherical mean has derivative

$$
m_x'(t)=\frac1{|\mathbb S^{n-1}|t^{n-1}}\int_{B_t(x)}\Delta u=0,
$$

so it equals $u(x)$; integration in the radius gives the ball mean property. The preceding [Weyl lemma](../../../partial-differential-equation.md#weyl-lemma) supplies smoothness if harmonicity was initially distributional.

For $x,z\in B_r(a)$ the inclusion $B_r(x)\subset B_{3r}(z)\subset B_{4r}(a)$ and nonnegativity give

$$
u(x)=\frac1{|B_r|}\int_{B_r(x)}u\leq\frac1{|B_r|}\int_{B_{3r}(z)}u=3^nu(z).
$$

Taking the supremum over $x$ and the infimum over $z$ proves the local estimate directly. To obtain the compact-set form, connect centres of a finite ball cover of $K$ to a fixed interior point by paths in $\Omega$. The compact union of those paths stays a positive distance from the complement of $\Omega$. Subdivide the paths into finitely many steps small enough that the local estimate applies at consecutive points. Multiply the finitely many comparison constants, first from one point of $K$ to the reference point and then to any other point of $K$. This gives a constant independent of $u$. In particular a nonnegative harmonic function is either everywhere positive or identically zero on each connected component.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Fix a compact $K\subset\Omega$ and choose $\delta>0$ such that a closed $3\delta$-neighbourhood of $K$ is compactly contained in $\Omega$. The hypothesis gives a common bound $M$ on that neighbourhood. Choose a smooth radial [mollifier](../../../distribution-theory.md#mollifier) $\rho_\delta$ supported in $B_\delta(0)$ with integral one. The [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions), integrated against its radial weights, gives

$$
u_j(x)=\int\rho_\delta(x-y)u_j(y)\,dy
$$

in a neighbourhood of $K$. Differentiating this fixed-radius convolution gives the uniform interior estimate

$$
|\nabla u_j(x)|\leq M\|\nabla\rho_\delta\|_1\leq C_\rho M/\delta.
$$

Thus the sequence is equicontinuous there; taking its pointwise limit gives the same local modulus of continuity for $u$. A finite small-ball cover of $K$ now proves [uniform convergence](../../../real-analysis.md#uniform-convergence) directly: choose the cover so both $u_j$ and $u$ vary by less than $\varepsilon$ inside each ball, then use convergence at its finitely many centres to make $|u_j-u|<\varepsilon$ there. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives $\sup_K|u_j-u|<3\varepsilon$ for large $j$.

Finally, pass to the limit in the reproducing convolution identity on smaller compact sets. It yields $u=u*\rho_\delta$, so $u$ is smooth locally. Also, for each compactly supported smooth [test function](../../../distribution-theory.md#test-function) $\phi$, uniform convergence on its support gives

$$
\int_\Omega u\Delta\phi=\lim_j\int_\Omega u_j\Delta\phi=0.
$$

Hence its smooth Laplacian is zero. We have proved **$u_j\to u$ uniformly on every compact subset and $u$ is harmonic**. Using the continuous representatives in the pointwise hypothesis makes this conclusion pointwise, rather than only almost everywhere. This is [compact convergence of locally bounded harmonic functions](../../../partial-differential-equation.md#compact-convergence-of-locally-bounded-harmonic-functions).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
