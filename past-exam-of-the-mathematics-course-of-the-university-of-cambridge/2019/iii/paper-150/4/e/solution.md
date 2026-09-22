<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Assume $\beta$ exists and choose a reduced residue class $a$ with $\chi_1(a)=-1$; such a class exists because $\chi_1$ is nonprincipal. Fix a sufficiently large constant $A=A(\epsilon)$ and take

$$
x=\exp(A(\log q)^2).
$$

Then $x\geq q^2$ for large $q$. Multiplying the formula from part (d) by $\varphi(q)/x$ gives

$$
\frac{\varphi(q)}x\psi(x;q,a)
=1+\frac{x^{\beta-1}}{\beta}
+O\left(
\varphi(q)(\log q)^2
\exp\left[-\frac{cA\log q}{1+\sqrt A}\right]
\right).
$$

Choose $A$ so large that the error is at most $\epsilon/4$ for all sufficiently large $q$. The assumed upper bound then implies

$$
\frac{x^{\beta-1}}{\beta}\leq1-\frac{3\epsilon}4.
$$

Since $\beta<1$, this gives

$$
x^{\beta-1}\leq1-\frac{3\epsilon}4.
$$

Taking logarithms,

$$
(1-\beta)A(\log q)^2
\geq-\log\left(1-\frac{3\epsilon}4\right).
$$

Therefore, with a positive constant depending only on $\epsilon$,

$$
\boxed{\beta\leq1-\frac{c}{(\log q)^2}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
