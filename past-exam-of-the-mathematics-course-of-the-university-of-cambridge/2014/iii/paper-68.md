# Paper 68

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_68.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_68.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [one-dimensional Sobolev representative](../../../sobolev-space.md#one-dimensional-sobolev-representative) is absolutely continuous. For $x<y$, the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) and [Holder inequality](../../../functional-analysis.md#holder-inequality) give

$$
|u(y)-u(x)|\leq\int_x^y|u'(s)|ds
\leq\|u'\|_{L^q(0,1)}|y-x|^{1-1/q}.
$$

Thus **$u$ has a representative in $C^{0,1-1/q}([0,1])$**. The qualification about representatives matters because a [Sobolev space](../../../sobolev-space.md) element is an almost-everywhere equivalence class.

In two dimensions, the [Sobolev fundamental theorem of calculus on lines](../../../sobolev-space.md#sobolev-fundamental-theorem-of-calculus-on-lines) and [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) imply that almost every horizontal and vertical slice belongs to $W^{1,q}(0,1)$ and has this one-dimensional [Hölder continuity](../../../sobolev-space.md#holder-condition). The slice seminorm depends on the slice; this does not give one uniform pointwise estimate on the square. For $q>2$, [Morrey's inequality](../../../sobolev-space.md#morrey-s-inequality) additionally gives a globally [Hölder continuous](../../../sobolev-space.md#holder-condition) representative of exponent $1-2/q$. For $1<q\leq2$, global continuity need not hold. For example, with a smooth cutoff around an interior point, $u(x)=|x-x_0|^{-a}$ lies in $W^{1,q}$ when $0<a<2/q-1$, but is unbounded. At $q=2$, the cutoff version of $\log\log(e/|x-x_0|)$ is unbounded while its [gradient](../../../calculus.md#gradient) has finite squared integral, since

$$
\int_0^\varepsilon\frac{dr}{r\log^2(e/r)}<\infty.
$$

These examples distinguish [Sobolev slicing and planar continuity](../../../sobolev-space.md#sobolev-slicing-and-planar-continuity) from a false two-dimensional application of the interval exponent.

Put $\Omega=(0,1)^2$. A [BV space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain) is a function $u\in L^1(\Omega)$ whose [distributional derivative](../../../distribution-theory.md#distributional-derivative) $Du$ is a finite vector-valued [Radon measure](../../../measure-theory.md#radon-measure). Equivalently its [total variation seminorm](../../../inverse-problem.md#total-variation-seminorm-on-a-domain) is finite:

$$
\boxed{|Du|(\Omega)=\sup_{\substack{\varphi\in C_c^1(\Omega;\mathbb R^2)\\|\varphi(x)|\leq1}}
\int_\Omega u\,\operatorname{div}\varphi\,dx.}
$$

The [BV space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain) has [norm](../../../functional-analysis.md#norm) $\|u\|_{L^1}+|Du|(\Omega)$. For $u\in W^{1,1}(\Omega)$, [integration by parts](../../../calculus.md#integration-by-parts) against the compactly supported field gives $\int u\operatorname{div}\varphi=-\int\nabla u\cdot\varphi\leq\int|\nabla u|$. Conversely the measurable choice $\varphi=-\nabla u/|\nabla u|$ on nonzero [gradients](../../../calculus.md#gradient) attains the pointwise bound. Approximating this bounded field by smooth fields, using interior cutoffs and the finite [measure](../../../measure-theory.md#measure) $|\nabla u|dx$, justifies the [supremum](../../../real-analysis.md#supremum) and gives

$$
\boxed{|Du|(\Omega)=\int_\Omega|\nabla u|dx.}
$$

It is a [norm](../../../functional-analysis.md#norm) of the [derivative](../../../calculus.md#derivative) [measure](../../../measure-theory.md#measure), rather than a pointwise [derivative](../../../calculus.md#derivative) at jump discontinuities.

There is a genuine mismatch in the printed definition of the next [functional](../../../calculus-of-variations.md#functional). Its constraints on $\varphi_0$ and $\varphi$ are independent. Hence its stated [supremum](../../../real-analysis.md#supremum), denoted $A_{\mathrm{box}}$, separates as

$$
\boxed{A_{\mathrm{box}}(u)=|\Omega|+|Du|(\Omega).}
$$

The scalar [supremum](../../../real-analysis.md#supremum) is $|\Omega|$, by cutoffs approaching one, and the vector [supremum](../../../real-analysis.md#supremum) is the variation. For an affine [image signal](../../../computer-science.md#image-signal) with $|\nabla u|=1$, this gives $2|\Omega|$, whereas the displayed square-root area would give $\sqrt2|\Omega|$. The intended [relaxed graph-area functional](../../../inverse-problem.md#relaxed-graph-area-functional) instead uses the coupled pointwise constraint $\varphi_0^2+|\varphi|^2\leq1$, giving

$$
A(u)=\int_\Omega\sqrt{1+|\nabla u|^2}\,dx+|D^su|(\Omega),
$$

where $D^su$ is the singular part of $Du$. Both readings have a [minimizer](../../../analysis.md#global-minimizer), but their equations are different.

Here is the [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations) for either reading. Let $A_\bullet$ be the literal $A_{\mathrm{box}}$ or the corrected $A$, and define the energy on $BV(\Omega)\cap L^2(\Omega)$, assigning infinity elsewhere. A [minimizing sequence](../../../calculus-of-variations.md#minimizing-sequence) has bounded energy by comparison with $u=0$. Both $A_\bullet\geq|Du|(\Omega)$, so its variation is bounded, and the fidelity bounds $\|u-g\|_2$, hence also $\|u\|_2$ and $\|u\|_1$. By [bounded-variation compactness](../../../inverse-problem.md#bounded-variation-compactness), a subsequence converges strongly in $L^1$ to $u\in BV$, and after another subsequence almost everywhere. [Fatou's lemma](../../../measure-theory.md#fatou-s-lemma) proves

$$
\int_\Omega(u-g)^2\leq\liminf_j\int_\Omega(u_j-g)^2.
$$

The regularizer is a [supremum](../../../real-analysis.md#supremum) of affine [functionals](../../../calculus-of-variations.md#functional) continuous in $L^1$, since the test-field divergence is bounded. It is therefore [lower semicontinuous](../../../calculus.md#lower-semicontinuity). Combining the two lower bounds proves **existence of a [minimizer](../../../analysis.md#global-minimizer)**. In fact the convex regularizer and the [strictly convex](../../../real-analysis.md#strictly-convex-function) squared fidelity make the [minimizer](../../../analysis.md#global-minimizer) unique up to null sets. This does not assert that the [minimizer](../../../analysis.md#global-minimizer) must belong to $W^{1,1}$.

For the intended graph area, conditionally assume that the [minimizer](../../../analysis.md#global-minimizer) is in $W^{1,1}$. For $\eta\in C_c^\infty(\Omega)$, differentiate at $u+t\eta$. The [derivative](../../../calculus.md#derivative) of the integrand is bounded by $|\nabla\eta|$, so dominated convergence applies. The weak equation is

$$
\alpha\int_\Omega\frac{\nabla u\cdot\nabla\eta}{\sqrt{1+|\nabla u|^2}}dx
+\int_\Omega(u-g)\eta\,dx=0,
$$

that is,

$$
\boxed{u-g-\alpha\operatorname{div}\frac{\nabla u}{\sqrt{1+|\nabla u|^2}}=0
\quad\hbox{in }\mathcal D'(\Omega).}
$$

This is the [graph-area Euler-Lagrange equation](../../../inverse-problem.md#graph-area-euler-lagrange-equation). Compactly supported variations impose no boundary condition in this statement.

For the literal printed [supremum](../../../real-analysis.md#supremum), the constant $|\Omega|$ drops out and one obtains [total variation denoising](../../../inverse-problem.md#total-variation-denoising). Its [total variation calibration](../../../inverse-problem.md#total-variation-calibration) form is

$$
\boxed{u-g-\alpha\operatorname{div}z=0,\qquad
|z|\leq1,\qquad z\cdot\nabla u=|\nabla u|\ \hbox{a.e.}}
$$

The distributional equation means $\alpha\int z\cdot\nabla\eta+\int(u-g)\eta=0$. In particular $z=\nabla u/|\nabla u|$ wherever the [gradient](../../../calculus.md#gradient) is nonzero; writing this quotient without handling zero [gradients](../../../calculus.md#gradient) would be incomplete. Formally the one-sided [derivative](../../../calculus.md#derivative) of $\int|\nabla u|$ is

$$
\int_{\{\nabla u\ne0\}}\frac{\nabla u}{|\nabla u|}\cdot\nabla\eta
+\int_{\{\nabla u=0\}}|\nabla\eta|.
$$

Minimality in the directions $\eta$ and $-\eta$ bounds the remaining linear [functional](../../../calculus-of-variations.md#functional) by the second integral. The [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) extends it on that zero-gradient set to a bounded vector field of magnitude at most one, furnishing $z$ and the displayed weak equation. Thus the literal definition has a nonsmooth [subgradient](../../../real-analysis.md#subgradient) equation, not the square-root equation above.

## 2

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Interpret the printed [Euclidean norm](../../../functional-analysis.md#euclidean-norm) literally on the full vector array $X^2$. It is a single global [norm](../../../functional-analysis.md#norm), not the sum of pixelwise [gradient](../../../calculus.md#gradient) lengths in [discrete isotropic total variation](../../../inverse-problem.md#discrete-isotropic-total-variation). Set $A=\nabla$ and let $A^*$ be its exact [adjoint operator](../../../hilbert-space.md#adjoint-operator) for the chosen difference and boundary conventions. The closed dual ball and its [image signal](../../../computer-science.md#image-signal) are

$$
B_\alpha=\{p\in X^2:\|p\|_2\leq\alpha\},\qquad
C=A^*B_\alpha.
$$

The set $C$ is nonempty, convex and compact, hence closed, because it is a linear [image signal](../../../computer-science.md#image-signal) of a compact ball in finite dimensions. [Euclidean norm duality](../../../functional-analysis.md#euclidean-norm-duality) gives

$$
\alpha\|Au\|_2=\sup_{p\in B_\alpha}\langle Au,p\rangle
=\sup_{w\in C}\langle u,w\rangle=\sigma_C(u),
$$

the [support function](../../../mathematical-optimization.md#support-function) of $C$.

The [metric projection onto a closed convex set](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) $w=P_Cg$ uniquely minimizes $\|g-w\|^2$ over $C$. Its [variational characterization of convex projection](../../../mathematical-optimization.md#variational-characterization-of-convex-projection) says

$$
\langle g-w,z-w\rangle\leq0\quad(z\in C).
$$

Put $u_*=g-w$. This inequality says precisely that $\sigma_C(u_*)=\langle u_*,w\rangle$. For any $v\in X$, the primal energy satisfies

$$
\sigma_C(v)+\frac12\|v-g\|^2
\geq\langle v,w\rangle+\frac12\|v-g\|^2.
$$

Completing the square shows that the right side is uniquely minimized by $v=g-w$. At that point the inequality is equality, so

$$
\boxed{u_*=g-P_Cg,\qquad C=\nabla^*B_\alpha.}
$$

This also follows from the [proximal operator of a support function](../../../convex-optimization.md#proximal-operator-of-a-support-function) and [Moreau decomposition](../../../convex-optimization.md#moreau-decomposition): the [convex conjugate](../../../convex-optimization.md#convex-conjugate) of $\sigma_C$ is the [indicator functional of a constraint set](../../../inverse-problem.md#indicator-functional-of-a-constraint-set) for $C$. The squared fidelity is [strictly convex](../../../real-analysis.md#strictly-convex-function) and coercive, so the primal [minimizer](../../../analysis.md#global-minimizer) exists and is unique.

The [convex projection](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) in this formula is the removed component $g-u_*$, not generally $u_*$ itself. A metric [convex projection](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) onto one fixed closed [convex set](../../../mathematical-optimization.md#convex-set) is idempotent. On a [right singular vector](../../../linear-algebra.md#right-singular-vector) direction with positive singular value of any nonzero $A$, this denoising map reduces to [soft thresholding](../../../probability-and-statistics.md#soft-thresholding) with a positive threshold, and applying it twice shrinks again. It therefore cannot be such a [convex projection](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) for all data. This qualifies the printed [convex projection](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) wording while giving the required [global gradient-norm projection residual](../../../inverse-problem.md#global-gradient-norm-projection-residual).

Compute $P_Cg$ by solving the convex dual least-squares problem

$$
\min_{p\in B_\alpha}f(p),\qquad
f(p)=\frac12\|g-A^*p\|^2.
$$

Its [gradient](../../../calculus.md#gradient) is $\nabla f(p)=A(A^*p-g)$ and has [Lipschitz constant](../../../real-analysis.md#lipschitz-constant) $L=\|A\|^2$. [Projected gradient descent](../../../convex-optimization.md#projected-gradient-descent) gives

$$
\boxed{p^{n+1}=P_{B_\alpha}\big[p^n+\tau A(g-A^*p^n)\big],\qquad
P_{B_\alpha}(r)=\frac{r}{\max(1,\|r\|_2/\alpha)}.}
$$

For fixed $0<\tau<2/L$, the finite-dimensional projected-gradient convergence theorem ensures that $p^n$ converges to a dual [minimizer](../../../analysis.md#global-minimizer). Reconstruct $u^n=g-A^*p^n$; its limit is the unique primal solution even if dual [minimizers](../../../analysis.md#global-minimizer) are nonunique. If $A=0$, the primal solution is simply $g$ and no iteration is needed. For unit-grid forward differences with periodic or zero-difference boundaries, $\|A\|^2\leq8$, so $0<\tau<1/4$ is sufficient. Grid-spacing factors or other boundary stencils change this bound.

The normalization here is global. If a pixelwise sum of [gradient](../../../calculus.md#gradient) lengths had instead been intended, the dual feasible set would be a product of pixelwise balls and [convex projection](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) would normalize each block separately; it is a different regularizer and should not be silently substituted.

For the [discrete Hessian-norm denoising](../../../inverse-problem.md#discrete-hessian-norm-denoising) variant, write $H=\nabla^2:X\to X^4$ and use

$$
\boxed{C_H=H^*\{p\in X^4:\|p\|_2\leq\alpha\},\qquad
u_*=g-P_{C_H}g.}
$$

This is again a compact convex [image signal](../../../computer-science.md#image-signal) of a Euclidean ball, now under the second-difference adjoint. In suitable conventions $H^*$ is a discrete double divergence, but its exact boundary adjoint is what defines the set. It lies in $(\ker H)^\perp$, so components in $\ker H$ are preserved by denoising. Interior second [derivatives](../../../calculus.md#derivative) annihilate affine [image signals](../../../computer-science.md#image-signal); whether all such [image signals](../../../computer-science.md#image-signal) remain in the kernel depends on the boundary convention. With a pixelwise Hessian [norm](../../../functional-analysis.md#norm), the corresponding balls would instead be four-component blocks.

## 3

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A rigorous [Mumford–Shah functional](../../../computer-science.md#mumford-shah-functional) permits nonsmooth [image signals](../../../computer-science.md#image-signal) and free discontinuities. One classical admissible class consists of relatively closed countably rectifiable sets $K\subset\Omega$ with finite [Hausdorff measure](../../../measure-theory.md#hausdorff-measure) $\mathcal H^1(K)$, and $u\in W^{1,2}(\Omega\setminus K)\cap L^\infty(\Omega)$ with finite energy. No exterior boundary values are prescribed. For an existence argument, use the equivalent relaxed class

$$
\mathcal A=\{u\in SBV(\Omega):|u|\leq M,\ \nabla u\in L^2(\Omega),\
\mathcal H^1(J_u)<\infty\},\qquad M=\|g\|_\infty.
$$

A [special bounded-variation space](../../../inverse-problem.md#special-bounded-variation-space) excludes the [Cantor part of a bounded-variation derivative](../../../inverse-problem.md#cantor-part-of-a-bounded-variation-derivative) of the [derivative](../../../calculus.md#derivative): $Du=\nabla u\,dx+[u]\nu_u\mathcal H^1\!\lfloor J_u$. The [jump set of a bounded-variation function](../../../inverse-problem.md#jump-set-of-a-bounded-variation-function) $J_u$ is the relaxed [image edge](../../../computer-science.md#image-edge) set. Clipping to $[-M,M]$ decreases squared fidelity, does not increase the [gradient](../../../calculus.md#gradient) term, and does not create jumps, so this bound loses no [minimizers](../../../analysis.md#global-minimizer).

Take a [minimizing sequence](../../../calculus-of-variations.md#minimizing-sequence) and compare with a constant [image signal](../../../computer-science.md#image-signal). Its $L^2$ [gradient](../../../calculus.md#gradient) [norms](../../../functional-analysis.md#norm) and jump lengths are bounded. Also

$$
|Du_j|(\Omega)\leq|\Omega|^{1/2}\|\nabla u_j\|_2
+2M\mathcal H^1(J_{u_j}),
$$

so the sequence is bounded in $BV$. The [SBV compactness theorem](../../../inverse-problem.md#sbv-compactness-theorem) for bounded values, superlinear [gradient](../../../calculus.md#gradient) growth and bounded jump [measure](../../../measure-theory.md#measure) yields an $L^1$ limit in $SBV$, [weak convergence](../../../weak-topology.md#weak-convergence) of [gradients](../../../calculus.md#gradient) in $L^2$, and [lower semicontinuity](../../../calculus.md#lower-semicontinuity) of both the Dirichlet term and the jump [measure](../../../measure-theory.md#measure). The uniform value bound upgrades convergence to $L^2$, so fidelity converges. This proves **existence of a relaxed [minimizer](../../../analysis.md#global-minimizer)**. [Essential closedness of Mumford–Shah jump sets](../../../computer-science.md#essential-closedness-of-mumford-shah-jump-sets) then supplies a relatively closed representative $K=\overline{J_u}\cap\Omega$, without added length, and $u\in W^{1,2}(\Omega\setminus K)$. This completes the outline for the classical pair problem. Arbitrary Hausdorff convergence of [image edge](../../../computer-science.md#image-edge) sets alone is not an adequate substitute for these [compactness](../../../topology.md#compact-space) and regularity results. No uniqueness is claimed for segmentation.

As $\alpha\to\infty$ with $\beta$ fixed, bounded energy forces $\nabla u\to0$ in $L^2$. The reduced [piecewise-constant Mumford–Shah problem](../../../computer-science.md#piecewise-constant-mumford-shah-problem) is

$$
\boxed{\min_{u\in SBV,\,\nabla u=0}\left\{
\int_\Omega(u-g)^2dx+\beta\mathcal H^1(J_u)\right\}.}
$$

Equivalently, use a [Caccioppoli partition](../../../inverse-problem.md#caccioppoli-partition) $\{E_i\}$ of the [image signal](../../../computer-science.md#image-signal) domain and constants $c_i$:

$$
\min_{\{E_i\},\{c_i\}}\left\{
\sum_i\int_{E_i}(c_i-g)^2dx+\frac\beta2\sum_i\operatorname{Per}(E_i;\Omega)\right\}.
$$

The relative perimeter counts only interior boundaries, and the factor one half counts each interface once. Adjacent equal-valued regions can be merged, removing unnecessary boundaries.

For fixed $K$, let $E_i$ be its positive-area regions. Minimization over $u$ reduces to independent scalar least-squares fits:

$$
\boxed{c_i=\frac1{|E_i|}\int_{E_i}g\,dx.}
$$

The minimized fidelity is $\int_\Omega g^2-\sum_i(\int_{E_i}g)^2/|E_i|$. Thus [region means in piecewise-constant segmentation](../../../computer-science.md#region-means-in-piecewise-constant-segmentation) give the optimal grey values for a fixed segmentation.

For a fixed full spatial function $u$, the [image edge](../../../computer-science.md#image-edge) set must contain its jumps; any extra curve only adds length. The optimal choice is its essential jump set, with a relatively closed representative when appropriate. There is no independent relocation of boundaries while that full function is held fixed. A different common alternating step fixes the values $c_i$ but allows the labels $E_i$ to move. It minimizes the fidelity-plus-perimeter partition [functional](../../../calculus-of-variations.md#functional) above. Without the perimeter term each point takes its nearest grey value; with it, interface length is penalized. At a smooth interface between two labels, outward normal displacement of $E_i$ has first variation

$$
\int_\Gamma\left[(c_i-g)^2-(c_j-g)^2+\beta\kappa\right]V\,ds,
$$

where $\kappa=\operatorname{div}_\Gamma\nu_i$ is positive for an outward normal to a circle. The stationary [segmentation interface curvature balance](../../../computer-science.md#segmentation-interface-curvature-balance) is

$$
\boxed{\beta\kappa=(c_j-g)^2-(c_i-g)^2.}
$$

This is the geometric interpretation of optimizing boundaries with fixed grey levels, and distinguishes it from fixing the whole spatial [image signal](../../../computer-science.md#image-signal).

As $\beta\to\infty$ with $\alpha$ fixed, a constant competitor bounds the minimum independently of $\beta$, forcing $\mathcal H^1(J_u)\to0$. [compactness](../../../topology.md#compact-space) in the relaxed formulation leaves no jump or [Cantor part of a bounded-variation derivative](../../../inverse-problem.md#cantor-part-of-a-bounded-variation-derivative), so the limit is in $W^{1,2}(\Omega)$ on the connected rectangle. The reduced [edge-free Mumford–Shah limit](../../../computer-science.md#edge-free-mumford-shah-limit) is

$$
\boxed{\min_{u\in H^1(\Omega)}\left\{
\int_\Omega(u-g)^2dx+\alpha\int_\Omega|\nabla u|^2dx\right\}.}
$$

A set of zero length can be omitted; this does not impose a zero [image signal](../../../computer-science.md#image-signal) or a Dirichlet boundary value. Comparison with any fixed $H^1$ competitor and [lower semicontinuity](../../../calculus.md#lower-semicontinuity) justify the limit minimization.

For completeness, the [bilinear form](../../../linear-algebra.md#bilinear-form) $B(u,v)=\int uv+\alpha\int\nabla u\cdot\nabla v$ on $H^1(\Omega)$ is continuous and coercive, with $B(u,u)\geq\min(1,\alpha)\|u\|_{H^1}^2$. The right-hand side $\int gv$ is bounded because $g\in L^2$ on the bounded rectangle. The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) gives a unique $u$ satisfying

$$
\int_\Omega uv+\alpha\int_\Omega\nabla u\cdot\nabla v=\int_\Omega gv
\quad(v\in H^1(\Omega)).
$$

It is the unique [minimizer](../../../analysis.md#global-minimizer) by strict convexity. Formally,

$$
\boxed{u-\alpha\Delta u=g\quad\hbox{in }\Omega,\qquad
\partial_\nu u=0\quad\hbox{on }\partial\Omega,}
$$

with the Neumann condition understood through this weak formulation. Equivalently, subtracting the weak equation shows that the energy increase at $u+v$ is $\|v\|_2^2+\alpha\|\nabla v\|_2^2>0$ for nonzero $v$.

## 4

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

In [diffusion image processing](../../../computer-science.md#diffusion-image-processing), the observed grey-value [image signal](../../../computer-science.md#image-signal) $g$ is the initial condition for an evolution $u(x,t)$; time controls the [image smoothing](../../../computer-science.md#image-smoothing) scale. A useful model must suppress [image noise](../../../computer-science.md#image-noise) while respecting the [image signal](../../../computer-science.md#image-signal)'s geometric boundaries. Unless exterior values are intended, use periodic boundaries or [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition), so the filter does not lose intensity through the [image signal](../../../computer-science.md#image-signal) border.

The basic linear model is the [heat equation](../../../diffusion-equation.md#heat-equation), $u_t=\Delta u$, $u(0)=g$. On the whole plane,

$$
\boxed{u(\cdot,t)=G_t*g,\qquad
G_t(x)=\frac1{4\pi t}e^{-|x|^2/(4t)}.}
$$

It is Gaussian [image smoothing](../../../computer-science.md#image-smoothing) with variance $2t$ in each coordinate. In Fourier variables, $\widehat u(\xi,t)=e^{-t|\xi|^2}\widehat g(\xi)$: high spatial frequencies are damped most strongly. Under zero-flux or periodic boundaries the mean is conserved, the maximum principle keeps values within the initial range, and

$$
\frac d{dt}\frac12\int_\Omega(u-\bar u)^2dx=-\int_\Omega|\nabla u|^2dx\leq0.
$$

These give stable [image noise](../../../computer-science.md#image-noise) suppression, but a sharp step also contains high frequencies and is blurred across a width of order $\sqrt t$. Constant diffusivity has no mechanism for distinguishing [image noise](../../../computer-science.md#image-noise) from an [image edge](../../../computer-science.md#image-edge).

Linear sharpening by the backward [heat equation](../../../diffusion-equation.md#heat-equation) would multiply Fourier modes by $e^{t|\xi|^2}$ and amplify arbitrarily fine [image noise](../../../computer-science.md#image-noise) without bound. It is an ill-posed initial-value problem. A controlled [unsharp masking](../../../computer-science.md#unsharp-masking) step instead uses $g+\lambda(g-G_t*g)$, with multiplier $1+\lambda(1-e^{-t|\xi|^2})$. This amplifies high frequencies by at most $1+\lambda$; it can improve apparent contrast but also amplifies [image noise](../../../computer-science.md#image-noise) and cannot reliably restore information already lost by [image smoothing](../../../computer-science.md#image-smoothing).

Nonlinear models use [image signal](../../../computer-science.md#image-signal) structure to select the diffusion. A gradient-based energy and its formal $L^2$ [gradient flow](../../../analysis.md#gradient-flow) are

$$
E(u)=\int_\Omega\Psi(|\nabla u|)dx+\frac\lambda2\int_\Omega(u-g)^2dx,
\qquad
u_t=\operatorname{div}\big(c(|\nabla u|)\nabla u\big)-\lambda(u-g),
\quad c(s)=\frac{\Psi'(s)}s.
$$

For a smooth solution with the corresponding zero-flux condition, $dE/dt=-\int u_t^2\leq0$. The fidelity term prevents indefinite drift towards a constant reconstruction; pure diffusion is usually stopped at a selected finite time.

The local [principal diffusion coefficients](../../../diffusion-equation.md#principal-diffusion-coefficients) distinguish suppression of diffusion from backward diffusion. Where $s=|\nabla u|>0$, the flux [derivative](../../../calculus.md#derivative) is

$$
c(s)I+\frac{c'(s)}s\nabla u\otimes\nabla u.
$$

Its coefficient along an [image signal](../../../computer-science.md#image-signal) level curve is $c(s)$; across that curve it is $c(s)+sc'(s)=\Psi''(s)$. Forward parabolic behavior requires both coefficients nonnegative, with strict positive lower bounds giving uniform parabolicity. Merely choosing $c>0$ and decreasing does not establish well-posedness.

For a convex area-type penalty $\Psi(s)=\sqrt{\varepsilon^2+s^2}$, the coefficients are

$$
c(s)=\frac1{\sqrt{\varepsilon^2+s^2}},\qquad
c(s)+sc'(s)=\frac{\varepsilon^2}{(\varepsilon^2+s^2)^{3/2}}>0.
$$

Diffusion across steep [image edges](../../../computer-science.md#image-edge) is weak but remains forward. As $\varepsilon\to0$, the [total variation flow](../../../inverse-problem.md#total-variation-flow) formally becomes $u_t=\operatorname{div}(\nabla u/|\nabla u|)$. Its convex [subgradient](../../../real-analysis.md#subgradient) formulation handles flat regions and discontinuities. It favors piecewise constant [image signals](../../../computer-science.md#image-signal) and preserves sharp transitions better than Gaussian [image smoothing](../../../computer-science.md#image-smoothing), but can produce [staircasing in total variation denoising](../../../inverse-problem.md#staircasing-in-total-variation-denoising), shrink small objects and move boundaries by [curvature](../../../differential-geometry.md#curvature). [image edge](../../../computer-science.md#image-edge) preservation does not mean exact preservation of all [image edge](../../../computer-science.md#image-edge) locations or amplitudes.

The [Perona-Malik equation](../../../diffusion-equation.md#perona-malik-equation) takes a decreasing diffusivity such as $c(s)=1/(1+s^2/\kappa^2)$. Small [gradients](../../../calculus.md#gradient) are smoothed strongly, while large [gradients](../../../calculus.md#gradient) have weak flux. More precisely,

$$
\boxed{c(s)+sc'(s)=\frac{1-s^2/\kappa^2}{(1+s^2/\kappa^2)^2}.}
$$

For $s>\kappa$, diffusion in the [gradient](../../../calculus.md#gradient) direction is backward, so a strong transition can steepen. This gives formal [image edge](../../../computer-science.md#image-edge) enhancement but also causes instability and continuum [ill-posedness](../../../partial-differential-equation.md#ill-posed-problem). The exponential choice $c(s)=e^{-s^2/\kappa^2}$ similarly has a negative normal coefficient for $s>\kappa/\sqrt2$. Discrete results depend on the stencil, step size and implicit regularization; appealing visual results are not a proof of a well-posed PDE.

A [regularized Perona-Malik diffusion](../../../diffusion-equation.md#regularized-perona-malik-diffusion) computes the conductance from a smoothed [image signal](../../../computer-science.md#image-signal), for example

$$
u_t=\operatorname{div}\big(c(|\nabla(G_\sigma*u)|)\nabla u\big).
$$

The flux still acts on $u$, but the [image edge](../../../computer-science.md#image-edge) detector is less sensitive to raw [image noise](../../../computer-science.md#image-noise). With a smooth kernel and a positive conductance bounded away from zero on the attained range, the local principal diffusion is forward; appropriate regularity and boundary assumptions give a well-posed nonlocal parabolic model. The exact regularization and fixed [image smoothing](../../../computer-science.md#image-smoothing) scale are part of the model.

A genuinely directional filter uses a [diffusion tensor for image filtering](../../../computer-science.md#diffusion-tensor-for-image-filtering):

$$
u_t=\operatorname{div}(D\nabla u),\qquad
D=a_n e_ne_n^T+a_t e_te_t^T,\quad 0<a_n\ll a_t.
$$

Here $e_n$ estimates the [image edge](../../../computer-science.md#image-edge) normal and $e_t$ its tangent. A [structure tensor](../../../computer-science.md#structure-tensor) $J_\rho=G_\rho*(\nabla u_\sigma\nabla u_\sigma^T)$ provides robust directions at a second averaging scale. Strong tangent diffusion smooths [image noise](../../../computer-science.md#image-noise) along an [image edge](../../../computer-science.md#image-edge), while weak normal diffusion reduces mixing across it. Related coherence-enhancing choices connect elongated features along their dominant orientation. Positive tensor [eigenvalues](../../../linear-operator-theory.md#eigenvalue) preserve forward parabolicity; this type of enhancement must be distinguished from Perona–Malik's backward normal diffusion.

For more direct sharpening, a [shock filter for image enhancement](../../../computer-science.md#shock-filter-for-image-enhancement) formally evolves $u_t=-\operatorname{sign}(\Delta u)|\nabla u|$. It is a Hamilton–Jacobi-type transport mechanism, not a positive diffusion operator, and steepens transitions around inflection boundaries. In practice it can be combined with regularized forward diffusion to control [image noise](../../../computer-science.md#image-noise). Any enhancement method needs a scale or stopping rule and an honest treatment of [image noise](../../../computer-science.md#image-noise) amplification.

**Linear heat flow offers predictable [image smoothing](../../../computer-science.md#image-smoothing) but blurs [image edges](../../../computer-science.md#image-edge); convex nonlinear diffusion can preserve them; backward or shock mechanisms sharpen them at a greater stability cost.** [Gradient](../../../calculus.md#gradient) thresholds, conductance regularization and positive tensor directions determine which of these behaviors a proposed filter actually has.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
