<h1 id="14a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [Green second identity](../../../../../../green-second-identity.md) to $u$ and the free-space [Green function](../../../../../../green-s-function.md) $G_{fs}$ on $V$ with a small ball about $\mathbf r_0$ removed. Both functions are harmonic there, so only boundary terms remain. The contribution from the small sphere tends to $u(\mathbf r_0)$ because

$$
G_{fs}(\mathbf r;\mathbf r_0)=-\frac1{4\pi|\mathbf r-\mathbf r_0|}
$$

has unit delta source, while the remaining small-sphere term vanishes. Taking the radius to zero gives [Green's third identity](../../../../../../green-s-third-identity.md)

$$
\boxed{
u(\mathbf r_0)=
\int_S\left(u\frac{\partial G_{fs}}{\partial n}
-G_{fs}\frac{\partial u}{\partial n}\right)dS}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14A](../../14a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
