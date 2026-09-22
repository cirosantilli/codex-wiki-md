<h1 id="s/s2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For one proposal, $P(Y=x,\text{accept})=q(x)\tilde p(x)/(M\tilde q(x))=\tilde p(x)/(MZ_q)$. Summing gives total acceptance probability $a=Z_p/(MZ_q)>0$. Conditioning on acceptance therefore gives $P(Y=x\mid\text{accept})=\tilde p(x)/Z_p=p(x)$.

The first accepted result has this law too: the probability of $k-1$ failures followed by acceptance at $x$ is $(1-a)^{k-1}\tilde p(x)/(MZ_q)$. Sum the [geometric series](../../../../../geometric-series.md) over $k\ge1$ to obtain $\boxed{P(X=x)=p(x)}$. Positive acceptance probability also proves almost-sure termination.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [S2](../../s2.md)
3. [S](../../../s.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
