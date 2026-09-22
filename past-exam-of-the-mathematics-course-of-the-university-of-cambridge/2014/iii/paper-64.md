# Paper 64

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_64.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_64.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)

## 1

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The [bounded-variation space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain) carries the [norm](../../../functional-analysis.md#norm) $\|u\|_{BV}=\|u\|_{L^1(\Omega)}+|Du|(\Omega)$. Its [weak-star convergence in BV](../../../inverse-problem.md#weak-star-convergence-in-bv) is characterized by

$$
\boxed{u_k\to u\text{ in }L^1(\Omega),\qquad Du_k\overset{*}{\rightharpoonup}Du\text{ in }\mathcal M(\Omega;\mathbb R^n).}
$$

The second condition means convergence of the [vector measure](../../../measure-theory.md#vector-measure) pairings against every $\varphi\in C_0(\Omega;\mathbb R^n)$. Equivalently, [strong convergence](../../../functional-analysis.md#norm-convergence) in $L^1$ together with $\sup_k|Du_k|(\Omega)<\infty$ suffices: [integration by parts](../../../calculus.md#integration-by-parts) identifies the limit on smooth compactly supported tests, and [uniform approximation](../../../uniform-approximation.md) extends this to $C_0$ tests.

The [bounded-variation compactness](../../../inverse-problem.md#bounded-variation-compactness) theorem says that

$$
\boxed{\sup_k\bigl(\|u_k\|_{L^1(\Omega)}+|Du_k|(\Omega)\bigr)<\infty}
$$

guarantees a [subsequence](../../../real-analysis.md#subsequence) convergent in [weak-star convergence in BV](../../../inverse-problem.md#weak-star-convergence-in-bv) on a bounded [Lipschitz domain](../../../real-analysis.md#lipschitz-domain). This is the uniform criterion for relative sequential compactness. If asking only for the existence of one convergent [subsequence](../../../real-analysis.md#subsequence), the exact condition is the existence of a BV-bounded [subsequence](../../../real-analysis.md#subsequence), equivalently $\liminf_k\|u_k\|_{BV}<\infty$. The entire sequence need not be bounded: alternating zero functions and constants tending to infinity gives a simple example. Conversely, a convergent [subsequence](../../../real-analysis.md#subsequence) has bounded $L^1$ [norm](../../../functional-analysis.md#norm) and bounded [total variation seminorm](../../../inverse-problem.md#total-variation-seminorm-on-a-domain) by the [Uniform boundedness principle](../../../banach-space.md#uniform-boundedness-principle) for its derivative-measure pairings.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Use a [bounded BV extension operator](../../../inverse-problem.md#bounded-bv-extension-operator) for the bounded [Lipschitz domain](../../../real-analysis.md#lipschitz-domain). Extend $u_k$ to $w_k\in BV(\mathbb R^n)$, supported in one fixed [compact set](../../../topology.md#compact-space), with $\|w_k\|_{BV(\mathbb R^n)}\le C_\Omega\|u_k\|_{BV(\Omega)}$. Such an extension is obtained by reflection in Lipschitz boundary charts, a [partition of unity](../../../differential-geometry.md#partition-of-unity) and a fixed [cutoff function](../../../distribution-theory.md#cutoff-function). A naive zero extension must also charge its boundary-trace jump; it cannot discard that contribution.

Let $M$ bound these [norms](../../../functional-analysis.md#norm) and let $w_{k,\epsilon}=w_k*\rho_\epsilon$ be their [mollifications](../../../distribution-theory.md#mollification). The [BV mollification error estimate](../../../inverse-problem.md#bv-mollification-error-estimate) gives

$$
\|w_{k,\epsilon}-w_k\|_1\le\epsilon|Dw_k|(\mathbb R^n)\le\epsilon M.
$$

The [variation measure](../../../measure-theory.md#variation-measure) here is on $\mathbb R^n$. The printed lemma's $|Dw|(\Omega)$ needs this correction unless it also assumes all the [derivative](../../../calculus.md#derivative) mass lies in $\Omega$: a nonconstant bump supported outside $\overline\Omega$ disproves its literal wording. The correct estimate follows by averaging the [BV translation estimate](../../../inverse-problem.md#bv-translation-estimate) $\|w(\cdot-h)-w\|_1\le|h||Dw|(\mathbb R^n)$ over a mollifier supported in $|h|\le\epsilon$.

For each fixed $\epsilon>0$, [convolution](../../../fourier-analysis.md#convolution) gives uniform bounds

$$
\|w_{k,\epsilon}\|_\infty\le M\|\rho_\epsilon\|_\infty,\qquad \|\nabla w_{k,\epsilon}\|_\infty\le M\|\nabla\rho_\epsilon\|_\infty.
$$

The [mollifications](../../../distribution-theory.md#mollification) have common [compact support](../../../function.md#compact-support) and are uniformly [equicontinuous](../../../topological-analysis.md#equicontinuity). The [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) supplies a uniformly convergent [subsequence](../../../real-analysis.md#subsequence) at each scale $\epsilon=1/m$. A diagonal [subsequence](../../../real-analysis.md#subsequence) converges at every one of those scales. For two late members of that [subsequence](../../../real-analysis.md#subsequence),

$$
\|w_k-w_\ell\|_1\le2M/m+\|w_{k,1/m}-w_{\ell,1/m}\|_1.
$$

First choose large $m$, then late $k,\ell$; the sequence is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) in $L^1$. Its limit $w$ belongs to the [BV space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain) because the [total variation seminorm on a domain](../../../inverse-problem.md#total-variation-seminorm-on-a-domain) is [sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity). Uniform [derivative](../../../calculus.md#derivative) bounds and [integration by parts](../../../calculus.md#integration-by-parts) give $Dw_k\overset{*}{\rightharpoonup}Dw$. Restriction to $\Omega$ proves the required [weak-star convergence in BV](../../../inverse-problem.md#weak-star-convergence-in-bv).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Apply the [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations) to $J(u)=\|f-Ku\|_1+\alpha|Du|(\Omega)$. Since $J(0)=\|f\|_1$, take a [minimizing sequence](../../../calculus-of-variations.md#minimizing-sequence) with $J(u_k)\le C:=\|f\|_1+1$. Then

$$
|Du_k|(\Omega)\le C/\alpha,\qquad \|Ku_k\|_1\le\|f\|_1+C,\qquad \|u_k\|_1\le\|K^{-1}\|\,(\|f\|_1+C).
$$

Thus the sequence is bounded in the [bounded-variation space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain). The [bounded-variation compactness](../../../inverse-problem.md#bounded-variation-compactness) gives a [subsequence](../../../real-analysis.md#subsequence) converging in the [strong convergence](../../../functional-analysis.md#norm-convergence) sense in $L^1$ to $u\in BV(\Omega)$. Boundedness of the [linear operator](../../../vector-space.md#linear-operator) $K$ gives $Ku_k\to Ku$ strongly in $L^1$, so the residual [norm](../../../functional-analysis.md#norm) converges. The variation term is [sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity), hence

$$
\boxed{J(u)\le\liminf_kJ(u_k)=\inf_{v\in BV(\Omega)}J(v).}
$$

Therefore $u$ attains the infimum. The useful inverse hypothesis is the lower bound $\|u\|_1\le C_K\|Ku\|_1$; a [bounded inverse](../../../topological-vector-space.md#bounded-inverse) on the range already suffices for this proof. No uniqueness follows from the nonsquared $L^1$ fidelity.

## 2

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For a scalar $u\in BV(\Omega)$, put $E_t=\{x\in\Omega:u(x)>t\}$. The [coarea formula for BV functions](../../../inverse-problem.md#coarea-formula-for-bv-functions) is the [measure](../../../measure-theory.md#measure) identity

$$
\boxed{|Du|(A)=\int_{\mathbb R}\operatorname{Per}(E_t;A)\,dt}
$$

for every Borel $A\subseteq\Omega$. For almost every real $t$, $E_t$ is a [finite-perimeter set](../../../inverse-problem.md#set-of-finite-perimeter), with $\operatorname{Per}(E_t;A)=|D\chi_{E_t}|(A)$. In particular $\operatorname{TV}(u)=\int_{\mathbb R}\operatorname{Per}(E_t;\Omega)dt$. This is [relative perimeter](../../../inverse-problem.md#relative-perimeter): it counts interfaces inside $\Omega$, and does not add the boundary jump of a zero extension.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For $t\in\mathbb R$, define the set functional

$$
F_t(E)=\alpha\operatorname{Per}(E;\Omega)+\int_E(t-f)\,dx.
$$

The [ROF level-set formulation](../../../inverse-problem.md#rof-level-set-formulation) states that the unique [minimizer](../../../analysis.md#global-minimizer) of $J(u)=\|u-f\|_2^2/2+\alpha\operatorname{TV}(u)$ has [superlevel sets](../../../topology.md#superlevel-set) minimizing $F_t$ for almost every $t$. Conversely, an admissible $u$ with minimizing [superlevel sets](../../../topology.md#superlevel-set) is the ROF [minimizer](../../../analysis.md#global-minimizer). Thus the concise characterization is

$$
\boxed{\hat u\text{ minimizes ROF}\iff\{\hat u>t\}\in\arg\min_E F_t(E)\text{ for a.e. }t.}
$$

The [signed layer-cake identity for quadratic fidelity](../../../inverse-problem.md#signed-layer-cake-identity-for-quadratic-fidelity) and the [coarea formula for BV functions](../../../inverse-problem.md#coarea-formula-for-bv-functions) give

$$
J(u)-\frac12\|f\|_2^2=\int_{\mathbb R}\bigl[F_t(\{u>t\})-F_t(E_t^0)\bigr]dt,\qquad E_t^0=\begin{cases}\Omega,&t<0,\\\varnothing,&t\ge0.\end{cases}
$$

Indeed $u^2/2-fu=\int_{\mathbb R}(t-f)(\chi_{\{u>t\}}-\chi_{\{0>t\}})dt$ pointwise. Its absolute integral is bounded by $u^2/2+|fu|$, so [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) applies for $u,f\in L^2$. The negative-level baseline is essential; integrating the unadjusted $F_t$ would generally diverge.

Each $F_t$ attains its minimum. A [minimizing sequence](../../../calculus-of-variations.md#minimizing-sequence) of [indicator functions](../../../measure-theory.md#indicator-function) has bounded $L^1$ [norm](../../../functional-analysis.md#norm), and comparison with the empty set bounds its perimeter by an $L^1$ forcing bound. [Bounded-variation compactness](../../../inverse-problem.md#bounded-variation-compactness) supplies a limiting [indicator function](../../../measure-theory.md#indicator-function). The forcing integral converges by [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem), while [relative perimeter](../../../inverse-problem.md#relative-perimeter) is [sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity).

For $s<t$, the supplied comparison lemma applied to $(f-t)/\alpha<(f-s)/\alpha$ makes every selected [minimizer](../../../analysis.md#global-minimizer) $A_t$ contained in $A_s$ up to a [null set](../../../measure-theory.md#null-set). The [comparison of perimeter minimizers with ordered forcing](../../../inverse-problem.md#comparison-of-perimeter-minimizers-with-ordered-forcing) also follows directly: compare $A_t$ with $A_t\cap A_s$, compare $A_s$ with $A_t\cup A_s$, add and use [submodularity of relative perimeter](../../../inverse-problem.md#submodularity-of-relative-perimeter) to obtain $(t-s)|A_t\setminus A_s|\le0$.

Select [minimizers](../../../analysis.md#global-minimizer) at rational levels, remove their countably many exceptional [null sets](../../../measure-theory.md#null-set), and reconstruct $v(x)=\sup\{q\in\mathbb Q:x\in A_q\}$. The strict [superlevel set](../../../topology.md#superlevel-set) is $\{v>t\}=\bigcup_{q>t}A_q$. This union also minimizes $F_t$: take $q\downarrow t$, use monotone $L^1$ convergence of its [indicator functions](../../../measure-theory.md#indicator-function) and [sequential lower semicontinuity](../../../calculus.md#sequential-lower-semicontinuity), and note that $m(t)=\min_EF_t(E)$ satisfies $|m(t)-m(s)|\le|\Omega||t-s|$.

To justify finite energy before assuming it, clip this reconstruction to $v_M\in[-M,M]$. Comparison with the empty set gives $\alpha\operatorname{Per}(E_t;\Omega)\le\int_\Omega|t-f|$ uniformly on a bounded interval of levels. Since $v_M=-M+\int_{-M}^M\chi_{E_t}\,dt$, pairing with compactly supported test-field divergences bounds its [total variation seminorm](../../../inverse-problem.md#total-variation-seminorm-on-a-domain) by $\int_{-M}^M\operatorname{Per}(E_t;\Omega)dt<\infty$. Thus $v_M$ belongs to the [BV space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain) before applying the [coarea formula for BV functions](../../../inverse-problem.md#coarea-formula-for-bv-functions). The layer-cake argument on the finite interval $[-M,M]$ shows $J(v_M)\le J(T_Mw)$ for every finite-energy competitor $w$, where $T_M$ is clipping. In particular $w=0$ bounds the $L^2$ [norms](../../../functional-analysis.md#norm) and variations uniformly. [Fatou's lemma](../../../measure-theory.md#fatou-s-lemma) excludes infinite values of $v$ on a positive-measure set. [Bounded-variation compactness](../../../inverse-problem.md#bounded-variation-compactness) and [weak convergence](../../../weak-topology.md#weak-convergence) in $L^2$ identify an admissible limit $v$. For any fixed competitor, $T_Mw\to w$ in $L^2$ and its variation tends to that of $w$, by [bounded-variation contraction under clipping](../../../inverse-problem.md#bounded-variation-contraction-under-clipping) and [sequential lower semicontinuity](../../../calculus.md#sequential-lower-semicontinuity). Thus $J(v)\le J(w)$.

The [quadratic fidelity](../../../inverse-problem.md#quadratic-fidelity) is [strictly convex](../../../real-analysis.md#strictly-convex-function), so every ROF [minimizer](../../../analysis.md#global-minimizer) equals $v$ [almost everywhere](../../../measure-theory.md#almost-everywhere) and has the selected minimizing [superlevel sets](../../../topology.md#superlevel-set). Conversely, for any $u$ whose levels minimize $F_t$, integrate the levelwise inequality against any competitor's levels in the displayed identity to obtain $J(u)\le J(w)$. This proves both directions for signed as well as nonnegative data.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The literal assumptions suffice for the scalar [quadratic fidelity](../../../inverse-problem.md#quadratic-fidelity) problem. One can avoid regularity of level-set boundaries by moving only a clipped part of the [minimizer](../../../analysis.md#global-minimizer). We prove the stronger [jump-amplitude inequality for total variation denoising](../../../inverse-problem.md#jump-amplitude-inequality-for-total-variation-denoising):

$$
\boxed{[u]_{\nu_u}\bigl([f]_{\nu_u}-[u]_{\nu_u}\bigr)\ge0\quad\mathcal H^{n-1}\text{-a.e. on }J_u.}
$$

Comparison with the zero function gives finite energy and hence $u\in L^2$. Here $u=\hat u$, and both differences use the same oriented [BV traces on a hypersurface](../../../inverse-problem.md#bv-trace-on-a-hypersurface). Reversing the normal reverses both differences and leaves the inequality unchanged. Outside $J_f$, the two traces of $f$ agree, so the inequality would read $-[u]^2\ge0$ at a jump of $u$. It therefore gives the requested [no-new-jumps property of total variation denoising](../../../inverse-problem.md#no-new-jumps-property-of-total-variation-denoising) in every dimension.

First use [residual-preserving clipping of an ROF minimizer](../../../inverse-problem.md#residual-preserving-clipping-of-an-rof-minimizer). For an integer $M>0$, put

$$
w=T_Mu=\max(-M,\min(M,u)),\qquad r=u-w,\qquad g=f-r=f-u+w.
$$

The [coarea formula for BV functions](../../../inverse-problem.md#coarea-formula-for-bv-functions) gives [scalar total variation splitting under clipping](../../../inverse-problem.md#scalar-total-variation-splitting-under-clipping):

$$
\operatorname{TV}(u)=\operatorname{TV}(w)+\operatorname{TV}(r).
$$

Indeed the levels in $(-M,M)$ contribute to $w$, while the levels outside that interval contribute to $r$. This uses the full signed coarea formula. For any $z\in BV(\Omega)\cap L^2(\Omega)$, minimality of $u$ and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) for the [total variation seminorm](../../../inverse-problem.md#total-variation-seminorm-on-a-domain) give

$$
\alpha\operatorname{TV}(w)+\alpha\operatorname{TV}(r)+\tfrac12\|w-g\|_2^2
\le\alpha\operatorname{TV}(z+r)+\tfrac12\|z-g\|_2^2
\le\alpha\operatorname{TV}(z)+\alpha\operatorname{TV}(r)+\tfrac12\|z-g\|_2^2.
$$

Cancel the tail variation. Thus $w$ is a bounded [ROF denoising](../../../inverse-problem.md#total-variation-denoising) [minimizer](../../../analysis.md#global-minimizer) for $g\in BV(\Omega)\cap L^2(\Omega)$. The data $g$ may still be unbounded. This is an exact reduction preserving $w-g=u-f$; it does not truncate the data and then pass to a limit of different reconstructions.

We next prove the [jump-amplitude inequality for a bounded ROF minimizer](../../../inverse-problem.md#jump-amplitude-inequality-for-a-bounded-rof-minimizer), allowing its data to be unbounded. Fix a coordinate $j$, a nonnegative $\varphi\in C_c^\infty(\Omega)$, and let $\Phi_t$ be the [local flow](../../../differential-geometry.md#local-flow) of the smooth [vector field](../../../calculus.md#vector-field) $Y=\varphi e_j$. The flow is the identity near the domain boundary, preserves each line parallel to $e_j$, and satisfies $\Phi_{-t}=\Phi_t^{-1}$. Write

$$
T_ta=a\circ\Phi_t,\qquad \delta_ta=T_ta-a,\qquad J_t=\det D\Phi_t.
$$

These maps are [diffeomorphisms](../../../geometry-and-topology.md#diffeomorphism), with $J_{\pm t}=1+O(t)$ and $J_t+J_{-t}-2=O(t^2)$ uniformly.

The useful trace calculation is the [BV jump-product limit with one bounded factor](../../../inverse-problem.md#bv-jump-product-limit-with-one-bounded-factor). For $a\in BV(\Omega)$ and $b\in BV(\Omega)\cap L^\infty(\Omega)$,

$$
\lim_{t\downarrow0}\frac1t\int_\Omega\delta_ta\,\delta_tb\,dx
=\int_{J_b}[a]_{\nu_b}[b]_{\nu_b}\,\varphi|\nu_b\cdot e_j|\,d\mathcal H^{n-1}.
$$

The right side is integrable: $|[b]|\le2\|b\|_\infty$ and only the common jump part of $a$ contributes. The same limit holds with both increments replaced by their negative-time increments, still dividing by positive $t$.

Here is why this calculation needs only one bounded factor. By the [BV slicing theorem](../../../inverse-problem.md#bv-slicing-theorem), almost every coordinate slice of $a$ and $b$ has one-sided representatives. On one such interval let $\mu=Da$ and use its right-continuous representative. Since $\varphi\ge0$,

$$
\delta_ta(x)=\mu((x,\Phi_t(x)]).
$$

[Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) rewrites the slice integral as

$$
\frac1t\int\delta_ta\,\delta_tb\,dx
=\int\left(\frac1t\int_{\Phi_{-t}(s)}^s\delta_tb(x)\,dx\right)d\mu(s).
$$

At each interior $s$, the inner expression tends to $\varphi(s)(b(s+)-b(s-))$; if $\varphi(s)=0$, it is zero. Its absolute value is at most $2\|b\|_\infty\|\varphi\|_\infty$. [Dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) against $|\mu|$ therefore leaves just the [measure atoms](../../../measure-theory.md#atom-measure-theory) common to the two slices. The bound $2\|b\|_\infty\|\varphi\|_\infty|Da|$ is also integrable over the transverse coordinates, by the [BV slicing theorem](../../../inverse-problem.md#bv-slicing-theorem). Integrating the slice jump sums gives the surface integral and its factor $|\nu_b\cdot e_j|$. Negative-time increments give the same product, because both slice differences reverse sign. At no point is a uniform bound on $a$ across the slices required.

For $0<\theta<1$, use the mixed competitors

$$
w_t=(1-\theta)w+\theta T_tw.
$$

The [total variation under opposite smooth flows](../../../inverse-problem.md#total-variation-under-opposite-smooth-flows) satisfies

$$
\operatorname{TV}(T_tw)+\operatorname{TV}(T_{-t}w)-2\operatorname{TV}(w)=O(t^2).
$$

To see this for the entire [vector Radon measure](../../../measure-theory.md#vector-radon-measure) $Dw=\sigma_w|Dw|$, the [change of variables formula](../../../calculus.md#change-of-variables-formula) gives

$$
\operatorname{TV}(T_tw)=\int_\Omega|\operatorname{cof}(D\Phi_{-t})\sigma_w|\,d|Dw|.
$$

For $\operatorname{cof}A=(\det A)A^{-T}$, the two [cofactor matrices](../../../linear-algebra.md#cofactor-matrix) expand as $I\pm tB+O(t^2)$, with the same $B$ and opposite signs. Their [norm](../../../functional-analysis.md#norm) expansions on $|\sigma_w|=1$ have cancelling linear terms. Integrating proves the estimate, including the absolutely continuous, jump and Cantor parts. The BV transformation formula is also given in [Lemma 4.2 on differentiable regularizers](https://arxiv.org/html/2312.01900v2); that lemma does not assume bounded data. The [total variation seminorm](../../../inverse-problem.md#total-variation-seminorm-on-a-domain) is a [convex function](../../../real-analysis.md#convex-function), so

$$
\operatorname{TV}(w_t)+\operatorname{TV}(w_{-t})-2\operatorname{TV}(w)\le O(t^2).
$$

Thus minimality forces the sum of the two fidelity changes to have nonnegative limit after division by $t$.

It remains to evaluate that sum without bounding $g$. Put $F_g(v)=\tfrac12\|v-g\|_2^2$. Exact expansion of the [quadratic fidelity](../../../inverse-problem.md#quadratic-fidelity), together with [change of variables](../../../calculus.md#change-of-variables-formula), gives the [opposite-flow fidelity identity for quadratic data](../../../inverse-problem.md#opposite-flow-fidelity-identity-for-quadratic-data):

$$
F_g(w_t)+F_g(w_{-t})-2F_g(w)
=-\frac{\theta(1-\theta)}2\bigl(\|\delta_tw\|_2^2+\|\delta_{-t}w\|_2^2\bigr)
+\theta\int\delta_tg\,\delta_tw\,dx+o(t).
$$

For completeness, the cross-term identity fixing its sign is

$$
\int g(\delta_tw+\delta_{-t}w)\,dx
=-\int\delta_tg\,\delta_tw\,dx+\int g(1-J_{-t})\delta_{-t}w\,dx.
$$

The last integral is $o(t)$: $\|1-J_{-t}\|_\infty=O(t)$, while

$$
\int|g|\,|\delta_{-t}w|\,dx
\le K\|\delta_{-t}w\|_1+2\|w\|_\infty\int_{\{|g|>K\}}|g|\,dx\longrightarrow0.
$$

Take $t\to0$ first, then $K\to\infty$. Here $g\in L^1$ and the [local flow](../../../differential-geometry.md#local-flow) is strongly continuous in $L^1$. The remaining Jacobian mass term is $O(t^2)\|w\|_2^2$. This argument avoids multiplying an unbounded fidelity derivative by an uncontrolled derivative measure.

Apply the [BV jump-product limit with one bounded factor](../../../inverse-problem.md#bv-jump-product-limit-with-one-bounded-factor) with $(a,b)=(g,w)$ and $(w,w)$, and use minimality. For every nonnegative $\varphi$ and every coordinate $j$,

$$
0\le\int_{J_w}\left([g][w]-(1-\theta)[w]^2\right)\varphi|\nu_w\cdot e_j|\,d\mathcal H^{n-1}.
$$

Let $\theta\downarrow0$. These are inequalities for finite signed [Radon measures](../../../measure-theory.md#radon-measure), so arbitrary nonnegative smooth tests imply nonnegativity of their densities. Since at least one coordinate of a unit normal is nonzero,

$$
[w]([g]-[w])\ge0\quad\mathcal H^{n-1}\text{-a.e. on }J_w.
$$

This proves the bounded-minimizer lemma with arbitrary $BV\cap L^2$ data.

Finally return to $w=T_Mu$ and $g=f-u+w$. At almost every finite [approximate jump point](../../../inverse-problem.md#approximate-jump-point) of $u$, choose an integer $M>\max(|u^+|,|u^-|)$. The [BV traces on a hypersurface](../../../inverse-problem.md#bv-trace-on-a-hypersurface) commute with clipping, so $w^\pm=u^\pm$, $r^\pm=0$ and $g^\pm=f^\pm$ there. It is consequently a jump point of $w$, and its inequality is exactly $[u]([f]-[u])\ge0$. A countable union over $M$ removes all exceptional surface-null sets. Outside $J_f$, the [BV traces on a hypersurface](../../../inverse-problem.md#bv-trace-on-a-hypersurface) of $f$ agree almost everywhere. We conclude

$$
\boxed{\mathcal H^{n-1}(J_{\hat u}\setminus J_f)=0\qquad\text{for }f\in BV(\Omega)\cap L^2(\Omega),\ \Omega\subset\mathbb R^n.}
$$

The mechanism is exact scalar coarea splitting, paired smooth-flow variations, a one-bounded-factor BV trace limit, and localization through integer clipping levels. It works in every dimension under the printed hypotheses, without essential boundedness of $f$ or $u$ and without regularity of their level-set boundaries.

In [total variation calibration](../../../inverse-problem.md#total-variation-calibration) notation, $\operatorname{div}z=(u-f)/\alpha$. Since this divergence is itself in the [BV space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain), the proved inequality equivalently reads

$$
[u]_{\nu_u}[\operatorname{div}z]_{\nu_u}\le0.
$$

Thus an upward output jump forces the appropriate nonpositive jump of the calibrated divergence. This is a consequence of the variational argument above, with common oriented [BV traces on a hypersurface](../../../inverse-problem.md#bv-trace-on-a-hypersurface); no curvature of the rectifiable interface or differentiability of its normal is assumed.

## 3

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [structure theorem for functions of bounded variation](../../../inverse-problem.md#structure-theorem-for-functions-of-bounded-variation) is the [measure](../../../measure-theory.md#measure) representation of the [distributional derivative](../../../distribution-theory.md#distributional-derivative): for $u\in BV(\Omega)$ there is a unique finite [vector Radon measure](../../../measure-theory.md#vector-radon-measure) $Du$ with

$$
\boxed{\int_\Omega u\,\operatorname{div}\varphi\,dx=-\int_\Omega\varphi\cdot dDu,\qquad |Du|(\Omega)=\operatorname{TV}(u)}
$$

for every $\varphi\in C_c^1(\Omega;\mathbb R^n)$. It also has a [polar decomposition of a vector measure](../../../measure-theory.md#polar-decomposition-of-a-vector-measure) $Du=\sigma_u|Du|$ with $|\sigma_u|=1$ for $|Du|$-almost every point.

To prove it, let $L(\varphi)=-\int u\operatorname{div}\varphi$. The test-function definition of [total variation seminorm](../../../inverse-problem.md#total-variation-seminorm-on-a-domain), applied to both signs, gives $|L(\varphi)|\le\operatorname{TV}(u)\|\varphi\|_\infty$. Compactly supported smooth [vector fields](../../../calculus.md#vector-field) are uniformly dense in $C_0(\Omega;\mathbb R^n)$, so $L$ extends uniquely to a bounded functional there. The [Riesz-Markov-Kakutani representation theorem](../../../functional-analysis.md#riesz-markov-kakutani-representation-theorem), applied componentwise, gives the unique [vector measure](../../../measure-theory.md#vector-measure) $Du$. The operator [norm](../../../functional-analysis.md#norm) of $L$ is exactly the defining variation supremum; the vector-measure dual [norm](../../../functional-analysis.md#norm) is $|Du|(\Omega)$, proving equality. Conversely any [finite measure](../../../measure-theory.md#finite-measure) satisfying the identity bounds that supremum, so this also characterizes membership in the [BV space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain).

The [Radon-Nikodym theorem](../../../measure-theory.md#radon-nikodym-theorem) applied to the components relative to $|Du|$ gives $\sigma_u$; the definition of the [variation measure](../../../measure-theory.md#variation-measure) forces $|\sigma_u|=1$ [almost everywhere](../../../measure-theory.md#almost-everywhere). If $u$ is smooth, ordinary [integration by parts](../../../calculus.md#integration-by-parts) gives $Du=\nabla u\,\mathcal L^n$. [Compact support](../../../function.md#compact-support) of the test field removes any boundary contribution; no boundary regularity is needed for this representation statement.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

First apply [Lebesgue decomposition](../../../measure-theory.md#lebesgue-decomposition-theorem) to the [derivative](../../../calculus.md#derivative) [measure](../../../measure-theory.md#measure) relative to $\mathcal L^n$:

$$
Du=D^au+D^su,\qquad D^au=\nabla u\,\mathcal L^n,\qquad D^su\perp\mathcal L^n.
$$

Here $\nabla u$ is the almost-everywhere [approximate gradient](../../../inverse-problem.md#approximate-gradient), rather than an assertion that $u$ belongs to $W^{1,1}$. Split the singular part into its [jump part of a BV derivative](../../../inverse-problem.md#jump-part-of-a-bv-derivative) and [Cantor part of a BV derivative](../../../inverse-problem.md#cantor-part-of-a-bounded-variation-derivative):

$$
\boxed{Du=\nabla u\,\mathcal L^n+(u^+-u^-)\nu_u\,\mathcal H^{n-1}\!\lfloor J_u+D^cu.}
$$

An [approximate jump point](../../../inverse-problem.md#approximate-jump-point) has a unit normal $\nu_u$ and distinct finite [BV traces on a hypersurface](../../../inverse-problem.md#bv-trace-on-a-hypersurface) $u^+,u^-$, obtained as mean limits on the corresponding two half-balls. Their set $J_u$ is the [jump set of a BV function](../../../inverse-problem.md#jump-set-of-a-bounded-variation-function), countably $(n-1)$-rectifiable. Reversing the normal swaps the [BV traces on a hypersurface](../../../inverse-problem.md#bv-trace-on-a-hypersurface) and leaves the displayed [measure](../../../measure-theory.md#measure) unchanged. The [approximate discontinuity set](../../../inverse-problem.md#approximate-discontinuity-set) $S_u$ differs from $J_u$ only by an $\mathcal H^{n-1}$-null set.

The remaining $D^cu=D^su-D^ju$ is singular to [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) and gives zero mass to every set with sigma-finite $\mathcal H^{n-1}$ [measure](../../../measure-theory.md#measure). It is diffuse rather than a second jump contribution. In one dimension the three parts are illustrated by an [affine function](../../../vector-space.md#affine-function), a [step function](../../../measure-theory.md#step-function) and the [Cantor function](../../../mathematics.md#cantor-function), respectively. Countably many jumps therefore do not imply that the singular [derivative](../../../calculus.md#derivative) has no [Cantor part of a BV derivative](../../../inverse-problem.md#cantor-part-of-a-bounded-variation-derivative).

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Put $\mu=Du$, a finite signed [Radon measure](../../../measure-theory.md#radon-measure), and define

$$
F_l(t)=\mu((a,t)),\qquad F_r(t)=\mu((a,t]).
$$

For $\varphi\in C_c^1((a,b))$, [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) for the [signed measure](../../../measure-theory.md#signed-measure) gives

$$
-\int_a^bF_l(t)\varphi'(t)dt=-\int_{(a,b)}\!\left[\int_s^b\varphi'(t)dt\right]d\mu(s)=\int\varphi\,d\mu.
$$

Thus $DF_l=\mu=Du$. A distribution on a connected interval with zero [derivative](../../../calculus.md#derivative) is constant: any compactly supported test of integral zero is the [derivative](../../../calculus.md#derivative) of a compactly supported test, so it pairs to zero with $u-F_l$. Choose the resulting constant $c$. Then

$$
\boxed{u_l(t)=c+\mu((a,t)),\qquad u_r(t)=c+\mu((a,t])}
$$

are [one-sided representatives of a one-dimensional BV function](../../../inverse-problem.md#one-sided-representatives-of-a-one-dimensional-bv-function). The first equals $u$ [almost everywhere](../../../measure-theory.md#almost-everywhere). Their difference is $\mu(\{t\})$, nonzero at at most countably many points, so the second also equals $u$ [almost everywhere](../../../measure-theory.md#almost-everywhere).

Finite-measure continuity applied to $|\mu|$ proves $F_l(s)\to F_l(t)$ as $s\uparrow t$, and $F_r(s)\to F_r(t)$ as $s\downarrow t$. Moreover the opposite one-sided limits are $F_l(t+)=F_r(t)$ and $F_r(t-)=F_l(t)$. Consequently both representatives are continuous exactly where $\mu(\{t\})=0$. For each positive integer $m$, there are only finitely many [measure atoms](../../../measure-theory.md#atom-measure-theory) of magnitude at least $1/m$, since their total magnitudes are bounded by $|\mu|((a,b))$. Their union is countable, proving the requested discontinuity bound. This does not require the jump points to be isolated; they can be dense.

The hint's one-dimensional statement is consistent with this construction: zero $\mathcal H^0$ [measure](../../../measure-theory.md#measure) means an empty set, so $S_u\subseteq J_u$. This concerns approximate discontinuities of the [BV space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain) class; arbitrary changes of representative at points could create artificial pointwise discontinuities. The interval-mass representatives above remove that ambiguity and give the required one-sided continuity directly.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
