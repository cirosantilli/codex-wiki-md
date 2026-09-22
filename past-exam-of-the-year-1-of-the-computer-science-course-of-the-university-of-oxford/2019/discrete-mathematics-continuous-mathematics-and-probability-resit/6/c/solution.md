<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $P=\mathbf z\mathbf z^T$, so $P^2=r^2P$ and $f^2=1+r^2$. Multiplying the proposed [inverse matrix](../../../../../matrix-inverse-split.md) by the [Hessian](../../../../../hessian-matrix.md) gives

$$
\left(\frac I f-\frac P{f^3}\right)f(I+P)=I+P-\frac{P+P^2}{f^2}=I.
$$

Hence **$\displaystyle H_f^{-1}=f(I+\mathbf z\mathbf z^T)=f\begin{pmatrix}1+x^2&xy\\xy&1+y^2\end{pmatrix}$**, as required. Its existence also follows from the [Hessian](../../../../../hessian-matrix.md) being a [positive-definite matrix](../../../../../positive-definite-matrix.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics, and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
