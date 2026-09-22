<h1 id="s/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Draw independent uniforms $U_1,U_2$ on $(0,1)$, put $V=2U_1-1$, and accept $V$ if $U_2\leq\sqrt{1-V^2}$; otherwise repeat independently. This is [rejection sampling](../../../../../rejection-sampling.md) from the uniform proposal $q(v)=1/2$. Its accepted unnormalized density is $q(v)\sqrt{1-v^2}$, and the acceptance probability is

$$
a=\frac12\int_{-1}^1\sqrt{1-v^2}\,dv=\frac\pi4.
$$

Dividing by $a$ gives the target [Wigner semicircle distribution](../../../../../wigner-semicircle-distribution.md). The number of trials up to and including the first acceptance has a [geometric distribution](../../../../../geometric-distribution.md) with success probability $\pi/4$, so

$$
\boxed{\mathbb E[N]=\frac4\pi.}
$$

The expected number of rejected trials alone is $4/\pi-1$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [S](../../../s.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
