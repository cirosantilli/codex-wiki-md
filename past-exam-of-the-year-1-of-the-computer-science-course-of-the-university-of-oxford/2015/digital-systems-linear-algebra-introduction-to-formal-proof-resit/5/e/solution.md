<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Find a [stationary distribution](../../../../../stationary-distribution.md) $\boldsymbol\pi=(u,v,w)^T$ from $P\boldsymbol\pi=\boldsymbol\pi$ and $u+v+w=1$. The first two independent [linear equations](../../../../../linear-equation.md) are

$$
4u-2v-w=0,\qquad -2u+3v-3w=0.
$$

They give $u=9w/8$ and $v=7w/4$. Normalization gives $w=8/31$, hence

$$
\boxed{\boldsymbol\pi=\frac1{31}\begin{pmatrix}9\\14\\8\end{pmatrix},\qquad
P^n\begin{pmatrix}1\\0\\0\end{pmatrix}\longrightarrow\boldsymbol\pi.}
$$

To justify the limit using the assumptions, distinct [eigenvalues](../../../../../eigenvalue.md) give an [eigenbasis](../../../../../eigenbasis.md), over the [complex numbers](../../../../../complex-number.md) if necessary. Choose $\boldsymbol\pi$ as the [eigenvector](../../../../../eigenvector.md) for 1 and let $\mathbf v_2,\mathbf v_3$ correspond to the other [eigenvalues](../../../../../eigenvalue.md) $\lambda_2,\lambda_3$. Expand the initial [probability distribution](../../../../../probability-distribution-split.md) as

$$
\mathbf p_0=\alpha\boldsymbol\pi+\beta\mathbf v_2+\gamma\mathbf v_3.
$$

Since $\mathbf1^TP=\mathbf1^T$, each $\lambda_j\ne1$ satisfies

$$
\mathbf1^T\mathbf v_j=\mathbf1^TP\mathbf v_j
=\lambda_j\mathbf1^T\mathbf v_j,
\qquad\text{so}\qquad\mathbf1^T\mathbf v_j=0.
$$

Multiplying the expansion by $\mathbf1^T$ therefore gives $\alpha=1$. It follows that

$$
P^n\mathbf p_0=\boldsymbol\pi+\beta\lambda_2^n\mathbf v_2
+\gamma\lambda_3^n\mathbf v_3\longrightarrow\boldsymbol\pi,
$$

because $|\lambda_2|,|\lambda_3|<1$. The components of the limiting [probability distribution](../../../../../probability-distribution-split.md) are approximately $0.2903,0.4516,0.2581$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
