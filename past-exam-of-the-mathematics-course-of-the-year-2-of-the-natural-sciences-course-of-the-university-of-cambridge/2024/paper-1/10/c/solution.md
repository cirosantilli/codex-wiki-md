<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the endpoint condition in its linear [Robin boundary condition](../../../../../robin-boundary-condition.md) form $y'(1)=y(1)/\alpha$. For a positive [eigenvalue](../../../../../eigenvalue.md) $\lambda=q^2$, the left [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) gives $y=C\sin(qx)$, and the right condition gives

$$
q\cos q=\frac1\alpha\sin q,\qquad\boxed{\tan q=\alpha q.}
$$

For each positive root $q_n$, the squared [norm](../../../../../norm.md) is

$$
N_n=\int_0^1\sin^2(q_nx)\,dx=\frac12-\frac{\sin(2q_n)}{4q_n}.
$$

Consequently the sine coefficients in any complete expansion are

$$
\boxed{a_n=\frac{\int_0^1f(x)\sin(q_nx)\,dx}{N_n}=\frac{2\int_0^1f(x)\sin(q_nx)\,dx}{1-\sin(2q_n)/(2q_n)}.}
$$

When $\alpha>1$, these are all modes and the [Sturm-Liouville eigenfunction expansion](../../../../../sturm-liouville-eigenfunction-expansion.md) gives exactly the stated sine series, with the usual convergence interpretation. Positivity of all [eigenvalues](../../../../../eigenvalue.md) follows from [integration by parts](../../../../../integration-by-parts.md) and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md):

$$
\int_0^1y(-y'')dx=\int_0^1(y')^2dx-\frac{y(1)^2}{\alpha}\geq\left(1-\frac1\alpha\right)\int_0^1(y')^2dx>0
$$

for a nonzero admissible $y$, since $y(1)=\int_0^1y'\,dx$.

However, the original PDF states only $\alpha>0$, and with that range its sine-only completeness claim is false. The missing modes are as follows. At $\alpha=1$, $\lambda=0$ admits $y=x$, so the correct expansion is

$$
\boxed{f(x)=3x\int_0^1t f(t)\,dt+\sum_{n\geq1}a_n\sin(q_nx),\qquad\alpha=1.}
$$

For $0<\alpha<1$, a negative [eigenvalue](../../../../../eigenvalue.md) $\lambda=-\kappa^2$ admits $y=\sinh(\kappa x)$, with

$$
\boxed{\tanh\kappa=\alpha\kappa,\qquad\kappa>0.}
$$

There is exactly one positive root: $\tanh\kappa/\kappa$ decreases strictly from $1$ to zero. For example, its [derivative](../../../../../derivative.md) has the sign of $\kappa\operatorname{sech}^2\kappa-\tanh\kappa<0$, because $\sinh\kappa\cosh\kappa>\kappa$. Thus the corrected expansion is

$$
\boxed{f(x)=a_-\sinh(\kappa x)+\sum_{n\geq1}a_n\sin(q_nx),\quad a_-=\frac{\int_0^1f(t)\sinh(\kappa t)\,dt}{\sinh(2\kappa)/(4\kappa)-1/2},\quad0<\alpha<1.}
$$

These are the [nonpositive modes in a Dirichlet-Robin interval expansion](../../../../../nonpositive-modes-in-a-dirichlet-robin-interval-expansion.md). As an explicit counterexample to the printed claim, at $\alpha=1$ take $f(x)=x$: it satisfies both [boundary conditions](../../../../../boundary-condition.md), and each positive root obeys

$$
\int_0^1x\sin(q_nx)\,dx=-\frac{\cos q_n}{q_n}+\frac{\sin q_n}{q_n^2}=0
$$

because $\tan q_n=q_n$. Thus all $a_n$ vanish despite $f\ne0$. Likewise $f=\sinh(\kappa x)$ is a counterexample for $\alpha<1$, by [orthogonality of Sturm-Liouville eigenfunctions](../../../../../orthogonality-of-sturm-liouville-eigenfunctions.md) with distinct [eigenvalues](../../../../../eigenvalue.md). The formulas above give the full solution without silently assuming away the omitted modes.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
