<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [complete-case analysis](../../../../../../complete-case-analysis.md) changes the mix of people contributing to the [logistic regression](../../../../../../logistic-regression.md). Let $A=1$ mean that both required variables are observed, and write $s_c(p,z)=\Pr(A=1\mid C=c,P=p,Z=z)$. Within $P>1$, [Bayes' theorem](../../../../../../bayes-theorem.md) gives

$$
\boxed{\operatorname{logit}\Pr(C=1\mid p,z,A=1)
=\operatorname{logit}\Pr(C=1\mid p,z)+\log\frac{s_1(p,z)}{s_0(p,z)}.}
$$

If completeness depends differently on the two responses, and that selection also varies with partner count or the other predictors, the extra term changes the fitted [regression coefficients](../../../../../../regression-coefficient.md). For example, people with high counts and poor condom use can be under-represented, weakening or otherwise distorting the apparent association. Dropping people with missing $P$ also excludes some whose membership of the $P>1$ target group is unknown.

**The fitted conditional association among complete responders need not equal the target-population association.** No direction of [selection bias](../../../../../../selection-bias.md) follows without specifying the response mechanism. Selection on predictors alone need not bias a correctly specified conditional [logistic regression](../../../../../../logistic-regression.md); it is the outcome-related selection described here that removes that reassurance.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
