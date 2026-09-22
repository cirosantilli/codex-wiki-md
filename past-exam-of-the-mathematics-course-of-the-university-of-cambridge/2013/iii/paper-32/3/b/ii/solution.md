<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $U\sim N(\mu,s^2)$ and $a=(T-\mu)/s$, substitution $U=\mu+sZ$ gives

$$
\mathbb E[U\mathbf1_{\{U\geq T\}}]
=\mu[1-\Phi(a)]+s\int_a^\infty z\phi(z)\,dz
=\mu[1-\Phi(a)]+s\phi(a),
$$

since $\phi'(z)=-z\phi(z)$. Divide by $1-\Phi(a)$ to obtain the upper-truncated normal mean.

For $U=\widehat\delta_1$, set $\mu=\delta$, $s=1/\sqrt{I_1}$ and $T=f_1/\sqrt{I_1}$. Then $a=f_1-\delta\sqrt{I_1}$. Symmetry of the normal density and distribution yields

$$
\boxed{\mathbb E_\delta(\widehat\delta_1\mid C)
=\delta+\frac1{\sqrt{I_1}}
\frac{\phi(\delta\sqrt{I_1}-f_1)}{\Phi(\delta\sqrt{I_1}-f_1)}.}
$$

The ratio $r(x)=\phi(x)/\Phi(x)$ is an [Inverse Mills ratio](../../../../../../../inverse-mills-ratio.md). It is positive, and the pooled [estimator](../../../../../../../estimator.md)'s conditional bias is therefore

$$
b(\delta)=\frac{n_1}{n_2\sqrt{I_1}}r(\delta\sqrt{I_1}-f_1).
$$

This identity supplies both correction procedures below.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
