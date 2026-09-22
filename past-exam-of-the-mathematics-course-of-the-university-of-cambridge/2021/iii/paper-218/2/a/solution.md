<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For user $j$ and offer $r$, both fits use

$$
\operatorname{logit}(p_j)=\beta_0+\beta_1\operatorname{age}_j+\beta_2\operatorname{fitness}_j
+\gamma_{\operatorname{region}_j}+\delta_{\operatorname{sex}_j}.
$$

The first model treats each click as Bernoulli$(p_j)$. The grouped model treats the click count $C_j=m_j\operatorname{prop}_j$ as $\operatorname{Bin}(m_j,p_j)$. Their likelihoods differ only by binomial coefficients independent of the parameters, so their fitted coefficients agree.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
