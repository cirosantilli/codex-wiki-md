<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**The printed distance needs a square.** The native PDF, paper page 3, prints $\|x^0-x^*\|$ in the final bound, but the general conclusion from (5) contains $\|x^0-x^*\|^2$. We first prove the corrected statement and then show that the printed version can fail.

Take the [expectation](../../../../expected-value-split.md) in (5), use the [tower property](../../../../law-of-total-expectation.md), and sum over $j=0,\ldots,k-1$. The squared [Euclidean distances](../../../../euclidean-distance.md) form a [telescoping sum](../../../../telescoping-sum.md):

$$
\sum_{j=0}^{k-1}\big(\mathbb E f(X^{j+1})-f(x^*)\big)
\leq\frac L2\left(\|x^0-x^*\|^2-\mathbb E\|X^k-x^*\|^2\right)+\frac{kM}{L}.
$$

Discard the final nonnegative squared [Euclidean distance](../../../../euclidean-distance.md). The smallest of $k$ numbers is at most their [arithmetic mean](../../../../arithmetic-mean.md), so

$$
\boxed{\min_{0\leq j<k}\mathbb E f(X^{j+1})-f(x^*)\leq\frac L{2k}\|x^0-x^*\|^2+\frac ML.}
$$

This is an $O(k^{-1})$ bound above the [stochastic gradient noise floor](../../../../stochastic-gradient-noise-floor.md) $M/L$ for the best expected [objective function](../../../../objective-function.md) value. By [Jensen's inequality](../../../../jensen-s-inequality.md), it also bounds $\mathbb E f(\bar X^k)-f(x^*)$ for the averaged iterate $\bar X^k=k^{-1}\sum_{j=0}^{k-1}X^{j+1}$, because $f$ is a [convex function](../../../../convex-function.md).

To test the printed version, take one component function, $f_1(x)=f(x)=x^2/4$, with $L=1$, $x^*=0$ and $x^0=10$. This [convex quadratic function](../../../../convex-quadratic-function.md) has $\nabla f(x)=x/2$, hence it has a $1$-[Lipschitz gradient](../../../../lipschitz-gradient.md). The [stochastic gradient descent](../../../../stochastic-gradient-descent.md) update is deterministic, its conditional [variance](../../../../variance-split.md) is zero, and the assumed positive bound $M=1/10$ is valid. At $k=1$, the new iterate is $X^1=5$, so

$$
f(X^1)-f(x^*)=\frac{25}{4}>5+\frac1{10}
=\frac L2\|x^0-x^*\|+\frac ML.
$$

Thus the printed inequality is false under its stated assumptions. The squared [Euclidean distance](../../../../euclidean-distance.md) in the corrected bound resolves the defect.

## ↑ Ancestors (12)

1. [F](../f.md)
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
