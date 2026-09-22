<h1 id="a/3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First give the general definitions and radius facts. The [spectrum of a bounded operator](../../../../../spectrum-of-a-bounded-operator.md) is $\sigma(A)=\{\lambda:A-\lambda I\text{ has no bounded inverse}\}$, and the [point spectrum](../../../../../point-spectrum.md) is $p\sigma(A)=\{\lambda:\ker(A-\lambda I)\ne0\}$. If $|\lambda|>\|A\|$, the [Neumann series](../../../../../neumann-series.md) inverts $I-A/\lambda$, hence also $A-\lambda I=-\lambda(I-A/\lambda)$. Thus $\sigma(A)$ is contained in the closed disc of radius $\|A\|$ and is bounded.

The [spectral radius](../../../../../spectral-radius.md) is $\nu(A)=\sup_{\lambda\in\sigma(A)}|\lambda|$. The [spectral radius formula](../../../../../spectral-radius-formula.md) is

$$
\boxed{\nu(A)=\lim_{m\to\infty}\|A^m\|^{1/m}=\inf_{m\geq1}\|A^m\|^{1/m}.}
$$

For the left shift $R$, an eigenvector satisfies $a_{j+1}=\lambda a_j$, so $a_j=\lambda^{j-1}a_1$. A nonzero such sequence is in $\ell_1$ exactly when $|\lambda|<1$. Since $\|R\|=1$, its spectrum is contained in the closed unit disc. It contains the open unit disc as [point spectrum](../../../../../point-spectrum.md) and therefore its closure by closedness of the spectrum. Hence

$$
\boxed{p\sigma(R)=\{\lambda:|\lambda|<1\},\qquad\sigma(R)=\{\lambda:|\lambda|\leq1\}.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
