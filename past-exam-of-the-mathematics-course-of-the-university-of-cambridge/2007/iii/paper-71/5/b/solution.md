<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose linearly independent basis functions $\phi_1,\ldots,\phi_N$ in the [zero-trace Sobolev space](../../../../../../zero-trace-sobolev-space.md), and put $V_N=\operatorname{span}\{\phi_i\}$. A concrete conforming [Galerkin method](../../../../../../galerkin-method.md) uses continuous piecewise-linear hat functions on an interval mesh, with zero endpoint values. Seek $u_N=\sum_j c_j\phi_j$ satisfying

$$
a(u_N,v_N)=\langle f,v_N\rangle\quad(v_N\in V_N).
$$

Testing against each basis function gives

$$
\boxed{\sum_{j=1}^N K_{ij}c_j=F_i,\qquad K_{ij}=\int_0^1[p\phi_j'\phi_i'+q\phi_j\phi_i]dx,\qquad F_i=\int_0^1f\phi_i\,dx.}
$$

The matrix is symmetric, and for a nonzero coefficient vector $c$, its represented function is nonzero by basis independence. The [coercivity](../../../../../../coercive-function.md) estimate gives $c^TKc=a(u_N,u_N)>0$. Thus $K$ is a [positive-definite matrix](../../../../../../positive-definite-matrix.md), the finite-dimensional problem has a unique solution, and it minimizes the same energy over $V_N$. This is [Ritz-Galerkin equivalence for a symmetric coercive form](../../../../../../ritz-galerkin-equivalence-for-a-symmetric-coercive-form.md).

Subtracting the continuous and discrete equations proves [Galerkin orthogonality](../../../../../../galerkin-orthogonality.md): $a(u-u_N,v_N)=0$ for all $v_N\in V_N$. Let $\|v\|_a=\sqrt{a(v,v)}$. For any comparison $v_N$, orthogonality and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) in this inner product give

$$
\|u-u_N\|_a^2=a(u-u_N,u-v_N)\leq\|u-u_N\|_a\|u-v_N\|_a.
$$

Therefore

$$
\boxed{\|u-u_N\|_a\leq\inf_{v_N\in V_N}\|u-v_N\|_a.}
$$

With $C_a=p_{\max}+q_{\max}/\pi^2$, the same argument in the derivative norm gives the [Céa lemma](../../../../../../cea-s-lemma.md) estimate $\|u-u_N\|_H\leq(C_a/p_{\min})\inf_{v_N\in V_N}\|u-v_N\|_H$.

Convergence now follows from approximation, not from a bare assertion that the residual is small. The defining density of smooth compactly supported functions in $H_0^1$ lets one approximate $u$ by such a smooth function. Its piecewise-linear interpolant has zero endpoints and derivative error tending to zero as the largest mesh interval tends to zero. For a smooth $w$, the derivative on each element is the average of $w'$ there, and the interval [Poincaré inequality](../../../../../../poincare-inequality.md) bounds its error by the element length times $\|w''\|_2$. Density and the boxed best-approximation estimate consequently give $u_N\to u$ in $H_0^1$, and hence in $L^2$, without assuming a bounded derivative of $p$. If the stronger regularity $u\in H^2$ is available, the same interpolation estimate gives first-order convergence in the derivative norm.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
