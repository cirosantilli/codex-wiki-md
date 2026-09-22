<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Linearity and $\|Tf\|_\infty\leq2\pi\|f\|_\infty$ show that the [integral](../../../../integral-split.md) defines a [bounded linear operator](../../../../continuous-linear-operator.md). Inductively,

$$
\boxed{|T^kf(t)|\leq\frac{t^k}{k!}\|f\|_\infty\qquad(0\leq t\leq2\pi).}
$$

For $k=0$ this is immediate. If it holds for $k$, then $|\sin s|\leq1$ gives $|T^{k+1}f(t)|\leq\int_0^t s^k\|f\|_\infty/k!\,ds$, which proves the next case. Thus $\|T^k\|\leq(2\pi)^k/k!$.

For every $\lambda\ne0$, the [series](../../../../series-mathematics.md) $A_\lambda=\sum_{k\geq0}\lambda^{-k-1}T^k$ converges in [operator norm](../../../../operator-norm.md), dominated by $|\lambda|^{-1}e^{2\pi/|\lambda|}$. Multiplying its [partial sums](../../../../partial-sum.md) by $\lambda I-T$ on either side gives the identity minus a remainder $\lambda^{-N-1}T^{N+1}$, which tends to zero by the factorial estimate. Therefore $A_\lambda$ is the bounded inverse of $\lambda I-T$.

Finally every function in the [image](../../../../image-of-a-function.md) of $T$ vanishes at zero, so $T$ is not onto the [continuous functions](../../../../continuous-function.md). Hence $0$ belongs to its [spectrum](../../../../spectrum-functional-analysis.md) and

$$
\boxed{\sigma(T)=\{0\}.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
