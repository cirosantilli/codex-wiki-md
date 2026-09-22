<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define

$$
R_X(\mu)=\sup_{\|v\|_2\leq1}
|\operatorname{MOM}_k(Xv)-\mu^Tv|.
$$

For every unit-ball vector $v$, the [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
|v^T(\widehat\mu-\mu_0)|
\leq|\operatorname{MOM}_k(Xv)-\widehat\mu^Tv|
+|\operatorname{MOM}_k(Xv)-\mu_0^Tv|.
$$

Taking the supremum and using optimality, $R_X(\widehat\mu)\leq R_X(\mu_0)$, yields

$$
\boxed{\|\widehat\mu-\mu_0\|_2
\leq R_X(\widehat\mu)+R_X(\mu_0)
\leq2R_X(\mu_0).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
