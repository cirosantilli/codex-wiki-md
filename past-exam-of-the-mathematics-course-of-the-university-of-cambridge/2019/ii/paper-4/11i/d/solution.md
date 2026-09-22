<h1 id="11i/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Pure periodicity means that $\theta$ reappears as the tail after one period. The [continued-fraction tail formula](../../../../../../continued-fraction-tail-formula.md) therefore gives

$$
\theta=[a_0,\ldots,a_n,\theta]
=\frac{p_n\theta+p_{n-1}}{q_n\theta+q_{n-1}}.
$$

After cross-multiplication,

$$
\boxed{f(\theta)
=q_n\theta^2+(q_{n-1}-p_n)\theta-p_{n-1}=0.}
$$

Now let

$$
\eta=[\overline{a_n,a_{n-1},\ldots,a_0}].
$$

By part (c), the matrix for one reversed period is

$$
\begin{pmatrix}p_n&q_n\\p_{n-1}&q_{n-1}\end{pmatrix},
$$

so its positive fixed point $\eta$ satisfies

$$
p_{n-1}\eta^2+(q_{n-1}-p_n)\eta-q_n=0.
$$

Putting $\eta=-1/X$ and multiplying by $-X^2$ turns this equation into $f(X)=0$. The product of the two roots of $f$ is $-p_{n-1}/q_n<0$; because $\theta>0$, the other root $\theta'$ is negative. Consequently $-1/\theta'>0$ is the positive fixed point selected by convergence of the reversed continued fraction. The [reversed-period identity for a purely periodic continued fraction](../../../../../../reversed-period-identity-for-a-purely-periodic-continued-fraction.md) is therefore

$$
\boxed{-\frac1{\theta'}=[\overline{a_n,a_{n-1},\ldots,a_0}].}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [11I](../../11i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
