<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First perform [homogenization of Dirichlet boundary data](../../../../../../homogenization-of-dirichlet-boundary-data.md): put $v=u-\psi\in H_0^1(B_1^+)$ and $g=f-\Delta\psi\in L^2(B_1^+)$. Then $\Delta v=g$ weakly. Extend both functions oddly across the flat face:

$$
\widetilde v(x',t)=\begin{cases}v(x',t)&t>0,\\-v(x',-t)&t<0,\end{cases}\qquad\widetilde g(x',t)=\begin{cases}g(x',t)&t>0,\\-g(x',-t)&t<0.\end{cases}
$$

The zero [Sobolev trace](../../../../../../trace-operator.md) of $v$ makes this [odd reflection](../../../../../../odd-reflection.md) an $H^1(B_1)$ function. This can also be seen by approximating $v$ by smooth [compactly supported](../../../../../../compact-support.md) functions in $B_1^+$ and reflecting the approximants. Its $H^1$ [norm](../../../../../../norm.md) is $\sqrt2$ times that of $v$, and $\|\widetilde g\|_{L^2(B_1)}=\sqrt2\|g\|_{L^2(B_1^+)}$.

For $\phi\in C_c^\infty(B_1)$, the function $\phi(x',t)-\phi(x',-t)$ on the upper half-ball has zero trace on the flat face and vanishes near the curved face, hence is an admissible $H_0^1$ test. Splitting the integrals over the two half-balls and changing $t$ to $-t$ shows

$$
\int_{B_1}D\widetilde v\cdot D\phi=-\int_{B_1}\widetilde g\phi.
$$

Thus $\Delta\widetilde v=\widetilde g$ weakly throughout the full ball; there is no extra distribution on the reflecting face.

Apply part (i) to $B_{1/2}\Subset B_1$, restrict to the upper half-ball, and then add $\psi$. Since $\|\Delta\psi\|_2\leq C(n)\|\psi\|_{H^2}$, this gives $u\in W^{2,2}(B_{1/2}^+)$ and the [second-derivative estimate at a flat Dirichlet boundary](../../../../../../second-derivative-estimate-at-a-flat-dirichlet-boundary.md)

$$
\boxed{\|u\|_{W^{2,2}(B_{1/2}^+)}\leq C(n)\left(\|u\|_{W^{1,2}(B_1^+)}+\|f\|_{L^2(B_1^+)}+\|\psi\|_{W^{2,2}(B_1^+)}\right).}
$$

The fixed radii leave distance $1/2$ for the interior estimate, so the constant depends only on dimension.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
