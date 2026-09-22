<h1 id="9/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $R$ count red balls and let $h_r$ be the probability of eventual absorption at $R=0$ starting from $R=r$. The [birth-death chain](../../../../../../birth-death-chain.md) moves to $r-1$ with probability $r/4$ and to $r+1$ with probability $(4-r)/4$. Its absorbing states have $h_0=1$, $h_4=0$. [First-step analysis](../../../../../../first-step-analysis.md) gives

$$
h_1=\frac14+\frac34h_2,\qquad h_2=\frac12h_1+\frac12h_3,\qquad h_3=\frac34h_2.
$$

Substitution yields $h_2=1/2$, $h_1=5/8$ and $h_3=3/8$. The initial state has one red ball, so **the probability that all balls end white is $5/8$**.

Absorption occurs almost surely: from each interior state there is probability at least $1/4$ of absorption within the next two draws. The chance of surviving $2m$ draws is therefore at most $(3/4)^m$. This also justifies the finite expected times used in part (ii). The process is the [absorbing four-ball Ehrenfest chain](../../../../../../absorbing-four-ball-ehrenfest-chain.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [9](../../../9.md)
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
