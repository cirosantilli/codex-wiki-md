<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A rigorous [Mumford–Shah functional](../../../../../mumford-shah-functional.md) permits nonsmooth [image signals](../../../../../image-signal.md) and free discontinuities. One classical admissible class consists of relatively closed countably rectifiable sets $K\subset\Omega$ with finite [Hausdorff measure](../../../../../hausdorff-measure.md) $\mathcal H^1(K)$, and $u\in W^{1,2}(\Omega\setminus K)\cap L^\infty(\Omega)$ with finite energy. No exterior boundary values are prescribed. For an existence argument, use the equivalent relaxed class

$$
\mathcal A=\{u\in SBV(\Omega):|u|\leq M,\ \nabla u\in L^2(\Omega),\
\mathcal H^1(J_u)<\infty\},\qquad M=\|g\|_\infty.
$$

A [special bounded-variation space](../../../../../special-bounded-variation-space.md) excludes the [Cantor part of a bounded-variation derivative](../../../../../cantor-part-of-a-bounded-variation-derivative.md) of the [derivative](../../../../../derivative.md): $Du=\nabla u\,dx+[u]\nu_u\mathcal H^1\!\lfloor J_u$. The [jump set of a bounded-variation function](../../../../../jump-set-of-a-bounded-variation-function.md) $J_u$ is the relaxed [image edge](../../../../../image-edge.md) set. Clipping to $[-M,M]$ decreases squared fidelity, does not increase the [gradient](../../../../../gradient.md) term, and does not create jumps, so this bound loses no [minimizers](../../../../../global-minimizer.md).

Take a [minimizing sequence](../../../../../minimizing-sequence.md) and compare with a constant [image signal](../../../../../image-signal.md). Its $L^2$ [gradient](../../../../../gradient.md) [norms](../../../../../norm.md) and jump lengths are bounded. Also

$$
|Du_j|(\Omega)\leq|\Omega|^{1/2}\|\nabla u_j\|_2
+2M\mathcal H^1(J_{u_j}),
$$

so the sequence is bounded in $BV$. The [SBV compactness theorem](../../../../../sbv-compactness-theorem.md) for bounded values, superlinear [gradient](../../../../../gradient.md) growth and bounded jump [measure](../../../../../measure.md) yields an $L^1$ limit in $SBV$, [weak convergence](../../../../../weak-convergence.md) of [gradients](../../../../../gradient.md) in $L^2$, and [lower semicontinuity](../../../../../lower-semicontinuity.md) of both the Dirichlet term and the jump [measure](../../../../../measure.md). The uniform value bound upgrades convergence to $L^2$, so fidelity converges. This proves **existence of a relaxed [minimizer](../../../../../global-minimizer.md)**. [Essential closedness of Mumford–Shah jump sets](../../../../../essential-closedness-of-mumford-shah-jump-sets.md) then supplies a relatively closed representative $K=\overline{J_u}\cap\Omega$, without added length, and $u\in W^{1,2}(\Omega\setminus K)$. This completes the outline for the classical pair problem. Arbitrary Hausdorff convergence of [image edge](../../../../../image-edge.md) sets alone is not an adequate substitute for these [compactness](../../../../../compact-space.md) and regularity results. No uniqueness is claimed for segmentation.

As $\alpha\to\infty$ with $\beta$ fixed, bounded energy forces $\nabla u\to0$ in $L^2$. The reduced [piecewise-constant Mumford–Shah problem](../../../../../piecewise-constant-mumford-shah-problem.md) is

$$
\boxed{\min_{u\in SBV,\,\nabla u=0}\left\{
\int_\Omega(u-g)^2dx+\beta\mathcal H^1(J_u)\right\}.}
$$

Equivalently, use a [Caccioppoli partition](../../../../../caccioppoli-partition.md) $\{E_i\}$ of the [image signal](../../../../../image-signal.md) domain and constants $c_i$:

$$
\min_{\{E_i\},\{c_i\}}\left\{
\sum_i\int_{E_i}(c_i-g)^2dx+\frac\beta2\sum_i\operatorname{Per}(E_i;\Omega)\right\}.
$$

The relative perimeter counts only interior boundaries, and the factor one half counts each interface once. Adjacent equal-valued regions can be merged, removing unnecessary boundaries.

For fixed $K$, let $E_i$ be its positive-area regions. Minimization over $u$ reduces to independent scalar least-squares fits:

$$
\boxed{c_i=\frac1{|E_i|}\int_{E_i}g\,dx.}
$$

The minimized fidelity is $\int_\Omega g^2-\sum_i(\int_{E_i}g)^2/|E_i|$. Thus [region means in piecewise-constant segmentation](../../../../../region-means-in-piecewise-constant-segmentation.md) give the optimal grey values for a fixed segmentation.

For a fixed full spatial function $u$, the [image edge](../../../../../image-edge.md) set must contain its jumps; any extra curve only adds length. The optimal choice is its essential jump set, with a relatively closed representative when appropriate. There is no independent relocation of boundaries while that full function is held fixed. A different common alternating step fixes the values $c_i$ but allows the labels $E_i$ to move. It minimizes the fidelity-plus-perimeter partition [functional](../../../../../functional.md) above. Without the perimeter term each point takes its nearest grey value; with it, interface length is penalized. At a smooth interface between two labels, outward normal displacement of $E_i$ has first variation

$$
\int_\Gamma\left[(c_i-g)^2-(c_j-g)^2+\beta\kappa\right]V\,ds,
$$

where $\kappa=\operatorname{div}_\Gamma\nu_i$ is positive for an outward normal to a circle. The stationary [segmentation interface curvature balance](../../../../../segmentation-interface-curvature-balance.md) is

$$
\boxed{\beta\kappa=(c_j-g)^2-(c_i-g)^2.}
$$

This is the geometric interpretation of optimizing boundaries with fixed grey levels, and distinguishes it from fixing the whole spatial [image signal](../../../../../image-signal.md).

As $\beta\to\infty$ with $\alpha$ fixed, a constant competitor bounds the minimum independently of $\beta$, forcing $\mathcal H^1(J_u)\to0$. [compactness](../../../../../compact-space.md) in the relaxed formulation leaves no jump or [Cantor part of a bounded-variation derivative](../../../../../cantor-part-of-a-bounded-variation-derivative.md), so the limit is in $W^{1,2}(\Omega)$ on the connected rectangle. The reduced [edge-free Mumford–Shah limit](../../../../../edge-free-mumford-shah-limit.md) is

$$
\boxed{\min_{u\in H^1(\Omega)}\left\{
\int_\Omega(u-g)^2dx+\alpha\int_\Omega|\nabla u|^2dx\right\}.}
$$

A set of zero length can be omitted; this does not impose a zero [image signal](../../../../../image-signal.md) or a Dirichlet boundary value. Comparison with any fixed $H^1$ competitor and [lower semicontinuity](../../../../../lower-semicontinuity.md) justify the limit minimization.

For completeness, the [bilinear form](../../../../../bilinear-form.md) $B(u,v)=\int uv+\alpha\int\nabla u\cdot\nabla v$ on $H^1(\Omega)$ is continuous and coercive, with $B(u,u)\geq\min(1,\alpha)\|u\|_{H^1}^2$. The right-hand side $\int gv$ is bounded because $g\in L^2$ on the bounded rectangle. The [Lax-Milgram theorem](../../../../../lax-milgram-theorem.md) gives a unique $u$ satisfying

$$
\int_\Omega uv+\alpha\int_\Omega\nabla u\cdot\nabla v=\int_\Omega gv
\quad(v\in H^1(\Omega)).
$$

It is the unique [minimizer](../../../../../global-minimizer.md) by strict convexity. Formally,

$$
\boxed{u-\alpha\Delta u=g\quad\hbox{in }\Omega,\qquad
\partial_\nu u=0\quad\hbox{on }\partial\Omega,}
$$

with the Neumann condition understood through this weak formulation. Equivalently, subtracting the weak equation shows that the energy increase at $u+v$ is $\|v\|_2^2+\alpha\|\nabla v\|_2^2>0$ for nonzero $v$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
