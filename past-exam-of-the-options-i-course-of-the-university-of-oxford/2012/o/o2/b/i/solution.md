<h1 id="o/o2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The design columns are $1$, $x$ and $z$. Their pairwise inner products are zero by the three supplied sums. Put $S_{xx}=\sum_ix_i^2$ and $S_{zz}=\sum_iz_i^2$, positive under the full-rank assumption. Then

$$
X^TX=\operatorname{diag}(n,S_{xx},S_{zz}).
$$

Applying part (a),

$$
\boxed{\widehat\theta=\begin{pmatrix}\widehat\alpha\\\widehat\beta\\\widehat\gamma\end{pmatrix}
=\begin{pmatrix}\overline Y\\\displaystyle\frac{\sum_ix_iY_i}{S_{xx}}\\\displaystyle\frac{\sum_iz_iY_i}{S_{zz}}\end{pmatrix},
\qquad
\operatorname{Var}(\widehat\theta)=\sigma^2\operatorname{diag}\left(\frac1n,\frac1{S_{xx}},\frac1{S_{zz}}\right).}
$$

The off-diagonal covariances vanish because the design columns are [orthogonal](../../../../../../orthogonal-vectors.md). With Gaussian errors, the coefficient estimators are also jointly normal and therefore independent.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [O2](../../../o2.md)
4. [O](../../../../o.md)
5. [2012](../../../../../2012-split.md)
6. [Past exam of the options I course of the University of Oxford](../../../../../split.md)
7. [Options I course of the University of Oxford](../../../../../../options-i-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
