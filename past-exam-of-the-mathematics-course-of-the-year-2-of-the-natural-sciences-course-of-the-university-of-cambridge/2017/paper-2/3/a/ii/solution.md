<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By translation and rotation invariance, use a radial [Green function](../../../../../../green-s-function-split.md) $G(R)$, where $R=|\mathbf r-\mathbf r'|$ is the [Euclidean distance](../../../../../../euclidean-distance.md). Away from the source, the radial [modified Helmholtz equation](../../../../../../modified-helmholtz-equation.md) is

$$
G''+\frac2R G'-k^2G=0.
$$

Writing $u=RG$ reduces this to $u''-\kappa^2u=0$, where $\kappa=|k|$. For $\kappa>0$, decay eliminates $e^{\kappa R}/R$, leaving $G=Ae^{-\kappa R}/R$. For $\kappa=0$, the two radial branches are a constant and $1/R$; decay again leaves $A/R$.

To fix the singular normalization, integrate the defining equation over a ball of radius $\varepsilon$ about $\mathbf r'$. The [divergence theorem](../../../../../../divergence-theorem.md) gives

$$
4\pi\varepsilon^2G'(\varepsilon)-k^2\int_{R<\varepsilon}G\,d^3\mathbf r=1.
$$

The volume term is $O(\varepsilon^2)$, whereas

$$
4\pi\varepsilon^2G'(\varepsilon)=-4\pi A e^{-\kappa\varepsilon}(1+\kappa\varepsilon)\longrightarrow-4\pi A.
$$

Consequently

$$
\boxed{A=-\frac1{4\pi},\qquad G(\mathbf r,\mathbf r')=-\frac{e^{-|k||\mathbf r-\mathbf r'|}}{4\pi|\mathbf r-\mathbf r'|}.}
$$

**Source qualification.** The printed $e^{-kR}$ is the decaying branch only when $k\geq0$, although the source declares $k$ real. For negative $k$ it grows, so it cannot be the requested decaying [Green function](../../../../../../green-s-function-split.md). The absolute value above covers every real $k$ and reduces to the printed form for nonnegative $k$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
