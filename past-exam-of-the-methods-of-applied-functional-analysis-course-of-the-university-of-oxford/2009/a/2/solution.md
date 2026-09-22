<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [coercive Neumann energy with a positive reaction term](../../../../coercive-neumann-energy-with-a-positive-reaction-term.md), let $\nu>0$ be the ellipticity constant and $A_0=\max_{i,j}\|a_{ij}\|_\infty$. [Cauchy-Schwarz](../../../../cauchy-schwarz-inequality.md) gives

$$
|B[u,v]|\le nA_0\|\nabla u\|_2\|\nabla v\|_2+\|c\|_\infty\|u\|_2\|v\|_2
\le C\|u\|_{H^1}\|v\|_{H^1}.
$$

Bilinearity follows from the [integral](../../../../integral-split.md) and weak-derivative [linearity](../../../../linearity.md). Ellipticity and the strictly positive zeroth-order coefficient give

$$
\boxed{B[u,u]\ge\nu\|\nabla u\|_2^2+\mu\|u\|_2^2\ge\kappa\|u\|_{H^1}^2,\quad\kappa=\min(\nu,\mu)>0.}
$$

This controls constants as well as [gradients](../../../../gradient.md), so no zero-mean constraint or [Neumann](../../../../neumann-boundary-condition.md) compatibility condition is required. Symmetry of the coefficients makes $B$ symmetric.

Write $F(v)=\int_\Omega fv$. This is a [bounded linear functional](../../../../continuous-linear-functional.md) on $H^1$, with $|F(v)|\le\|f\|_2\|v\|_{H^1}$. Consequently

$$
I(v)\ge\frac\kappa2\|v\|_{H^1}^2-\|f\|_2\|v\|_{H^1}\longrightarrow+\infty
$$

as the [norm](../../../../norm.md) tends to [infinity](../../../../infinity.md). The infimum is finite, and every [minimizing sequence](../../../../minimizing-sequence.md) is [bounded](../../../../boundedness.md). The [Hilbert space](../../../../hilbert-space-split.md) $H^1$ is reflexive, so a minimizing [subsequence](../../../../subsequence.md) converges [weakly](../../../../weak-convergence.md) to some $u\in H^1$.

To verify lower semicontinuity directly, put $w_j=v_j-u$. Boundedness of $B$ makes $B[u,w_j]\to0$ under [weak convergence](../../../../weak-convergence.md), and symmetry gives

$$
B[v_j,v_j]=B[u,u]+2B[u,w_j]+B[w_j,w_j]\ge B[u,u]+o(1).
$$

Also $F(v_j)\to F(u)$. Therefore $I(u)\le\liminf I(v_j)$, so **the absolute minimum is attained**.

For every $h\in H^1$ the real [function](../../../../function-split.md) $t\mapsto I(u+th)$ has a minimum at zero. Its [derivative](../../../../derivative.md) there is $B[u,h]-F(h)$, yielding the required weak equation for every $h$. If two [weak solutions](../../../../weak-solution.md) exist, their difference $z$ satisfies $B[z,h]=0$ for all $h$; choose $h=z$ and use coercivity to obtain $z=0$. In fact the weak equation also gives the exact energy identity

$$
\boxed{I(v)-I(u)=\tfrac12B[v-u,v-u]\ge\tfrac\kappa2\|v-u\|_{H^1}^2.}
$$

Thus the [minimizer](../../../../global-minimizer.md) and [weak solution](../../../../weak-solution.md) are both unique. The natural [boundary condition](../../../../boundary-condition.md) is encoded by testing in the whole $H^1$ space, without needing [pointwise](../../../../pointwise-convergence.md) [conormal derivatives](../../../../conormal-flux-of-a-divergence-form-operator.md) for rough coefficients.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../split.md)
5. [Methods of applied functional analysis course of the University of Oxford](../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
