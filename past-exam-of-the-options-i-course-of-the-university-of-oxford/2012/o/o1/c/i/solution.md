<h1 id="o/o1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the stated [geometric distribution](../../../../../../geometric-distribution.md), write $S=\sum_iX_i$. Then

$$
\ell_n(\theta)=n\log\theta+(S-n)\log(1-\theta),
\qquad
-\ell_n''(\theta)=\frac n{\theta^2}+\frac{S-n}{(1-\theta)^2}.
$$

Since $\mathbb E X_i=1/\theta$, we have $\mathbb E(S-n)=n(1-\theta)/\theta$. Taking [expectation](../../../../../../expected-value-split.md) gives the sample [Fisher information](../../../../../../fisher-information-matrix.md)

$$
I_n(\theta)=\frac n{\theta^2}+\frac n{\theta(1-\theta)}
=\boxed{\frac n{\theta^2(1-\theta)}}.
$$

The support begins at one, so this [expectation](../../../../../../expected-value-split.md) uses the trials-until-first-success convention of the geometric law.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [O1](../../../o1.md)
4. [O](../../../../o.md)
5. [2012](../../../../../2012-split.md)
6. [Past exam of the options I course of the University of Oxford](../../../../../split.md)
7. [Options I course of the University of Oxford](../../../../../../options-i-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
