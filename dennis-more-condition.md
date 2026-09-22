<h1 id="dennis-more-condition">Dennis-Moré condition</h1>

↑ **Parent:** [Quasi-Newton method](quasi-newton-method.md)

For a convergent [quasi-Newton method](quasi-newton-method.md) sequence $x_k\to x_*$ with $\nabla f(x_*)=0$, nonsingular $H_*=\nabla^2f(x_*)$, and continuous Hessian nearby, the displayed condition implies q-[superlinear convergence](superlinear-convergence.md). Here $B_ks_k=-\nabla f(x_k)$ and $s_k=x_{k+1}-x_k$. The condition requires Hessian accuracy only along the actual steps, rather than convergence of the full matrix approximations. It is associated with [John E. Dennis](john-e-dennis.md) and [Jorge Moré](jorge-more.md).

Indeed, the first-order expansion of the [gradient](gradient.md) gives $\nabla f(x_{k+1})=-(B_k-H_*)s_k+o(\|s_k\|)=o(\|s_k\|)$. Nonsingularity of $H_*$ gives $\|x-x_*\|\leq C\|\nabla f(x)\|$ locally. Consequently $\|e_{k+1}\|\leq\varepsilon_k(\|e_k\|+\|e_{k+1}\|)$ with $\varepsilon_k\to0$. Rearrangement proves $\|e_{k+1}\|/\|e_k\|\to0$. Finite termination is understood separately from ratios with zero denominators.

## ↑ Ancestors (6)

1. [Quasi-Newton method](quasi-newton-method.md)
2. [Newton's method in optimization](newton-s-method-in-optimization.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Gauss-Newton algorithm](gauss-newton-algorithm.md)
- [John E. Dennis](john-e-dennis.md)
- [Jorge Moré](jorge-more.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2009/b/5/b/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2009/b/5/c/solution.md)
