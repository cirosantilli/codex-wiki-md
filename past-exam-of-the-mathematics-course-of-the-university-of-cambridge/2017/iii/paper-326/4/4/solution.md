<h1 id="4/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the standard inverse-problem setting of a bounded linear $K:\ell^2\to\ell^2$ and exact data having a finite-penalty solution. Let $u^\dagger$ denote the unique $J$-minimizing exact solution for $J(u)=\|u\|_1+\beta\|u\|_2^2$, $\beta>0$. This is the limiting target of [elastic net regularization in Hilbert sequence space](../../../../../../elastic-net-regularization-in-hilbert-sequence-space.md); it need not be the Moore–Penrose minimum-norm solution unless additional hypotheses identify them, for example injectivity of $K$.

For each $\alpha>0$, the reconstruction objective is weakly lower semicontinuous, coercive by $\alpha\beta\|u\|_2^2$, and [strictly convex](../../../../../../strictly-convex-function.md). The direct method on the reflexive [l2 sequence space](../../../../../../l2-sequence-space.md) gives existence, and strict convexity gives uniqueness. For two data sets, monotonicity of the one-norm [subgradients](../../../../../../subgradient.md) and the quadratic penalty give, with $d=u_1-u_2$ and $g=f_1-f_2$,

$$
\|Kd\|^2+2\alpha\beta\|d\|^2\leq\langle g,Kd\rangle\leq\|g\|\|Kd\|.
$$

Completing the square yields $\|d\|\leq\|g\|/(2\sqrt{2\alpha\beta})$, so each reconstruction map is continuous.

Minimality against $u^\dagger$ gives

$$
\frac12\|Ku_\alpha^\delta-f^\delta\|^2+\alpha J(u_\alpha^\delta)\leq\frac{\delta^2}{2}+\alpha J(u^\dagger).
$$

Choose $\alpha\to0$ and $\delta^2/\alpha\to0$, for example $\alpha=\delta$. This bounds the Hilbert norms, drives the data residual to zero and gives $\limsup J(u_\alpha^\delta)\leq J(u^\dagger)$. Every [weakly convergent](../../../../../../weak-convergence.md) subsequence has an exact solution as its limit, by boundedness of $K$; [weak lower semicontinuity](../../../../../../weak-lower-semicontinuity.md) and uniqueness of the penalty minimizer identify that limit with $u^\dagger$. Separately applying [weak lower semicontinuity](../../../../../../weak-lower-semicontinuity.md) to the one-norm gives

$$
\limsup\beta\|u_\alpha^\delta\|_2^2\leq J(u^\dagger)-\|u^\dagger\|_1=\beta\|u^\dagger\|_2^2.
$$

[Weak convergence](../../../../../../weak-convergence.md) and convergence of Hilbert norms imply [strong convergence](../../../../../../norm-convergence.md) by the [Radon-Riesz theorem](../../../../../../radon-riesz-theorem.md). This proves [norm convergence of elastic net regularization](../../../../../../norm-convergence-of-elastic-net-regularization.md):

$$
\boxed{u_\alpha^\delta\to u^\dagger\text{ in }\ell^2,\qquad\alpha\to0,\quad\delta^2/\alpha\to0.}
$$

The argument applies to every [sequence](../../../../../../sequence.md) of noise levels and admissible data, hence gives the usual uniform noise-ball convergence for a fixed admissible exact datum.

For [nonlinearity of elastic net reconstruction](../../../../../../nonlinearity-of-elastic-net-reconstruction.md), zero is the minimizer exactly when $\|K^*f^\delta\|_\infty\leq\alpha$. This includes a neighborhood of zero. If $K\ne0$, choose $e_j$ with $Ke_j\ne0$ and $f^\delta=tKe_j$ for $t\|Ke_j\|^2>\alpha$; zero then fails its optimality condition. A linear map vanishing on a neighborhood would vanish everywhere, so **the elastic-net reconstruction is nonlinear whenever $K\ne0$**. For $K=I$ the explicit formula is $[R_\alpha f]_j=\operatorname{sign}(f_j)(|f_j|-\alpha)_+/(1+2\alpha\beta)$, exhibiting [soft thresholding](../../../../../../soft-thresholding.md).

A concrete distinction from Moore–Penrose convergence is $K(u)=u_1+2u_2$ (embedded in the first output coordinate of $\ell^2$), exact datum one, and $\beta=1$. Its minimum-norm solution is $(1/5,2/5,0,\ldots)$, with penalty $4/5$, while the unique penalty-minimizing exact solution is $(0,1/2,0,\ldots)$, with penalty $3/4$. For $0<\alpha<2$ the exact-data elastic-net reconstruction is $(0,(2-\alpha)/(4+2\alpha),0,\ldots)$, converging to the latter. Thus it is not a Moore–Penrose-consistent regularization for every noninjective operator under the earlier definition.

The PDF supplies neither a nonzero assumption on $K$ nor a target/domain qualification here. Its unconditional nonlinearity claim is false for $K=0$, whose reconstruction is the zero linear map. The convergence proof above states the finite-penalty exact-solution hypotheses explicitly; it establishes convergence to the penalty-minimizing solution, not an automatically identical [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md).

## ↑ Ancestors (11)

1. [4](../4.md)
2. [4](../../4.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
