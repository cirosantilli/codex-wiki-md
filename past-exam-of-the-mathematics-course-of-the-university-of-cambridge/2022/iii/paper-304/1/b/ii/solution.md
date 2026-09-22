<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose a real lift $\Delta\theta=\theta_f-\theta_i$. Classical paths fall into [winding number](../../../../../../../winding-number.md) sectors $j\in\mathbb Z$ and are

$$
\theta_j(t)=\theta_i+\frac{\Delta\theta+2\pi j}{T}t,
\qquad
S_j=\frac{mR^2}{2T}(\Delta\theta+2\pi j)^2.
$$

Each sector has the same fluctuation determinant, so the image-sum form of the propagator is

$$
K(\theta_f,T;\theta_i,0)
=\sqrt{\frac{mR^2}{2\pi i\hbar T}}
\sum_{j\in\mathbb Z}e^{iS_j/\hbar}.
$$

Set $a=\hbar T/(2mR^2)$. Applying the [Poisson summation formula](../../../../../../../poisson-summation-formula.md) to the Gaussian $e^{ix^2/(4a)}$ gives

$$
\frac1{\sqrt{4\pi ia}}
\sum_{j\in\mathbb Z}e^{i(\Delta\theta+2\pi j)^2/(4a)}
=\frac1{2\pi}\sum_{n\in\mathbb Z}e^{in\Delta\theta-ian^2},
$$

which is exactly the spectral propagator found in part i. Thus the angular-momentum sum is dual to a sum over homotopy classes of classical paths.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 304](../../../../paper-304-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
