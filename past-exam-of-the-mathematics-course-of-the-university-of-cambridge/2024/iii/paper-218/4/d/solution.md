<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A binary [logistic regression](../../../../../../logistic-regression.md) sets

$$
\mathbb P(Y=1\mid X=x)
=\frac{1}{1+e^{-(\gamma_0+x^T\beta)}}
$$

and classifies by the sign of $\gamma_0+x^T\beta$. Its unpenalized [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) minimizes the empirical [logistic loss](../../../../../../logistic-loss.md)

$$
L(\gamma)=\sum_{i=1}^n
\log\left(1+e^{-Y_iX_i^{*T}\gamma}\right).
$$

The plotted data are [complete separation](../../../../../../complete-separation.md) data: there is a vector $v$ with every signed margin $Y_iX_i^{*T}v>0$. For every finite $c>0$, increasing $c$ strictly decreases each term of $L(cv)$, and $L(cv)\to0$ as $c\to\infty$. No finite parameter attains zero, so the unpenalized optimization has no solution.

Adding an $L^2$ penalty $\lambda\|\gamma\|_2^2$ with $\lambda>0$, constraining $\|\gamma\|_2$, or using a finite stopping rule makes the problem attain a finite approximate solution. The penalized option is preferable because [cross-validation](../../../../../../cross-validation.md) can select the strength of [regularization](../../../../../../regularization.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
