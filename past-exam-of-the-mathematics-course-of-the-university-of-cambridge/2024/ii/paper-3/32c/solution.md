<h1 id="32c/solution">Solution</h1>

↑ **Parent:** [32C](../32c.md)

A [vector](../../../../../vector.md) field $V=V_1\partial_x+\phi\partial_u$ is a Lie symmetry when

$$
\operatorname{pr}^{(N)}V(\Delta)=0
$$

on the equation manifold $\Delta=0$. With total [derivative](../../../../../derivative.md) $D_x$, the prolongation coefficients obey

$$
\phi_0=\phi,\qquad
\phi_{j+1}=D_x\phi_j-u^{(j+1)}D_xV_1.
$$

For $V_1=f(x)$, direct iteration gives

$$
\begin{aligned}
\phi_3={}&\phi_{xxx}+u'(3\phi_{xxu}-f''')+3(u')^2\phi_{xuu}
 +(u')^3\phi_{uuu}\\
&+3(\phi_{xu}-f''+u'\phi_{uu})u''+(\phi_u-3f')u'''.
\end{aligned}
$$

Thus $\alpha=\beta=3$.

For $u'''=u^{-3}$, invariance requires $\phi_3+3u^{-4}\phi=0$ after substituting $u'''=u^{-3}$. Equating coefficients of the independent jet variables gives

$$
\phi_{uu}=0,\qquad \phi_{xu}=f'',\qquad f'''=0,
$$

and the remaining terms force $\phi=(3a/4)u$ and $f=ax+b$. Hence the Lie algebra is spanned by

$$
\boxed{\partial_x,
\qquad
4x\partial_x+3u\partial_u.}
$$

## ↑ Ancestors (10)

1. [32C](../32c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
