<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

First verify that $V_0$ is a [vector space](../../../../../vector-space-split.md). Sums and scalar multiples preserve [continuity](../../../../../continuous-function.md) and the condition at zero. For every [partition of an interval](../../../../../partition-of-an-interval.md) $D$, the [triangle inequality](../../../../../triangle-inequality.md) and [absolute homogeneity of a norm](../../../../../absolute-homogeneity-of-a-norm.md) of the [absolute value](../../../../../absolute-value.md) imply

$$
V(f+g,D)\leq V(f,D)+V(g,D),\qquad V(\lambda f,D)=|\lambda|V(f,D).
$$

Taking [suprema](../../../../../supremum.md) yields

$$
V(f+g)\leq V(f)+V(g),\qquad V(\lambda f)=|\lambda|V(f).
$$

For $\lambda=0$ the second equality follows directly from $V(0)=0$. In particular, [finite variation](../../../../../total-variation-of-a-function.md) is preserved, so $V_0$ is closed under these operations.

Nonnegativity is immediate. For any $t\in[0,1]$, use the [partition of an interval](../../../../../partition-of-an-interval.md) $(0,t,1)$, omitting repeated endpoints if necessary, to get

$$
|f(t)|=|f(t)-f(0)|\leq V(f).
$$

Thus $V(f)=0$ forces $f=0$, and conversely $f=0$ has zero [total variation of a function](../../../../../total-variation-of-a-function.md). These observations prove that $\|f\|=V(f)$ is a [norm](../../../../../norm.md) on $V_0$.

Applying the same bound to $f_n-f$ gives

$$
\boxed{\|f_n-f\|_\infty\leq V(f_n-f)=\|f_n-f\|.}
$$

Therefore convergence in the [anchored variation norm](../../../../../anchored-variation-norm.md) implies [uniform convergence](../../../../../uniform-convergence.md) on $[0,1]$. The anchoring condition $f(0)=0$ removes the nonzero constant [functions](../../../../../function-split.md) which otherwise have zero [total variation of a function](../../../../../total-variation-of-a-function.md).

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [a](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
