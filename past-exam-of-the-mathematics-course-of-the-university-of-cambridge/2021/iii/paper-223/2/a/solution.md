<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $q_s=F^{-1}(s)$ and $k=-F^{-1}(\alpha)>0$. Symmetry gives $F^{-1}(1-\alpha)=k$. Differentiating the [trimmed mean](../../../../../../trimmed-mean.md) functional along $F_t=(1-t)F+t\Delta_x$ gives

$$
\operatorname{IF}(x;T,F)
=\frac1{1-2\alpha}
\int_\alpha^{1-\alpha}
\frac{s-\mathbf1_{\{x\leq q_s\}}}{f(q_s)}\,ds.
$$

Under the substitution $y=q_s$, symmetry implies

$$
\int_\alpha^{1-\alpha}\frac{s}{f(q_s)}\,ds
=\int_{-k}^kF(y)\,dy=k,
$$

while

$$
\int_\alpha^{1-\alpha}
\frac{\mathbf1_{\{x\leq q_s\}}}{f(q_s)}\,ds
=\int_{-k}^k\mathbf1_{\{x\leq y\}}\,dy.
$$

Evaluating the last integral in the three regions $x<-k$, $|x|\leq k$, and $x>k$ yields

$$
\boxed{
\operatorname{IF}(x;T,F)
=\frac1{1-2\alpha}
\begin{cases}
-k,&x<-k,\\
x,&|x|\leq k,\\
k,&x>k.
\end{cases}}
$$

This is the [influence function of a trimmed mean](../../../../../../influence-function-of-a-trimmed-mean.md), namely the [Huber score](../../../../../../huber-score.md) with clipping parameter $k$, divided by $1-2\alpha$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
