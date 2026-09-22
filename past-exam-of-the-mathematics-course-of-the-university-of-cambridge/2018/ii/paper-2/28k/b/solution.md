<h1 id="28k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [admissible estimator](../../../../../../admissible-estimator.md) is one for which there is no estimator $\delta$ satisfying

$$
R(\theta,\delta)\leq R(\theta,\widehat\theta)
$$

for every $\theta$, with strict inequality for at least one $\theta$. For $p\geq3$, the [James–Stein estimator](../../../../../../james-stein-estimator.md)

$$
\delta_{\rm JS}(X)=
\left(1-\frac{p-2}{\lVert X\rVert^2}\right)X
$$

has risk

$$
R(\theta,\delta_{\rm JS})
=p-(p-2)^2\mathbb E_\theta
\frac1{\lVert X\rVert^2}<p.
$$

It strictly dominates $X$, and hence

$$
\boxed{\widehat\theta_{\rm MLE}\text{ is inadmissible}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28K](../../28k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
