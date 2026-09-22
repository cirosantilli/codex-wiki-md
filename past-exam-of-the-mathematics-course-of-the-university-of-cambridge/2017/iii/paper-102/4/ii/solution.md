<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take an integer $k\geq0$, so $k\rho$ is a [dominant integral weight](../../../../../../dominant-integral-weight.md). Apply the dilation $e^\mu\mapsto e^{(k+1)\mu}$ to the [Weyl denominator formula](../../../../../../weyl-denominator-formula.md):

$$
\sum_{w\in W}\det(w)e^{(k+1)w\rho}
=e^{(k+1)\rho}\prod_{\alpha\in R^+}(1-e^{-(k+1)\alpha}).
$$

This is exactly the numerator of the [Weyl character formula](../../../../../../weyl-character-formula.md) for $L(k\rho)$. Divide by its denominator and use a finite [geometric series](../../../../../../geometric-series.md) in each root direction:

$$
\boxed{\operatorname{ch}L(k\rho)
=e^{k\rho}\prod_{\alpha\in R^+}
\frac{1-e^{-(k+1)\alpha}}{1-e^{-\alpha}}
=e^{k\rho}\prod_{\alpha\in R^+}(1+e^{-\alpha}+\cdots+e^{-k\alpha}).}
$$

This [character of a Weyl-vector multiple](../../../../../../character-of-a-weyl-vector-multiple.md) also gives $\dim L(k\rho)=(k+1)^{|R^+|}$ by evaluating every formal exponential at one. This evaluation is safe in the final polynomial expression, without dividing by a zero denominator.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
