<h1 id="5/d/3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [Random-scan Gibbs sampler](../../../../../../../../random-scan-gibbs-sampler.md), the correct [transition kernel](../../../../../../../../markov-kernel.md) is a measure, since a one-coordinate update is singular with respect to full-dimensional [Lebesgue measure](../../../../../../../../lebesgue-measure.md) when $p>1$. Write $x_{-i}$ for all coordinates except $i$. Then

$$
\boxed{P(x,dx')=\frac1p\sum_{i=1}^p\pi_i(x_i'\mid x_{-i})\,dx_i'\prod_{j\ne i}\delta_{x_j}(dx_j').}
$$

Each [Dirac measure](../../../../../../../../dirac-measure.md) fixes an unupdated coordinate. Equivalently, $P(x,A)=p^{-1}\sum_i\int\mathbf1_A(x_{-i},z)\pi_i(z\mid x_{-i})\,dz$, with $z$ placed in coordinate $i$. Replacing this kernel by an ordinary density on the whole product space would omit those fixed-coordinate constraints.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [3](../../3.md)
3. [D](../../../d.md)
4. [5](../../../../5.md)
5. [Paper 37](../../../../../paper-37-split.md)
6. [Iii](../../../../../split.md)
7. [2015](../../../../../../split.md)
8. [Past exam of the mathematics course of the University of Cambridge](../../../../../../../split.md)
9. [Mathematics course of the University of Cambridge](../../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../../split.md)
