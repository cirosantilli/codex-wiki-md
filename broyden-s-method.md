<h1 id="broyden-s-method">Broyden's method</h1>

↑ **Parent:** [Newton root-finding iteration](newton-root-finding-iteration.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Broyden's_method)

A secant-updating method for a vector equation $F(x)=0$, named for [Charles George Broyden](charles-george-broyden.md). Solve $B_kd_k=-F(x_k)$, choose $x_{k+1}=x_k+\alpha_kd_k$, and form $s_k=x_{k+1}-x_k$, $y_k=F(x_{k+1})-F(x_k)$. For a nonzero step the displayed “good Broyden” update satisfies $B_{k+1}s_k=y_k$, learning the [Jacobian matrix](jacobian-matrix.md) action along the observed step rather than evaluating a new full [Jacobian matrix](jacobian-matrix.md).

The update also has a least-change characterization in the [Frobenius norm](frobenius-norm.md). Write $u=y_k-B_ks_k$. Any correction $E$ satisfying $Es_k=u$ has squared row norms bounded below by $u_i^2/\|s_k\|^2$, by the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md). Summing these bounds gives $\|E\|_F^2\ge\|u\|^2/\|s_k\|^2$, with equality for $E=us_k^{\mathsf T}/\|s_k\|^2$. This proves the rank-one correction is the least-change update satisfying the secant constraint. [Superlinear convergence](superlinear-convergence.md) needs local regularity and suitable initialization; it is not a global consequence of this algebraic identity.[pp. 577–581, motivation and Jacobian-updating construction.](a-class-of-methods-for-solving-nonlinear-simultaneous-equations-by-charles-george-broyden.md)

## ↑ Ancestors (6)

1. [Newton root-finding iteration](newton-root-finding-iteration.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Charles George Broyden](charles-george-broyden.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/discrete-mathematics-probability-and-continuous-mathematics/5/c/ii/solution.md)
- [Quasi-Newton Methods by NEOS Guide](quasi-newton-methods-by-neos-guide.md)
