<h1 id="8/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $I_c$ be the [indicator random variable](../../../../../../indicator-random-variable.md) that colour $c$ appears at least once. Then $X=I_R+I_B+I_G$. For a colour of single-roll probability $p_c$, independence of rolls gives $\mathbb P(I_c=0)=(1-p_c)^n$. By [linearity of expectation](../../../../../../linearity-of-expectation.md),

$$
\boxed{\mathbb E X=\sum_c\bigl(1-(1-p_c)^n\bigr)=3-\left(\frac12\right)^n-\left(\frac23\right)^n-\left(\frac56\right)^n.}
$$

The three indicators are not independent, but [linearity of expectation](../../../../../../linearity-of-expectation.md) does not require them to be. This is the [expected number of observed categories](../../../../../../expected-number-of-observed-categories.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
