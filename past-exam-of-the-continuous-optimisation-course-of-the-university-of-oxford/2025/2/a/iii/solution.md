<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Cauchy point](../../../../../cauchy-point.md) provides both an inexpensive fallback step and a standard against which a better step can be judged. Requiring a fixed [fraction of Cauchy decrease](../../../../../fraction-of-cauchy-decrease.md) gives

$$
m_k(0)-m_k(s_k)\geq\frac\kappa2\|\nabla f(x^k)\|\min\{\Delta_k,\|\nabla f(x^k)\|/\|H_k\|\},\qquad\kappa>0.
$$

Consequently an exact [global minimum](../../../../../global-minimum.md) of each [trust-region subproblem](../../../../../trust-region-subproblem.md) is unnecessary. A step from any inner solver is adequate if it meets this bound.

The convergence argument combines this decrease with model accuracy. For example, suppose the [gradient](../../../../../gradient.md) is uniformly [Lipschitz continuous](../../../../../lipschitz-continuity.md) on a neighborhood of the visited [level set](../../../../../level-set.md), the model [Hessian matrices](../../../../../hessian-matrix.md) are uniformly bounded, and the usual acceptance and radius safeguards are used. If $\|\nabla f(x^k)\|\geq\epsilon>0$, the [Taylor expansion](../../../../../taylor-expansion.md) gives a model error bounded by $K\|s_k\|^2$. For sufficiently small $\Delta_k$, division by the [Cauchy decrease bound](../../../../../cauchy-decrease-bound.md) makes $|1-\rho_k|$ small. Such trials are successful and cannot keep shrinking the radius. With the [gradient](../../../../../gradient.md) bounded away from zero, the radius therefore has a positive lower bound, and each accepted step decreases $f$ by a fixed positive amount. There must be infinitely many accepted steps, since repeated rejection would force the radius below the small-radius acceptance threshold. This contradicts boundedness below of $f$ and proves $\liminf_k\|\nabla f(x^k)\|=0$.

Stronger standard conclusions can be obtained with further regularity and safeguards. Merely being twice [continuously differentiable](../../../../../continuously-differentiable-function.md) and bounded below does not supply uniform [Hessian](../../../../../hessian-matrix.md) bounds on an unbounded [level set](../../../../../level-set.md); those uniform assumptions must be stated when using this argument.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Continuous optimisation course of the University of Oxford](../../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
