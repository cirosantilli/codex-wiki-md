<h1 id="continuous-mathematics/4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Minimize the square of the [Euclidean distance](../../../../../../euclidean-distance.md), using [minimizers under strictly increasing transformations](../../../../../../minimizers-under-strictly-increasing-transformations.md). For $s=x+y>0$,

$$
x^2+y^2+\ln^2(x+y)=\frac{s^2}{2}+\frac{(x-y)^2}{2}+\ln^2s.
$$

For fixed $s$ the unique minimum has $x=y=s/2$. Put $x=y=\alpha>0$ and $J(\alpha)=2\alpha^2+\ln^2(2\alpha)$. Its [derivative](../../../../../../derivative.md) is

$$
J'(\alpha)=\frac{2}{\alpha}\left(2\alpha^2+\ln(2\alpha)\right).
$$

Let $h(\alpha)=2\alpha^2+\ln(2\alpha)$. Since $h'(\alpha)=4\alpha+1/\alpha>0$, it is [strictly increasing](../../../../../../strictly-increasing-function.md), with limits $-\infty$ and $+\infty$ at the two ends of $(0,\infty)$. It therefore has exactly one zero. The sign of $J'$ changes there from negative to positive, proving the unique [global minimum](../../../../../../global-minimum.md). The nearest point is **$P=(\alpha,\alpha,\ln(2\alpha))$** at that zero.[Question 4(d), p. 4: the logarithm is interpreted as ln(2α)](../../../../../../discrete-mathematics-continuous-mathematics-and-probability-examination-paper-a10100w1-2022.md)

The [Newton root-finding iteration](../../../../../../newton-root-finding-iteration.md) is

$$
\alpha_{k+1}=\alpha_k-\frac{2\alpha_k^2+\ln(2\alpha_k)}{4\alpha_k+1/\alpha_k}.
$$

Starting at $0.4$ gives $0.376376476$, $0.376544572$, and $0.376544582$. Moreover $h(0.3765)<0<h(0.3766)$ certifies the rounding. Thus **$\alpha=0.377$ to three significant figures**; more accurately $P\approx(0.3765445825,0.3765445825,-0.2835716452)$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [4](../../4.md)
3. [Continuous mathematics](../../../continuous-mathematics.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
