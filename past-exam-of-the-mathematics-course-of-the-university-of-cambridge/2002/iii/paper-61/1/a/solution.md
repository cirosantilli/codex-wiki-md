<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret convergence in $C[0,1]$ as [uniform convergence](../../../../../../uniform-convergence.md), and work first with real [continuous functions](../../../../../../continuous-function.md). Set $e_{n,j}=U_n(p_j)-p_j$, for $j=0,1,2$, and put $M=\|f\|_\infty$. The given barriers have one $\gamma\ge0$ independent of both $t$ and $n$. A [positive linear operator on continuous functions](../../../../../../positive-linear-operator-on-continuous-functions.md) preserves non-strict inequalities, so application of $U_n$ and evaluation at $t$ give

$$
\left|U_nf(t)-f(t)U_n1(t)\right|\le\varepsilon U_n1(t)+\gamma U_n((\cdot-t)^2)(t).
$$

Strict pointwise inequalities need not remain strict under a positive operator; non-strict ones suffice. Linearity and the cancellation of the exact moments yield

$$
U_n((\cdot-t)^2)(t)=e_{n,2}(t)-2t e_{n,1}(t)+t^2e_{n,0}(t)\ge0.
$$

Subtracting $f(t)$ rather than $f(t)U_n1(t)$ therefore gives the [quadratic barrier estimate for positive approximation operators](../../../../../../quadratic-barrier-estimate-for-positive-approximation-operators.md):

$$
\|U_nf-f\|_\infty\le\varepsilon\bigl(1+\|e_{n,0}\|_\infty\bigr)+M\|e_{n,0}\|_\infty+\gamma\bigl(\|e_{n,2}\|_\infty+2\|e_{n,1}\|_\infty+\|e_{n,0}\|_\infty\bigr).
$$

For fixed $\varepsilon$, all three moment errors tend uniformly to zero. Thus $\limsup_n\|U_nf-f\|_\infty\le\varepsilon$. Since $\varepsilon$ was arbitrary,

$$
\boxed{\|U_nf-f\|_\infty\longrightarrow0.}
$$

This completes the [Korovkin theorem](../../../../../../korovkin-theorem.md) proof. Complex-valued functions follow by applying the real result to real and imaginary parts. [Uniform convergence](../../../../../../uniform-convergence.md) of the three test functions is essential to this uniform conclusion; purely pointwise test convergence should not be silently substituted.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
