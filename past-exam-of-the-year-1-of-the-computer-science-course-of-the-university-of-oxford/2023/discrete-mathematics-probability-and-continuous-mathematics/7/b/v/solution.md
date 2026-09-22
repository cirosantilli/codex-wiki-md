<h1 id="7/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Put $\beta=1-2/n$. The fixed point of this [affine recurrence](../../../../../../affine-recurrence.md) is $n/2$. Subtracting it gives $r_{k+1}-n/2=\beta(r_k-n/2)$. Repeated substitution, or [mathematical induction](../../../../../../mathematical-induction.md), therefore yields

$$
\boxed{r_k=\frac n2+\frac n2\left(1-\frac2n\right)^k.}
$$

For $n>2$ this expression applies to every $k\ge0$. For $n=2$, state the initial value $r_0=2$ separately and obtain $r_k=1$ for every $k\ge1$, avoiding any need to interpret $0^0$. The expected red imbalance decays towards zero, although the urn composition itself remains random.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [B](../../b.md)
3. [7](../../../7.md)
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
