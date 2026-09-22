<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\mathbf z=(x,y)^T$, $r^2=\mathbf z^T\mathbf z$ and $f=\sqrt{1+r^2}$. The [chain rule](../../../../../chain-rule.md) yields

$$
\boxed{\nabla f=\frac{\mathbf z}{f},\qquad H_f=\frac I f-\frac{\mathbf z\mathbf z^T}{f^3}=\frac1{f^3}\begin{pmatrix}1+y^2&-xy\\-xy&1+x^2\end{pmatrix}.}
$$

For every nonzero [vector](../../../../../vector.md) $\mathbf v$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
\mathbf v^TH_f\mathbf v=\frac{(1+r^2)\|\mathbf v\|^2-(\mathbf z^T\mathbf v)^2}{f^3}\geq\frac{\|\mathbf v\|^2}{f^3}>0.
$$

Thus the [Hessian](../../../../../hessian-matrix.md) is a [positive-definite matrix](../../../../../positive-definite-matrix.md) everywhere. The [Hessian criterion for convexity](../../../../../hessian-criterion-for-convexity.md) implies that **$f$ is strictly [convex](../../../../../convex-function.md) on $\mathbb R^2$**. Its unique global [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md) is at $\mathbf z=0$, where $f=1$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics, and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
