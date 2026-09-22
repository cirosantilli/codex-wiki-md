<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $u=\varphi+w$ with $w\in W_0^{1,2}(B)$. On this space define

$$
\mathcal B(w,z)=\int_B\alpha_{ij}D_jwD_i z.
$$

Boundedness of the coefficients makes $\mathcal B$ bounded, and ellipticity gives

$$
\mathcal B(w,w)\geq\gamma\lVert Dw\rVert_2^2,
$$

which is coercive by the [Poincaré inequality](../../../../../../poincare-inequality.md). The functional $z\mapsto-\mathcal B(\varphi,z)$ is bounded, so the [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) gives a unique $w$ and hence a unique weak solution $u$.

The supplied global [De Giorgi-Nash-Moser theorem](../../../../../../de-giorgi-nash-moser-theorem.md) and the weak maximum principle give $u\in C^{0,\beta}(\overline B)$ for some $\beta=\beta(n,\gamma,\Gamma)$. Finally, test the weak equation with $u\psi^2$. Ellipticity, the coefficient bound, and [Young inequality](../../../../../../young-s-inequality-for-products.md) yield

$$
\gamma\int_B|Du|^2\psi^2
\leq2\Gamma\int_B|u||Du||\psi||D\psi|
\leq\frac\gamma2\int_B|Du|^2\psi^2
+\frac{2\Gamma^2}{\gamma}\int_Bu^2|D\psi|^2.
$$

Rearranging gives

$$
\boxed{
\int_B|Du|^2\psi^2
\leq4\left(\frac\Gamma\gamma\right)^2
\int_Bu^2|D\psi|^2.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
