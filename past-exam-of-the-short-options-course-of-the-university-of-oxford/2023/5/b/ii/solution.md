<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The integral $I$ is the [convolution](../../../../../convolution.md) of the positive-half-line kernels $x^{a-1}$ and $x^{b-1}$. The [convolution theorem for Laplace transforms](../../../../../convolution-theorem-for-laplace-transforms.md) therefore gives, for $p>0$,

$$
\mathcal L I(p)=\Gamma(a)\Gamma(b)p^{-(a+b)}.
$$

On the other hand, the substitution $t=xu$ gives $I(x)=x^{a+b-1}B(a,b)$, where $B(a,b)=\int_0^1u^{a-1}(1-u)^{b-1}\,du$ is the [beta function](../../../../../beta-function.md). Applying part (i) again yields $\mathcal L I(p)=B(a,b)\Gamma(a+b)p^{-(a+b)}$. Comparing the two expressions proves

$$
\boxed{B(a,b)=\frac{\Gamma(a)\Gamma(b)}{\Gamma(a+b)}}.
$$

All integrands used in the real-$p$ convolution argument are nonnegative, so [Tonelli's theorem](../../../../../tonelli-theorem.md) justifies the interchange; the endpoint singularities are integrable because $a,b>0$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
