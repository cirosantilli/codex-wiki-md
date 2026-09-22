<h1 id="30j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [AdaBoost](../../../../../../adaboost.md) algorithm starts with weights $w_i^{(1)}=1/n$. For $m=1,\ldots,M$:

- choose $\widehat h_m\in B$ minimizing the weighted classification error$$
  \varepsilon_m=\sum_{i=1}^nw_i^{(m)}
  \mathbf1_{\{Y_i\ne\widehat h_m(X_i)\}};
  $$
- set$$
  \widehat\beta_m=\frac12\log\frac{1-\varepsilon_m}{\varepsilon_m};
  $$
- update and normalize$$
  w_i^{(m+1)}
  =\frac{w_i^{(m)}
  e^{-\widehat\beta_mY_i\widehat h_m(X_i)}}{
  \sum_jw_j^{(m)}
  e^{-\widehat\beta_mY_j\widehat h_m(X_j)}}.
  $$

Because $h\in B$ implies $-h\in B$, the selected classifier can always have weighted error at most $1/2$, so $\widehat\beta_m\geq0$. The output score is

$$
\boxed{\widehat f=\sum_{m=1}^M\widehat\beta_m\widehat h_m}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30J](../../30j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
