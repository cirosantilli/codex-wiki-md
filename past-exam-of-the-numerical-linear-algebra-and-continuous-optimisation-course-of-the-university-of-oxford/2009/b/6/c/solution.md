<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On the strictly feasible set $\Omega^\circ_c=\{x:c_j(x)>0\text{ for all }j\}$, use the [logarithmic barrier](../../../../../logarithmic-barrier.md)

$$
\boxed{\Phi_\mu(x)=f(x)-\mu\sum_{j=1}^M\log c_j(x),\qquad\mu>0.}
$$

Choose a strictly feasible starting point and parameters $\mu_n\downarrow0$. For each parameter minimize the barrier functional by an unconstrained method confined to $\Omega^\circ_c$, warm-starting from the preceding point. In the exact version take a stationary point $x_n$ of the barrier subproblem. The stationarity equation is

$$
\nabla f(x_n)-\sum_j\lambda_{n,j}\nabla c_j(x_n)=0,\qquad\boxed{\lambda_{n,j}=\mu_n/c_j(x_n)>0,\quad\lambda_{n,j}c_j(x_n)=\mu_n.}
$$

These are the natural [Lagrange multiplier](../../../../../lagrange-multiplier.md) estimates; the basic method need not perform a separate primal-dual correction.

The [barrier method KKT convergence theorem](../../../../../barrier-method-kkt-convergence-theorem.md) is a global stationarity result: if the exact barrier stationary points form a bounded sequence, then every cluster point satisfying the [linear independence constraint qualification](../../../../../linear-independence-constraint-qualification.md) is a [KKT point](../../../../../kkt-point.md). To prove it, take any subsequence $x_n\to x_*$. Continuity gives feasibility of $x_*$. For an inactive index, $c_j(x_*)>0$ and therefore $\lambda_{n,j}=\mu_n/c_j(x_n)\to0$.

The active gradients at $x_*$ are independent. The supplied dual-basis result gives bounded vectors $\varphi_{n,i}$, converging as $n\to\infty$, with $\nabla c_j(x_n)^T\varphi_{n,i}=\delta_{ji}$ for active $i,j$. Pair stationarity with these vectors:

$$
\lambda_{n,i}=\varphi_{n,i}^T\left(\nabla f(x_n)-\sum_{j\notin\mathcal A(x_*)}\lambda_{n,j}\nabla c_j(x_n)\right).
$$

Thus all active multipliers are bounded as well. Extract a convergent multiplier subsequence. Its limit is nonnegative, satisfies stationarity by continuity, and satisfies complementarity because $\lambda_{n,j}c_j(x_n)=\mu_n\to0$. This proves the claimed KKT conclusion. The same proof permits approximate barrier stationary points whose stationarity residual tends to zero. Bounded iterates and the constraint qualification are substantive hypotheses, not automatic consequences of writing a barrier functional.

For a global-minimum conclusion one needs global minimization of the barrier subproblems and appropriate access to every feasible point. Specifically, suppose $x_n$ globally minimizes $\Phi_{\mu_n}$, has a cluster point $x_*$, and $\overline{\Omega^\circ_c}=\Omega$. For any fixed strictly feasible $z$,

$$
f(x_n)\leq f(z)+\mu_n\sum_j\bigl(\log c_j(x_n)-\log c_j(z)\bigr).
$$

Along the convergent subsequence the $c_j(x_n)$ are bounded above, so taking the upper limit gives $f(x_*)\leq f(z)$. Density of strictly feasible points and continuity of $f$ extend the inequality to every feasible $z$. Hence $x_*$ is a global minimizer under these stronger hypotheses.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
