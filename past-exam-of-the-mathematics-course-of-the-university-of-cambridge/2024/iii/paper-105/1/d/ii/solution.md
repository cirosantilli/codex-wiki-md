<h1 id="1/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $L=d^2/dx^2+1$ with homogeneous [Dirichlet data](../../../../../../../dirichlet-boundary-condition.md) at $0$ and $2\pi$, [integration by parts](../../../../../../../integration-by-parts.md) shows that $L^*=L$. Its homogeneous kernel is

$$
\ker L=\operatorname{span}\{\sin x\},
$$

because $A\cos x+B\sin x$ vanishes at both endpoints exactly when $A=0$.

The forcing obeys the [orthogonality](../../../../../../../orthogonal-vectors.md) condition

$$
\int_0^{2\pi}\cos x\sin x\,dx=0.
$$

The [Fredholm alternative for an elliptic Dirichlet problem](../../../../../../../fredholm-alternative-for-an-elliptic-dirichlet-problem.md) therefore says that solutions exist, though they are not unique. Indeed,

$$
\boxed{u(x)=\frac{x}{2}\sin x+C\sin x}
$$

satisfies $u''+u=\cos x$ and both boundary conditions for every constant $C$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
