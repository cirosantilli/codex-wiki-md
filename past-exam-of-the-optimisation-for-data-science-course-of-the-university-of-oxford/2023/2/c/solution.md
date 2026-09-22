<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**There is a summation-index misprint.** On the native PDF, paper page 3, equation (4) has $X^k$ inside a sum indexed by $j$. The intended telescoping estimate has $X^j$ inside that sum; this is the estimate proved below and used in part (d). The index mismatch is present in the original PDF, rather than being introduced by the transcription.

Take the [expectation](../../../../expected-value-split.md) of the supplied [conditional expectation](../../../../conditional-expectation.md) bound (3), using the [tower property](../../../../law-of-total-expectation.md):

$$
\mathbb E f(X^{j+1})\leq\mathbb E f(X^j)-\frac1{2L}\mathbb E\|\nabla f(X^j)\|^2+\frac M{2L}.
$$

Rearranging and forming a [telescoping sum](../../../../telescoping-sum.md) gives

$$
\frac1{2L}\sum_{j=0}^{k-1}\mathbb E\|\nabla f(X^j)\|^2
\leq f(x^0)-\mathbb E f(X^k)+\frac{kM}{2L}.
$$

Because $x^*$ is a [global minimizer](../../../../global-minimizer.md), $f(X^k)\geq f(x^*)$ for every realisation. Hence the corrected equation (4) is

$$
\boxed{\sum_{j=0}^{k-1}\frac1{2L}\mathbb E\|\nabla f(X^j)\|^2\leq f(x^0)-f(x^*)+\frac{kM}{2L}.}
$$

All [expectations](../../../../expected-value-split.md) at a finite iteration are finite here: a deterministic starting point and finitely many choices of the sampled index produce only finitely many possible iterates. **The bound controls accumulated squared gradients**, with an additive contribution from the [stochastic gradient noise floor](../../../../stochastic-gradient-noise-floor.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
