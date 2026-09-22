<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Independence](../../../../../../../independent-random-variables.md) of the centered [standard normal random variables](../../../../../../../standard-normal-random-variable.md) gives $\mathbb E\epsilon_i=0$ for every $i$. Also

$$
\mathbb E\epsilon_1^2=1,\qquad
\mathbb E\epsilon_i^2=\mathbb E\eta_i^2\,\mathbb E\eta_{i-1}^2=1\quad(i\ge2).
$$

For nonadjacent indices, the underlying sets of $\eta$ variables are disjoint, so the errors are [independent](../../../../../../../independent-random-variables.md) and have zero [covariance](../../../../../../../covariance.md). For adjacent indices with $i\ge2$,

$$
\mathbb E[\epsilon_i\epsilon_{i+1}]
=\mathbb E[\eta_{i-1}\eta_i^2\eta_{i+1}]
=\mathbb E\eta_{i-1}\,\mathbb E\eta_i^2\,\mathbb E\eta_{i+1}=0.
$$

The first adjacent pair separately gives $\mathbb E[\epsilon_1\epsilon_2]=\mathbb E[\eta_1^2\eta_2]=0$. Hence

$$
\boxed{\Sigma=I_n.}
$$

These [adjacent products of independent Gaussian variables](../../../../../../../adjacent-products-of-independent-gaussian-variables.md) are [uncorrelated random variables](../../../../../../../uncorrelated-random-variables.md) even though adjacent errors share a factor and are dependent.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
