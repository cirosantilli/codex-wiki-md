<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Condition on $X^k=x$, and set $r=x-x^*$, $g=\nabla f(x)$ and $h=\nabla f_{S_k}(x)$. Since the sampled index is independent of $X^k$ and has the [discrete uniform distribution](../../../../discrete-uniform-distribution.md), $h$ is an [unbiased stochastic gradient](../../../../unbiased-stochastic-gradient.md):

$$
\mathbb E[h\mid X^k=x]=\frac1m\sum_{i=1}^m\nabla f_i(x)=g.
$$

Write $\sigma_k^2=\mathbb E[\|h-g\|^2\mid X^k=x]\leq M$. Expanding $h=g+(h-g)$ and using the zero conditional mean of $h-g$ proves the [stochastic gradient second-moment identity](../../../../stochastic-gradient-second-moment-identity.md)

$$
\mathbb E[\|h\|^2\mid X^k=x]=\|g\|^2+\sigma_k^2.
$$

The [stochastic gradient descent](../../../../stochastic-gradient-descent.md) update is $X^{k+1}=x-h/L$. Expanding the squared [Euclidean distance](../../../../euclidean-distance.md) and using the preceding identities gives

$$
D_k:=\frac L2\mathbb E\left[\|X^k-x^*\|^2-\|X^{k+1}-x^*\|^2\,\middle|\,X^k=x\right]
=g^Tr-\frac1{2L}(\|g\|^2+\sigma_k^2).
$$

The [subgradient inequality](../../../../subgradient-inequality.md) for the [differentiable](../../../../differentiable-function.md) [convex function](../../../../convex-function.md) $f$ gives $f(x)-f(x^*)\leq g^Tr$. Combining this with (3),

$$
\begin{aligned}
\mathbb E[f(X^{k+1})\mid X^k=x]
&\leq f(x)-\frac1{2L}\|g\|^2+\frac M{2L}\\
&\leq f(x^*)+g^Tr-\frac1{2L}\|g\|^2+\frac M{2L}\\
&=f(x^*)+D_k+\frac{\sigma_k^2+M}{2L}\\
&\leq f(x^*)+D_k+\frac ML.
\end{aligned}
$$

Removing the temporary notation for the conditioning point yields

$$
\boxed{\mathbb E[f(X^{k+1})\mid X^k]\leq f(x^*)+\frac L2\mathbb E\left[\|X^k-x^*\|^2-\|X^{k+1}-x^*\|^2\,\middle|\,X^k\right]+\frac ML.}
$$

**The noise contributes twice** in this argument: once in the supplied bound (3), and once in converting the expected squared step into the squared [gradient](../../../../gradient.md). Each contribution is at most $M/(2L)$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the optimisation for data science course of the University of Oxford](../../../split.md)
5. [Optimisation for data science course of the University of Oxford](../../../../optimisation-for-data-science-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
