<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the [minimum-integral decision region](../../../../../../../minimum-integral-decision-region.md) principle to $g(x)=\pi_2f_2(x)-\pi_1f_1(x)$. The optimal [Bayes classifier](../../../../../../../bayes-classifier.md) chooses class one when $\pi_1f_1(x)>\pi_2f_2(x)$, and class two for the reverse inequality. Ties can be assigned either way. An everywhere valid discriminant score is

$$
\boxed{\delta(x)=\pi_1f_1(x)-\pi_2f_2(x),\qquad\text{choose class one if }\delta(x)>0.}
$$

Where both weighted densities are positive one may equivalently use $\log(\pi_1f_1(x)/(\pi_2f_2(x)))$ and threshold zero. This chooses the largest posterior class probability, because both posterior probabilities have the same positive mixture-density denominator.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
