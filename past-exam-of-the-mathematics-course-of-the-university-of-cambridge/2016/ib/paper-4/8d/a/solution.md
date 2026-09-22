<h1 id="8d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the numerical method to the scalar test equation $y'=\lambda y$, with $z=h\lambda$. Its [linear stability domain](../../../../../../linear-stability-domain.md) consists of those $z\in\mathbb C$ for which the discrete solution stays bounded as the step count tends to infinity. For a one-step method with [stability function](../../../../../../stability-function.md) $R$, this is

$$
\boxed{\mathcal S=\{z:|R(z)|\leq1\}.}
$$

If asymptotic decay is required, use $|R(z)|<1$ instead; this only changes the boundary conventions in part (b). A method is [A-stable](../../../../../../a-stability.md) if its stability domain contains the left half-plane, so every decaying linear test equation is stable for every positive step size. For a multistep method, the corresponding definition uses the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) for every characteristic root, including simplicity of unit-modulus roots.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8D](../../8d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
