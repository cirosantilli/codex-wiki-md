<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With zero cost for correct assignments, the total expected misclassification cost is

$$
L(R_1)=c(2\mid1)\pi_1\int_{R_1^c}f_1+
 c(1\mid2)\pi_2\int_{R_1}f_2.
$$

The part depending on $R_1$ is the integral of $c(1\mid2)\pi_2f_2-c(2\mid1)\pi_1f_1$. Therefore the [cost-sensitive Bayes classifier](../../../../../../../cost-sensitive-bayes-classifier.md) is

$$
\boxed{\text{choose class one when }
 c(2\mid1)\pi_1f_1(x)>c(1\mid2)\pi_2f_2(x).}
$$

For positive costs and weighted densities, the log posterior-odds score from part (ii) now has threshold $\log(c(1\mid2)/c(2\mid1))$. Larger cost of sending class one to class two expands the region assigned to class one. The weighted-density comparison also handles zero costs without taking an undefined logarithm.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
