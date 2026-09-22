<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

For square-integrable wavefunctions with the stated decay, multiplication by the real coordinate $x$ is [Hermitian](../../../../../hermitian-operator.md) because

$$
\langle\psi,x\chi\rangle=\langle x\psi,\chi\rangle.
$$

For $p_x=-i\hbar\partial_x$, [integration by parts](../../../../../integration-by-parts.md) gives

$$
\langle\psi,p_x\chi\rangle
=\langle p_x\psi,\chi\rangle
-i\hbar\int_{-\infty}^{\infty}[\overline\psi\chi]_{x=-\infty}^{x=\infty}\,dy,
$$

and the boundary term vanishes. The same arguments apply to $y$ and $p_y$.

If $F$ and $G$ are Hermitian on a common suitable domain, then $(FG)^\dagger=GF$, so

$$
\left[\frac12(FG+GF)\right]^\dagger
=\frac12(FG+GF).
$$

Because $x$ commutes with $p_y$ and $y$ with $p_x$,

$$
L=xp_y-yp_x
$$

is Hermitian. Using $p_xx=xp_x-i\hbar$ and its $y$ analogue,

$$
D=\frac12(xp_x+p_xx+yp_y+p_yy)
=-i\hbar(x\partial_x+y\partial_y+1),
$$

so $D$ is Hermitian as well.

Finally set $R=x\partial_y-y\partial_x$ and $S=x\partial_x+y\partial_y$. Direct evaluation on a smooth test function gives $[R,S]=0$: rotations commute with radial dilations. The scalar term in $D$ also commutes with everything, and therefore

$$
\boxed{[L,D]=0}.
$$

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
