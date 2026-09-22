<h1 id="9/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $k\ge1$, the [event](../../../../../../event.md) $\{\lfloor X\rfloor\ge k\}$ equals $\{X\ge k\}$. Integrating the [Pareto distribution](../../../../../../pareto-distribution.md)'s density gives

$$
\boxed{\mathbb P(\lfloor X\rfloor\ge k)=k^{1-t},\qquad
\mathbb P(\lfloor X\rfloor=k)=k^{1-t}-(k+1)^{1-t}\quad(k\ge1).}
$$

The mass formula follows by subtracting consecutive tail probabilities, or by integrating over $[k,k+1)$. With the paper's convention $0\in\mathbb N$, include the separate endpoint values **$\mathbb P(\lfloor X\rfloor\ge0)=1$ and $\mathbb P(\lfloor X\rfloor=0)=0$**, since $X\ge1$ almost surely. Substituting $k=0$ into the power expression would be invalid.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
