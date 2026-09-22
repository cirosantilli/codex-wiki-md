# Nonpositive modes in a Dirichlet-Robin interval expansion

↑ **Parent:** [Sturm-Liouville eigenfunction expansion](sturm-liouville-eigenfunction-expansion.md)

For $-y''=\lambda y$, positive [eigenvalues](eigenvalue.md) have [eigenfunctions](eigenfunction.md) $\sin(q_nx)$, where $\tan q_n=\alpha q_n$ and $q_n>0$. Their squared [norms](norm.md) are $N_n=1/2-\sin(2q_n)/(4q_n)$. A zero [eigenvalue](eigenvalue.md) occurs precisely at $\alpha=1$, with [eigenfunction](eigenfunction.md) $x$. A negative [eigenvalue](eigenvalue.md) occurs precisely at $0<\alpha<1$: it is $-\kappa^2$ with [eigenfunction](eigenfunction.md) $\sinh(\kappa x)$, where $\tanh\kappa=\alpha\kappa$. There is exactly one such $\kappa$, since $\tanh\kappa/\kappa$ decreases strictly from $1$ to $0$. The [integration by parts](integration-by-parts.md) identity

$$
\langle y,-y''\rangle=\int_0^1|y'|^2dx-\frac{|y(1)|^2}{\alpha}
$$

and the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) show positivity for $\alpha>1$ and nonnegativity at equality. The complete expansion of a [square-integrable function](square-integrable-function.md) therefore includes the extra term $3x\int_0^1tf(t)dt$ when $\alpha=1$, or $\sinh(\kappa x)\int_0^1f(t)\sinh(\kappa t)dt/[\sinh(2\kappa)/(4\kappa)-1/2]$ when $\alpha<1$, in addition to $\sum_n[\int_0^1f(t)\sin(q_nt)dt/N_n]\sin(q_nx)$. Omitting that extra mode makes the system incomplete. In particular, $f=x$ at $\alpha=1$ is orthogonal to every positive sine mode and is an immediate counterexample to a sine-only expansion.

## ↑ Ancestors (7)

1. [Sturm-Liouville eigenfunction expansion](sturm-liouville-eigenfunction-expansion.md)
2. [Sturm-Liouville problem](sturm-liouville-problem.md)
3. [Sturm-Liouville theory](sturm-liouville-theory-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Dirichlet-Robin eigenvalues on a finite interval](dirichlet-robin-eigenvalues-on-a-finite-interval.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/10/c/solution.md)
