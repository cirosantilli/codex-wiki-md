<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Expand the two observations in order using the [chain rule for mutual information](../../../../../chain-rule-for-mutual-information.md):

$$
I(X,Y;Z)=I(X;Z)+I(Y;Z\mid X).
$$

The remaining [conditional mutual information](../../../../../conditional-mutual-information.md) is

$$
I(Y;Z\mid X)=\sum_xp_X(x)D\!\left(p_{Y,Z\mid x}\,\middle\|\,p_{Y\mid x}p_{Z\mid x}\right)\geq0.
$$

[Relative entropy nonnegativity](../../../../../relative-entropy-nonnegativity.md) proves the inequality. Equality requires every positive-weight [relative entropy](../../../../../kullback-leibler-divergence.md) to vanish, which is equivalent to $p(y,z\mid x)=p(y\mid x)p(z\mid x)$ for every $x$ of positive [probability](../../../../../probability.md). Thus **equality holds exactly when $Y$ and $Z$ have [conditional independence](../../../../../conditional-independence.md) given $X$.** No unconditional [independence](../../../../../independent-random-variables.md) is required.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
