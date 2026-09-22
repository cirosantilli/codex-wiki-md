<h1 id="18h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Newton's method for minimization uses

$$
\boxed{x_{k+1}=x_k-[\nabla^2f(x_k)]^{-1}\nabla f(x_k)}.
$$

For a quantitative local bound, suppose on a convex neighbourhood containing the iterates that

$$
mI\preceq\nabla^2f(x)\preceq LI,
\qquad
\|\nabla^2f(x)-\nabla^2f(y)\|\leq M\|x-y\|,
$$

with $m>0$, and let $x^*$ be the minimizer. The [integral](../../../../../../integral.md) form of the [gradient](../../../../../../gradient.md) and the Hessian Lipschitz bound give the [quadratic convergence bound for Newton's method](../../../../../../quadratic-convergence-bound-for-newton-s-method.md)

$$
\|x_{k+1}-x^*\|
\leq\frac M{2m}\|x_k-x^*\|^2.
$$

If $q=M\|x_0-x^*\|/(2m)<1$, induction yields

$$
\|x_k-x^*\|\leq\frac{2m}{M}q^{2^k}.
$$

Since $f(x)-f(x^*)\leq L\|x-x^*\|^2/2$,

$$
\boxed{f(x_k)-f(x^*)
\leq\frac{2Lm^2}{M^2}q^{2^{k+1}}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
