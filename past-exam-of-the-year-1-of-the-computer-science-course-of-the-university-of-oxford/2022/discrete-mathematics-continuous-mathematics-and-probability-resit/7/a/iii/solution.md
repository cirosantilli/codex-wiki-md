<h1 id="7/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Interpret existence of the [expectations](../../../../../../expected-value-split.md) as finite [expected values](../../../../../../expected-value-split.md), equivalently $\mathbb E|X|<\infty$ and $\mathbb E|Y|<\infty$. First justify the summations rather than assuming that a signed double series can be rearranged. [Independence](../../../../../../independent-random-variables.md) and [Tonelli theorem](../../../../../../tonelli-theorem.md) give

$$
\sum_{x,y}|xy|p_{X,Y}(x,y)=\sum_{x,y}|x|p_X(x)|y|p_Y(y)=\mathbb E|X|\,\mathbb E|Y|<\infty.
$$

Consequently $XY$ is an [integrable random variable](../../../../../../integrable-random-variable.md), and [Fubini theorem](../../../../../../fubini-s-theorem.md) permits summing the signed terms in either order:

$$
\mathbb E[XY]=\sum_x\sum_yxy\,p_X(x)p_Y(y)=\left(\sum_xxp_X(x)\right)\left(\sum_yyp_Y(y)\right)=\boxed{\mathbb E[X]\mathbb E[Y].}
$$

If extended infinite [expectations](../../../../../../expected-value-split.md) are allowed instead, the phrase “exist” needs additional care: expressions such as $0\cdot\infty$ do not define an [expectation](../../../../../../expected-value-split.md). The finite-[expectation](../../../../../../expected-value-split.md) convention avoids that ambiguity.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
