# Smooth convex approximation proof of the Tanaka formula

↑ **Parent:** [Tanaka's formula](tanaka-s-formula.md)

Choose $f_n(0)=0$ and $f_n'(x)=\phi(nx)$, where $\phi$ is continuously differentiable, nondecreasing, equal to $-1$ on $(-\infty,0]$ and $1$ on $[1,\infty)$. Then $f_n''\geq0$ and $0\leq|x|-f_n(x)\leq2/n$. For $X=M+A$ with continuous adapted finite-variation $A$, the [Itô isometry](ito-isometry.md) and [Doob L2 maximal inequality](doob-l2-maximal-inequality.md) give local uniform convergence in probability of the martingale integrals. Dominated convergence against the total-variation measure gives pathwise uniform convergence of the drift integrals. The nondecreasing corrections $\frac12\int f_n''(X)d[M]$ therefore converge locally uniformly in probability to $|X|-\int\operatorname{sgn}_-(X)dX$. A subsequence on one probability-one event shows that the limit is continuous and nondecreasing. Localization removes the deterministic bounds used in the argument.

## ↑ Ancestors (9)

1. [Tanaka's formula](tanaka-s-formula.md)
2. [Itô's lemma](ito-s-lemma.md)
3. [Stochastic calculus](stochastic-calculus-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29/2/c/solution.md)
- [Right local time of a continuous semimartingale](right-local-time-of-a-continuous-semimartingale.md)
