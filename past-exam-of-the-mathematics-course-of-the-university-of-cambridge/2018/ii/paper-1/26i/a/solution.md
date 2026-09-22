<h1 id="26i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $d=\dim X$ and choose a local parametrization

$$
\phi:U\subseteq\mathbb R^d\longrightarrow X,
\qquad \phi(u_0)=p,
$$

whose derivative has rank $d$. Define

$$
T_pX=\operatorname{im}D\phi_{u_0}\subseteq\mathbb R^n.
$$

This is a vector subspace because it is the image of a linear map, and rank $D\phi_{u_0}=d$ gives $\dim T_pX=d$.

If $\psi$ is another local parametrization through $p$, the transition map $h=\psi^{-1}\circ\phi$ is a local diffeomorphism. The chain rule gives

$$
D\phi=D\psi\,Dh,
$$

and $Dh$ is invertible, so $\operatorname{im}D\phi=\operatorname{im}D\psi$. Thus the definition is independent of the parametrization. Equivalently, $T_pX$ is the set of velocity vectors of smooth curves in $X$ through $p$. This is the [tangent space from a local parametrization](../../../../../../tangent-space-from-a-local-parametrization.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26I](../../26i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
