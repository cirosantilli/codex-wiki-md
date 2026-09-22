<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For student $i$ in school $j$, "lme1" is the [random-intercept linear mixed model](../../../../../../random-intercept-linear-mixed-model.md)

$$
\operatorname{THK}_{ij}
=\beta_0+\beta_1\operatorname{PTHK}_{ij}
+\beta_2\operatorname{TV}_j+\beta_3\operatorname{SC}_j
+b_j+\varepsilon_{ij},
$$

where

$$
b_j\overset{\rm iid}\sim N(0,\tau^2),
\qquad
\varepsilon_{ij}\overset{\rm iid}\sim N(0,\sigma^2),
$$

independently. The estimates are

$$
(\widehat\beta_0,\widehat\beta_1,\widehat\beta_2,\widehat\beta_3)
=(1.78880,0.30973,0.02175,0.47023),
$$



$$
\widehat\tau^2=0.0437,
\qquad
\widehat\sigma^2=1.6531.
$$

The fixed intercept is the population-average expected post-study score for an untreated reference student with PTHK zero. The random intercept $b_j$ is school $j$'s deviation from that population intercept.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
