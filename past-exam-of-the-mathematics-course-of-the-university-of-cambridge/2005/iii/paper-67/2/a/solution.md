<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For definiteness take $f$ in the [Schwartz space](../../../../../../schwartz-space.md); sufficiently smooth compactly supported data are also adequate. These hypotheses make the line integrals, [Cauchy principal values](../../../../../../cauchy-principal-value.md) and decay estimates below well defined. Write $\lambda=re^{i\theta}$ with $r>0$, $r\ne1$, and introduce orthonormal local coordinates

$$
\tau=x_1\cos\theta+x_2\sin\theta,\qquad
\rho=-x_1\sin\theta+x_2\cos\theta.
$$

Let $F(\tau,\rho,\theta)=f(x_1,x_2)$, $a_r=(r+r^{-1})/2$ and $b_r=(r-r^{-1})/2$. Substitution into the directional [transport equation](../../../../../../transport-equation.md) gives

$$
L_\lambda=a_r\partial_\tau-i b_r\partial_\rho.
$$

Now make the invertible real-linear change of coordinates

$$
\boxed{z=\tau-i\frac{a_r}{b_r}\rho,\qquad \nu(r)=2a_r=r+r^{-1}.}
$$

Since $\operatorname{Im}z=-a_r\rho/b_r$, its [Wirtinger derivative](../../../../../../wirtinger-derivatives.md) is $\partial_{\bar z}=(\partial_\tau-i b_r\partial_\rho/a_r)/2$. Hence $L_\lambda=\nu(r)\partial_{\bar z}$, as required. The change becomes singular at $r=1$, where the complex operator degenerates to a real directional derivative. Also the original equation contains $\lambda^{-1}$, so $\lambda=0$ is excluded from the differential equation; the normalized solution will extend analytically there.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
