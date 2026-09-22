<h1 id="3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Gowers U3 norm](../../../../../../gowers-u3-norm.md) derivative identity is

$$
\|F\|_{U^3(G)}^8=\mathbb E_{h\in G}\|\partial_hF\|_{U^2(G)}^4.
$$

Let $\kappa=\|F\|_{U^3(G)}^8$. Since $\|I\|_{U^3(G)}\geq\mathbb E I=N/M\geq1/16$, by repeated [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md), the interval hypothesis gives $\kappa\geq16^{-8}\delta^8$. Also $\|\partial_hF\|_{U^2}^4\leq1$. Therefore the set

$$
H=\{h:\|\partial_hF\|_{U^2}^4\geq\kappa/2\}
$$

has density at least $\kappa/2$ in $G$.

Use normalized [Fourier coefficients on a finite abelian group](../../../../../../fourier-coefficient-on-a-finite-abelian-group.md) $\widehat g(k)=\mathbb E_xg(x)e(-kx/M)$. The [Gowers U2 norm](../../../../../../gowers-u2-norm.md) and [Parseval identity](../../../../../../parseval-identity.md) give

$$
\|g\|_{U^2}^4=\sum_k|\widehat g(k)|^4\leq\left(\max_k|\widehat g(k)|^2\right)\mathbb E_x|g(x)|^2.
$$

For $g=\partial_hF$, the final mean is at most one. Thus each $h\in H$ has a frequency $\theta(h)=k_h/M$ with

$$
\boxed{|\mathbb E_x\partial_hF(x)e(-\theta(h)x)|\geq(\kappa/2)^{1/2}\gg\delta^4.}
$$

The derivative is identically zero unless $h$ is represented by an integer in $[-N+1,N-1]$, so $H$ lies in the requested interval of shifts. Its size is $\gg\delta^8M\gg\delta^8N$. Keep one such frequency for each shift; these same choices will satisfy the energy conclusion below.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [3](../../3.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
