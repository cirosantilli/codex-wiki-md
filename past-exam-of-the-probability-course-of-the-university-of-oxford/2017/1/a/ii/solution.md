<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the inverse [change of variables for probability densities](../../../../../change-of-variables-for-probability-densities.md)

$$
x=vw,\qquad y=(1-v)w,\qquad 0<v<1,\quad w>0.
$$

Its absolute [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\left|\det\begin{pmatrix}w&v\\-w&1-v\end{pmatrix}\right|=w.
$$

Therefore

$$
\boxed{f_{V,W}(v,w)=w e^{-w}\mathbf1_{\{0<v<1,\ w>0\}}.}
$$

Since $\int_0^\infty we^{-w}\,dw=1$, its [marginal densities](../../../../../marginal-density.md) are $f_V(v)=\mathbf1_{(0,1)}(v)$ and $f_W(w)=we^{-w}\mathbf1_{(0,\infty)}(w)$. The joint density factorizes as $f_Vf_W$, so **$V$ and $W$ are [independent random variables](../../../../../independent-random-variables.md)**, with $V$ uniform on $[0,1]$ and $W\sim\operatorname{Gamma}(2,1)$ in the shape-rate convention. This is [beta-gamma independence](../../../../../beta-gamma-independence.md) with both shape parameters equal to one.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
