<h1 id="9/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For any real $y$, put $k=\lfloor y\rfloor$. Since $Y$ is integer-valued,

$$
\{Y\leq y\}=\{\lfloor X\rfloor\leq k\}=\{X<k+1\}.
$$

Continuity of the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) of $X$ therefore gives

$$
\boxed{F_Y(y)=F_X(\lfloor y\rfloor+1)}.
$$

The strict inequality $X<k+1$ matters before using the absence of point masses. The resulting [probability distribution](../../../../../../probability-distribution-split.md) is discrete, with [probability mass function](../../../../../../probability-mass-function.md)

$$
\boxed{\mathbb P(Y=k)=F_X(k+1)-F_X(k)\quad(k\in\mathbb Z)}.
$$

Thus **$Y$ has no ordinary [probability density function](../../../../../../probability-density-function.md)** with respect to length on the real line. Its [cumulative distribution function](../../../../../../cumulative-distribution-function.md) is a step function; its derivative is zero almost everywhere and does not recover its probabilities. The [floor function](../../../../../../floor-function.md) has converted a density into masses on the integers.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
