<h1 id="s9/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

After three multiplicative steps, $k$ upward moves and $3-k$ downward moves give

$$
S_3(k)=100(1.1)^k(0.9)^{3-k}.
$$

For $k=0,1,2,3$, respectively, the prices are $\boxed{72.9,\ 89.1,\ 108.9,\ 133.1}$. Since the steps are independent, the endpoint [probabilities](../../../../../probability.md) are binomial:

$$
\boxed{\Pr(S_3=S_3(k))=\binom3k p^k(1-p)^{3-k}.}
$$

In the displayed ascending-price order they are $(1-p)^3$, $3p(1-p)^2$, $3p^2(1-p)$, and $p^3$. Different paths with the same count of up moves recombine because multiplication by $1.1$ and $0.9$ commutes.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [S9](../../../s9.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
