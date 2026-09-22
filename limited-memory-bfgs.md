# Limited-memory BFGS

↑ **Parent:** [BFGS method](bfgs-method.md)

Limited-memory BFGS is a [quasi-Newton method](quasi-newton-method.md) that applies an inverse-[Hessian matrix](hessian-matrix.md) approximation without storing a dense square [matrix](matrix.md). It retains only a fixed number $\ell$ of recent secant pairs $s_k=x_{k+1}-x_k$ and $y_k=\nabla f(x_{k+1})-\nabla f(x_k)$. The standard two-loop recursion computes the search direction using $O(\ell d)$ storage and arithmetic in dimension $d$.

With a positive-definite initial metric and safeguarded curvature updates, the step is $x_{k+1}=x_k-\alpha_kH_k\nabla f(x_k)$, with $\alpha_k$ chosen by a [line search](line-search.md). It is useful when full-memory [BFGS](bfgs-method.md) would require too much storage. Fixed-memory convergence results typically give [linear convergence](linear-convergence.md) under strong [convexity](convex-function.md), bounded metric and suitable [line search](line-search.md) assumptions; one must not automatically transfer the full-memory superlinear theorem. In a nonconvex problem, a local method does not by itself certify a [global minimum](global-minimum.md).[Final two paragraphs: inverse-Hessian products from stored secant [vectors](vector.md) and limited-memory implementations](quasi-newton-methods-by-neos-guide.md)

## ↑ Ancestors (7)

1. [BFGS method](bfgs-method.md)
2. [Quasi-Newton method](quasi-newton-method.md)
3. [Newton's method in optimization](newton-s-method-in-optimization.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability/6/c/iv/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/6/b/ii/solution.md)
