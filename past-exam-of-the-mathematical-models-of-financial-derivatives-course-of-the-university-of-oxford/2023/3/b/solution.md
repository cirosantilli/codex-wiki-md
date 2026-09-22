<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the [Itô product rule](../../../../ito-product-rule.md) with deterministic [integrating factor](../../../../integrating-factor.md) $e^{\alpha u}$:

$$
d(e^{\alpha u}x_u)=\alpha\widetilde\mu e^{\alpha u}du+\sigma e^{\alpha u}dZ_u.
$$

Integrate from $t$ to $T$ and multiply by $e^{-\alpha T}$ to obtain

$$
\boxed{x_T=x_t e^{-\alpha(T-t)}+\widetilde\mu(1-e^{-\alpha(T-t)})+\sigma e^{-\alpha T}\int_t^T e^{\alpha u}\,dZ_u}.
$$

This is the explicit solution behind the [Ornstein-Uhlenbeck transition distribution](../../../../ornstein-uhlenbeck-transition-distribution.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
