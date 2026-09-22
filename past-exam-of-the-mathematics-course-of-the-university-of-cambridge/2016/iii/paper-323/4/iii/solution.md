<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $|\zeta\rangle=\sum_{i,j}M_{ij}|i\rangle_A|j\rangle_B$. Normalization says $\|M\|_{\rm HS}=1$, and the [Schmidt rank](../../../../../../schmidt-rank.md) equals the [matrix rank](../../../../../../matrix-rank.md) of $M$. Its nonzero [singular values](../../../../../../singular-value.md) are therefore $s_1,\ldots,s_r$ with $\sum_js_j^2=1$.

The overlap with the [maximally entangled state](../../../../../../maximally-entangled-state.md) is $\langle\phi^+|\zeta\rangle=\operatorname{Tr}(M)/\sqrt d$. The [trace norm](../../../../../../trace-norm.md) estimate of Q3(i), with test [linear operator](../../../../../../linear-operator.md) $I$, followed by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), gives

$$
|\operatorname{Tr}M|\leq\|M\|_1=\sum_{j=1}^rs_j\leq\sqrt{r\sum_js_j^2}=\sqrt r.
$$

For two [pure states](../../../../../../pure-state.md), the unsquared [quantum fidelity](../../../../../../fidelity-of-quantum-states.md) is the absolute value of their overlap. **Hence the [maximally entangled overlap bound from Schmidt rank](../../../../../../maximally-entangled-overlap-bound-from-schmidt-rank.md) is**

$$
\boxed{F(|\phi^+\rangle\langle\phi^+|,|\zeta\rangle\langle\zeta|)\leq\sqrt{\frac rd}.}
$$

The bound is attained by $|\zeta\rangle=r^{-1/2}\sum_{j=0}^{r-1}|jj\rangle$. Thus uniform [Schmidt coefficients](../../../../../../schmidt-coefficient.md) on $r$ aligned basis pairs give the greatest possible overlap for that [Schmidt rank](../../../../../../schmidt-rank.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
